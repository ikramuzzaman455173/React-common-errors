<h3 align="center">Simple Common Errors In React 😀</h3>

> Uncaught SyntaxError: The requested module '/src/app.js?t=1679635880304' does not provide an export named 'App' 

![typererror](https://user-images.githubusercontent.com/106922916/227433620-92f7168d-3eaa-41f3-8eb6-7d9ff5b52087.png)

### Your Main Code Is:)

```jsx
import React from 'react';

const App = () => {
  return (
    <div>
      <h3>Hello Developer</h3>
    </div>
  );
};

export default App
```

`
(export default App) Main Problem Code
`

### Solve Code:)

```jsx
import React from 'react';

export const App = () => {
  return (
    <div>
      <h3>Hello Developer</h3>
    </div>
  );
};
```
> Main Difference Is:)

`👉export👈 const App = () => {}`
