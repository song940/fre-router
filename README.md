## fre-routes

> simple routes for fre

[![fre-routes](https://img.shields.io/npm/v/fre-routes.svg)](https://npmjs.org/fre-routes)

### Installation

```bash
$ npm install fre-routes
```

### Example

```js
import { h, render } from 'fre'
import { useRoutes, push } from 'fre-routes';

const routes = {
  '/': () => (
    <div>
      <p>home</p>
      <button onClick={() => push('/home/jack')}>Go jack</button>
    </div>
  ),
  '/home/:id': ({ id }) => (
    <div>
      <p>{id}</p>
      <button onClick={() => push('/')}>Go home</button>
    </div>
  ),
}

const App = () => useRoutes(routes)

render(<App />, document.getElementById('root'))
```

### Contributing
- Fork this Repo first
- Clone your Repo
- Install dependencies by `$ npm install`
- Checkout a feature branch
- Feel free to add your features
- Make sure your features are fully tested
- Publish your local branch, Open a pull request
- Enjoy hacking <3

### MIT

This work is licensed under the [MIT license](./LICENSE).

---