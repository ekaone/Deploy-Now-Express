## Deploy a Basic Node App using Now

Cretae `now.json` and set your desired `route` like an example below:
```
{
  "version": 2,
  "builds": [{ "src": "index.js", "use": "@now/node-server" }],
  "routes": [
    {
      "src": "/users",
      "dest": "/index.js",
      "methods": ["GET"]
    },
    {
      "src": "/user",
      "dest": "/index.js",
      "methods": ["POST"]
    }
  ]
}
```
