# Request Header Parser Microservice

![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)

Request Header Parser Microservice is the 2nd project for FreeCodeCamp *Back End Development and APIs* course. It returns a JSON that contains three headers
from a user request: **ip address**, **accept language** and **user agent**.

🙏 Credits
---
![FreeCodeCamp](https://img.shields.io/badge/Freecodecamp-%23123.svg?&style=for-the-badge&logo=freecodecamp&logoColor=green)

Everything **not** written by me has been cloned from [this GitHub repository](https://github.com/freeCodeCamp/boilerplate-project-headerparser/).

The default README that comes with the cloned repository:
> This is the boilerplate for the Request Header Parser Microservice project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/request-header-parser-microservice

Here is the solution I wrote for this project:
```
//My additions

app.get("/api/whoami", function(req, res)
{
  return res.json({
    ipaddress: req.ip,
    language: req.headers["accept-language"],
    software: req.headers["user-agent"],
  });
});
```
