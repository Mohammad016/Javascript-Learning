# Javascript-Learning
A fresh learning of JavaScript


## Difference in syntax between js and node js

**JavaScript (JS)** is a *language*. **Node.js** is a *runtime environment* that allows you to run JavaScript outside the browser (e.g., on a server).

So the core language syntax is the same — but what differs is:

The **execution context** (browser vs server)

The **APIs available**
```text
Browser JS gives you:

  DOM APIs (document, querySelector, etc.)
  fetch, 
  localStorage, 
  sessionStorage


Node.js gives you:

  File system (fs)
  HTTP server (http)
  Path utilities (path)
  Buffer, streams, crypto, etc.

```

The **module system**
[Java script project code](https://github.com/Mohammad016/Javascript-Learning/blob/main/javascriptProjects.md)

___
**Hosting**
```text
  A website is just a bunch of files (HTML, CSS, images, JS).
  A host is where you park those files so anyone on the internet can access them.

What Is a Server?

A server is simply a computer (like yours) that:
	•	Runs 24/7
	•	Listens for requests (like from your browser)
	•	Responds with something (like HTML, JSON, or files)

When you visit a website like example.com, your browser sends a request to a server.
The server runs some code (maybe in Node.js or Python), fetches data (maybe from a database), and sends a response.

Hosting a Server Means 3 Things
	1.	You write backend code (e.g., in Node.js, Express, Python Flask, etc.)
	2.	You run that code on a machine (your own or in the cloud)
	3.	You make it publicly accessible via a domain or IP address

```
*Example*
In Local
---

```javascript
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello from server!");
});

app.listen(3000, () => {
  console.log("Server running on http://localhost:3000");
});
```
	•	This script creates a server on your machine.
	•	It listens for requests on port 3000.
	•	If you open http://localhost:3000 in your browser, you’ll see "Hello From Server!"

Host This on the Internet
---
1. Choose a cloud host
     ```text
    •Free/Beginner-friendly:
      	•	Render
      	•	Railway
      	•	Vercel (frontend mostly)
      	•	Glitch
     
    •Professional/Advanced:
      	•	AWS (EC2, Elastic Beanstalk)
      	•	DigitalOcean
      	•	Heroku (used to be free)
     ```
2. Upload your server code
     ```text
       •	You can connect your GitHub repo to these services
       •	Or use their command-line tools to deploy your project
     ```
3. They assign a domain or IP
   ```text
   Railway might give : https://your-app.railway.app
   Vercel might give : https://your-app.vercel.app
   ```
Once your server is live, you can:

	•	Connect a database (MongoDB, PostgreSQL)
	•	Add authentication (login/signup)
	•	Handle file uploads
	•	Connect to a frontend (like a React app or static site)
