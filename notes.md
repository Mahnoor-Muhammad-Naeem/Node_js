## Theory: Node.js aur Express.js (Short & Simple)

**Node.js kya hai?**
- Chrome V8 engine par chalne wala JavaScript runtime.
- Server-side JavaScript likhne ke liye use hota hai.
- Non-blocking, event-driven architecture hai — yani ek waqt me bohat saari requests handle kar sakta hai.

**Express.js kya hai?**
- Node.js ke upar ek lightweight web framework.
- Routing (URLs ko handle karna), middleware (request/response ke beech processing), views/templates (jaise EJS) ko asaan banata hai.
- Rapid development ke liye bohat mashhoor hai.

**EJS kya karta hai?**
- “Embedded JavaScript” templating engine.
- HTML ke andar JS likh ke dynamic pages banane deta hai (e.g., `<%= user.name %>`).

**Nodemon kis kaam ka?**
- Development tool jo file save hote hi server ko auto-restart karta hai.
- Aap command mein `node` ki jagah `nodemon` use karte ho (agar chaho to `"dev": "nodemon index.js"` bhi rakh sakte ho).

**Request → Response ka basic flow**
1. Client (browser/postman) request bhejta hai (`GET /`).
2. Express route us request ko match karta hai.
3. Middleware/handler code run hota hai.
4. Server response bhej deta hai (HTML, JSON, text, etc.).

Itna hi — ab aap `index.js` me Express server code likh ke `npm run dev` se chala sakte ho.
