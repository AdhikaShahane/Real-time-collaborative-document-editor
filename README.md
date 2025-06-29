# Real-time-collaborative-document-editor

COMPANY: CODTECH IT SOLUTION

NAME: ADHIKA SHAHANE

INTERN ID: CT1MTDF577

DOMAIN: FRONT END DEVELOPMENT

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

in this This project is a simplified clone of  Docs that allows users to create, edit, and collaborate on documents in real-time. It’s built as a full-stack web application using modern technologies including React for the frontend, Node.js + Express for the backend, Socket.IO for real-time communication, and Tailwind CSS for styling.The frontend is created using React, a popular JavaScript library for building user interfaces. The main part of the interface is a rich text editor, where users can type and format their content. For this, we use a ready-made component like React Quill which supports bold text, italics, headings, bullet points, and more.To make the app look clean and modern, we use Tailwind CSS, a utility-first CSS framework. It allows us to style the app quickly using class , and font-bold without writing separate CSS rules.When the user edits the document, changes are sent instantly to the server using WebSockets, and other users connected to the same document will see those changes live. This creates a real-time collaborative editing experience.
The backend server is built using Node.js and Express and handles WebSocket communication using Socket.IO.
When a user joins a document, the server adds them to a unique "room" (based on the document ID).
As users make changes, the server listens for updates and broadcasts them to others in the same room.
Optionally, document content can be saved to a MongoDB database to persist changes across sessions.

Frontend: React, Tailwind CSS, React Quill
Backend: Node.js, Express.js, Socket.IO
Real-time Communication: WebSockets (via Socket.IO)
the client-server interaction is handled using both HTTP and WebSockets. When the user opens the app in their browser, the React frontend loads via a standard HTTP request. After loading, the frontend establishes a WebSocket connection with the Node.js + Express backend using Socket.IO. Once connected, the client joins a specific "document room" by sending the document ID to the server. As the user types, their changes are sent in real-time to the server, which then broadcasts these updates to all other clients in the same room, enabling live collaboration. This two-way communication keeps all users’ editors synchronized instantly. Also optinaly , the server can also save the document to a database for later retrieval.




