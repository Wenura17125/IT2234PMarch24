# IT2234P Web Services and Server Technologies

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Code Quality](https://img.shields.io/badge/Code%20Quality-A-brightgreen?style=for-the-badge)]()


> 📚 A comprehensive collection of practical lessons for Web Services and Server Technologies course.

## 📋 Course Overview

This repository serves as a practical guide through various web services and server technologies, focusing on building RESTful APIs with Node.js. Each implementation includes both source code and visual outputs from testing.

## 🗓️ Latest Session: Building RESTful API with Node.js (March 24, 2025)

### 🎯 Learning Objectives

- Set up a basic HTTP server using Node.js
- Implement RESTful API endpoints
- Work with student data management
- Test API endpoints using Postman
- Handle different HTTP methods and responses

### 💻 Implementation Details

#### 1. Server Setup

The server is implemented using Node.js's built-in HTTP module:

```javascript
const {createServer} = require('node:http');

const localhost = '127.0.0.1';
const port = 3000;
const server = createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end("Hello Node JS");
});

server.listen(port, localhost, () => {
    console.log(`Running on: ${localhost}:${port}`);
});
```

#### 2. Student Database

A sample student database is implemented with the following structure:

```javascript
let students = [
    {regno:'2020ict32', name:'anushika', gender:'f', age:'25', course:'ICT'},
    {regno:'2020ict125', name:'wenura', gender:'m', age:'25', course:'ICT'},
    {regno:'2020ict78', name:'mekala', gender:'f', age:'24', course:'ICT'},
    {regno:'2020ict56', name:'shanaka', gender:'m', age:'23', course:'ICT'},
    {regno:'2020ict06', name:'hasala', gender:'m', age:'23', course:'ICT'},
];
```

### 📊 Implementation Results

| Test Case | Description | Output |
|-----------|-------------|--------|
| Server Setup | Basic HTTP server initialization | [View](output/serverCmd.png) |
| Server Response | Testing server response in browser | [View](output/serverWeb.png) |
| Postman Testing | Testing API endpoints with Postman | [View](output/postmanServer.png) |
| Student Data | Retrieving student information | [View](output/postmanApp.png) |
| Student by ID | Finding specific student by ID | [View](output/postmanAppStuid.png) |
| Found Student | Successfully retrieved student data | [View](output/postmanFoundStudent.png) |
| Gender Analysis | Student gender distribution | [View](output/gender.png) |

### 🔍 Technical Notes

- Server implemented using Node.js HTTP module
- RESTful API endpoints for student data management
- In-memory student database implementation
- Comprehensive testing using Postman
- Visual documentation of all API responses

---

<div align="center">

📖 **API Documentation** | 🛠️ **Implementation Examples** | 📊 **Test Results**

</div>