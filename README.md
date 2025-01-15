# docker_install

**1. Xóa kho Docker cũ (nếu có)**

Trước tiên, hãy chắc chắn rằng bạn không còn sử dụng kho Docker cũ. Bạn có thể gỡ bỏ Docker và xóa kho Docker hiện tại.
Gỡ bỏ Docker nếu đã cài trước đó:

```
sudo apt remove docker docker-engine docker.io containerd runc
```

Xóa kho Docker hiện tại (nếu đã thêm):

```
sudo rm /etc/apt/sources.list.d/docker.list
```

**2. Cài đặt kho Docker chính thức**

Để đảm bảo bạn sử dụng kho chính thức của Docker, làm theo các bước sau:

Cài đặt các gói phụ thuộc:

```
sudo apt update
sudo apt install -y ca-certificates curl gnupg lsb-release
```

Thêm kho Docker chính thức:

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo tee /etc/apt/trusted.gpg.d/docker.asc
echo "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

**3. Cập nhật và cài đặt Docker**

Bây giờ, bạn có thể cài đặt Docker Engine từ kho chính thức:

```
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
```

**4. Kiểm tra Docker đã cài đặt chưa**

Sau khi cài đặt thành công, kiểm tra phiên bản Docker:

```
docker --version
```

**5. Cài đặt Docker Compose (Nếu cần)**

Docker Compose là một công cụ mạnh mẽ để chạy nhiều container Docker cùng lúc.

Bạn có thể cài Docker Compose theo các bước sau:

Tải Docker Compose:

```
sudo curl -L "https://github.com/docker/compose/releases/download/$(curl -s https://api.github.com/repos/docker/compose/releases/latest | jq -r .tag_name)/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

Cấp quyền thực thi:

```
sudo chmod +x /usr/local/bin/docker-compose
```

Kiểm tra phiên bản Docker Compose:

```
docker-compose --version
```

**6. Kiểm tra Docker đang chạy**

Bật và kiểm tra trạng thái của Docker:

```
sudo systemctl enable docker
sudo systemctl start docker
sudo systemctl status docker
```

**7. Thêm người dùng vào nhóm Docker (tuỳ chọn)**

Để sử dụng Docker mà không cần sudo, thêm người dùng vào nhóm Docker:

```
sudo usermod -aG docker $USER
```

Sau đó, đăng xuất và đăng nhập lại, hoặc khởi động lại máy chủ để thay đổi có hiệu lực.
