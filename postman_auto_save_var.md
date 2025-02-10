```
var responseJSON = pm.response.json();
pm.collectionVariables.set("X-Access-Token", responseJSON.token);
pm.collectionVariables.set("authorization", responseJSON.token);

```
