# React Boilerplate to create libraries

This project contains all react components needed for your development. You can
build and distribute as npm package.

## Installing

To start using it just add this project as dependeny:

```bash
// packages.json
"dependencies": {
  "mylib-react-ui": "git@github.com:cristianoliveira/react-lib-boilerplate.git"
}
```

## Basic theme usage

To have all elements in the correct style you must wrap your app with the `MyLibTheme` component.
```javascript
// App.js
import MyLibTheme from 'mylib-react-ui';

const App = () => (
  <MyLibTheme>
    <MyPageComponent />
  </MyLibTheme>
);

ReactDOM.render(<App />, document.getElementById('app'));
```

Using the components
```javascript
// FooButton.js

import { Button } from 'mylib-react-ui';

const FooButton = () => {
  <div>
    <Button>Click</Button>
  </div>
}

export default FooButton;
```

## Live style guide and documentation

This project also has a live style guide and usage documentation :).
To install and run the Styleguidist server do:

```
npm install
npm run styleguide
```

Then open [http://localhost:6060](http://localhost:6060) in your browser. There you going to find all
components and examples of use.


## Tests

To run all tests execute:
```
npm run test
```

# Dependencies

This project includes:

  - Reactjs
  - Babel
  - Webpack 3.0
  - Postcss
  - Jest
  - Eslint
  - Styledist
