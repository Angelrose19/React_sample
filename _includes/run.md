# Run the React Application
Now you are ready to run your first real React application!

Run this command to move to the myfirstreact directory:
```text
C:\Users\Your Name>cd myfirstreact
```

Run this command to run the React application myfirstreact:
```text
C:\Users\Your Name\myfirstreact>npm start
```

A new browser window will pop up with your newly created React App! If not, open your browser and type localhost:3000 in the address bar.

The result :
![](assets/run.png)

# Modify the React Application
How do I change the content?

Look in the myfirstreact directory, and you will find a src folder. Inside the src folder there is a file called App.js, open it and it will look like this:

/myfirstreact/src/App.js:
```javascript
import React, { Component } from 'react';
import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div className="App">
        <header className="App-header">
          <img src={logo} className="App-logo" alt="logo" />
          <p>
            Edit <code>src/App.js</code> and save to reload.
          </p>
          <a
            className="App-link"
            href="https://reactjs.org"
            target="_blank"
            rel="noopener noreferrer"
          >
            Learn React
          </a>
        </header>
      </div>
    );
  }
}

export default App;
```
Try changing the HTML content and save the file.

Notice that the changes are visible immediately after you save the file, you do not have to reload the browser!

Example
Replace all the content inside the <div className="App"> with a <h1> element.

See the changes in the browser when you click Save.

```javascript
import React, { Component } from 'react';

class App extends Component {
  render() {
    return (
      <div className="App">
        <h1>Hello World!</h1>
      </div>
    );
  }
}

export default App;
```
