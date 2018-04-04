## Next.js Blog

Next requires almost zero-config. To set up a Next project from scratch, you just need to install Next and React:

```
yarn install next react react-dom
```

You set up the basic scripts for working with Next:

```javascript
  "scripts": {
    "start": "next start",
    "dev": "next",
    "build": "next build"
  }
```

You then create a pages folder, and in that, create an index.js file with some content:

```javascript
const index = ({ title = "hello world" }) => (
  <div>
    <h2>{title}</h2>
  </div>
);

export default index;
```
Since Next.js detects that you are using React, it doesn't even need to be imported at the top of the file. 

You then run:

```
yarn run dev
```

You should see in the terminal:

```terminal
> Ready on http://localhost:3000
> Building page: /
```

And that's it! You should see your 'hello world' in the browser