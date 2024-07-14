# Assignment: Virtual Whiteboard
![Virtual White Board](https://0x0.st/XLfJ.png)

## Objective:
Build a virtual whiteboard application that allows real-time collaboration between multiple users. The whiteboard should support basic drawing functionalities as depicted in the provided image, including a pencil, line, rectangle, delete button, and color picker in the toolbar.

## Requirements:

### 1. Backend (Node.js):
- Set up a Node.js server using Express.
- Use WebSockets (e.g., Socket.io) for real-time communication between clients.
- Implement RESTful API endpoints for the following operations:
  - Create a new whiteboard session.
  - Save the current state of a whiteboard session.
  - Retrieve a saved whiteboard session.
- Use PostgreSQL to store whiteboard session data.
- Implement basic validation and error handling.

### 2. Frontend (React):
- Create a React application that interacts with the backend API and uses WebSockets for real-time updates.
- Implement the following features:
  - A canvas where users can draw using different tools (pencil, line, rectangle, eraser, and color picker) as shown in the provided image.
  - Real-time synchronization of drawing actions between multiple users.
  - Save the current whiteboard session.
  - Load a saved whiteboard session.
  - Basic UI for selecting tools and colors, mimicking the toolbar in the image.
- Use React hooks and functional components.
- Style the application using Tailwind CSS to ensure it is user-friendly and responsive.

### 3. Database:
- Design a schema for storing whiteboard sessions in PostgreSQL, which should include at least:
  - `sessionId` (unique identifier)
  - `sessionData` (serialized data representing the whiteboard state)
  - `createdAt` (timestamp)
  - `updatedAt` (timestamp)

### 4. Additional Requirements:
- Ensure that multiple users can draw on the whiteboard simultaneously and see each other's updates in real-time.
- Implement a simple authentication mechanism to identify users (optional, for an added challenge).
- Document the application setup and usage in a README file.
- Deploy the application to a cloud service (e.g., Heroku, Vercel) and provide a demo URL.

## Submission:
- Once the assignment is complete, push the code to a public GitHub repository.
- Share the GitHub repository URL and the deployed application URL.

## Evaluation Criteria:
- Code quality and structure.
- Correctness and completeness of the implemented features.
- UI/UX design and responsiveness.
- Real-time collaboration functionality.
- Proper use of version control.
- Documentation (README file with instructions on how to set up and run the application).
- Successful deployment and working demo.

## Steps to Get Started:

### 1. Backend:
- Initialize a Node.js project.
- Set up Express and Socket.io.
- Create API routes for creating, saving, and retrieving whiteboard sessions.
- Connect to PostgreSQL and implement CRUD operations for whiteboard sessions.

### 2. Frontend:
- Initialize a React project.
- Create components for the whiteboard canvas and tool selection based on the provided image.
- Set up WebSocket communication for real-time drawing synchronization.
- Implement API calls to save and retrieve whiteboard sessions.

### 3. Database:
- Set up PostgreSQL and define the schema for storing whiteboard sessions.

### 4. Styling and Testing:
- Use Tailwind CSS to style the frontend and make it user-friendly.
- Test the application to ensure real-time collaboration works correctly.

### 5. Deployment:
- Deploy the application to a cloud service.
- Provide the demo URL in the README file.

## Sample API Endpoints:

- **Create Whiteboard Session:**
```
POST /api/sessions
Body: {
  "sessionId": "unique-id"
}
```


- **Save Whiteboard Session:**
```
PUT /api/sessions/
Body: {
  "sessionData": "serialized-whiteboard-data"
}
```

- **Retrieve Whiteboard Session:**
```
GET /api/sessions/
```


## Sample React Components:

- **WhiteboardCanvas:** Component for the drawing canvas.
- **Toolbox:** Component for selecting drawing tools and colors, as depicted in the provided image.
- **SaveLoadControls:** Component for saving and loading whiteboard sessions.

Good luck! If you have any questions, feel free to ask.

