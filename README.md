The content is for vercel.json file that should be added in root directory.

{
    "version": 2,
    "builds": [
      {
        "src": "app.js",         //index.js , server.js according to the server file name
        "use": "@vercel/node"
      }
    ],
    "routes": [
      {
        "src": "/(.*)",
        "dest": "app.js"             //index.js , server.js according to the server file name
      }
    ]
  }
