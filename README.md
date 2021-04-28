# React Toastify

## Installation

```javascript
npm install --save react-toastify
```

### Usage

```javascript
import { ToastContainer, toast } from "react-toastify";
// Toast container is like an globale object configuration file

import "react-toastify/dist/ReactToastify.css";

function App() {
  const notify = () => {
    toast("Default Notification 🚀");

    // Success
    toast.success("Success Notification ☑️", {
      position: toast.POSITION.TOP_CENTER,
      autoClose: 2000,
    });

    // Error
    toast.error("Error Notification ☀️", {
      position: toast.POSITION.TOP_LEFT,
    });

    // Warn
    toast.warn("Warnning Notification 🚨", {
      position: toast.POSITION.BOTTOM_LEFT,
    });

    // Warn
    toast.info("Info Notification 🎄", {
      position: toast.POSITION.BOTTOM_RIGHT,
    });

    toast("custom style", {
      position: toast.POSITION.BOTTOM_CENTER,
      className: "toast",
      autoClose: false,
    });
  };
  return (
    <div className="App">
      <button onClick={notify}>Toast</button>
      <ToastContainer />
    </div>
  );
}

export default App;
```
