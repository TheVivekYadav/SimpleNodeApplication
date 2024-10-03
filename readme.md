# Node.js with Express - Installation and Simple Programs

## 1. Installation and Project Creation

### Step 1: Install Node.js
- [ ] Download and install Node.js from [nodejs.org](https://nodejs.org/)
- [ ] Verify installation by running `node -v` and `npm -v` in your terminal

### Step 2: Create a new project
- [ ] Open your terminal
- [ ] Create a new directory: `mkdir express-demo`
- [ ] Navigate to the directory: `cd express-demo`
- [ ] Initialize a new Node.js project: `npm init -y`

### Step 3: Install Express
- [ ] Install Express in your project: `npm install express`

## 2. Simple "Hello World" Program

### Step 1: Create app.js
- [ ] Create a new file named `app.js` in your project directory
- [ ] Open `app.js` in your text editor

### Step 2: Write the "Hello World" code
- [ ] Add the following code to `app.js`:

```javascript
const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Hello World');
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
    console.log(`Server is running on port ${PORT}`);
});
```

### Step 3: Run the server
- [ ] Start the server: `node app.js`
- [ ] Open your browser and navigate to `http://localhost:3000`
- [ ] You should see "Hello World" displayed in your browser

### step4: using package.json
- [ ] Open `package.json` in your text editor
- [ ] Add the following code to `package.json`:

```json
{
    "name": "express-demo",
    "version": "1.0.0",
    "scripts": {
        "start": "node app.js"
    }
}
```

### Step 5: Run the server
- [ ] Start the server: `npm start`
- [ ] Open your browser and navigate to `http://localhost:3000`
- [ ] You should see "Hello World" displayed in your browser

