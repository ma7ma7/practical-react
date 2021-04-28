# React Icons

```javascript
$npm i react-icons --save
```

Example how to use the library with distributed value

```javascript
import React from "react";
import { RiReactjsFill } from "react-icons/ri";
import { RiAngularjsFill } from "react-icons/ri";
import { RiVuejsFill } from "react-icons/ri";
import { IconContext } from "react-icons";

function ReactIcons() {
  return (
    <div>
      <h2>React Icons</h2>
      <IconContext.Provider value={{ size: "5rem" }}>
        <RiReactjsFill color="blue" />
        <RiAngularjsFill color="red" />
        <RiVuejsFill color="green" />
      </IconContext.Provider>
    </div>
  );
}

export default ReactIcons;
```
