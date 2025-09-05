
# Node.js + Express Setup (Commands Only)

**Run these commands in order:**

```bash
npm init -y
npm install express
npm run dev
# (to stop the server) press: Ctrl + C
npm i nodemon
npm install ejs
```

**package.json script (add after the `test` command):**
```json
"dev": "node index.js"
```

**Write your code in `index.js`.**

---

## package.json (example)

```json
{
  "name": "node-express-setup",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "node index.js"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "dependencies": {
    "express": "^4.19.2",
    "ejs": "^3.1.10"
  },
  "devDependencies": {
    "nodemon": "^3.1.0"
  }
}
```

---

## Theory: Node.js and Express.js (Short & Simple)

**What is Node.js?**
- A JavaScript runtime built on Chrome’s V8 engine.  
- Used for writing JavaScript on the server side.  
- Has a non-blocking, event-driven architecture — meaning it can handle many requests at the same time efficiently.  

**What is Express.js?**
- A lightweight web framework built on top of Node.js.  
- Makes routing (handling URLs), middleware (processing between request and response), and views/templates (like EJS) easier.  
- Very popular for rapid web development.  

**What does EJS do?**
- A templating engine (“Embedded JavaScript”).  
- Lets you write JavaScript inside HTML to create dynamic pages (e.g., `<%= user.name %>`).  

**What is Nodemon used for?**
- A development tool that automatically restarts the server when you save changes to files.  
- Instead of running with `node`, you can use `nodemon` (e.g., `"dev": "nodemon index.js"`).  

**Request → Response basic flow**
1. Client (browser or Postman) sends a request (`GET /`).  
2. Express matches the request with a route.  
3. Middleware/handler code runs.  
4. Server sends back a response (HTML, JSON, text, etc.).  

That’s it — now you can write your Express server code inside `index.js` and run it using `npm run dev`.  
