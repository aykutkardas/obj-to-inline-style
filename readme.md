# Object to Inline Style

## Install

```sh
npm install obj-to-inline-style
```

```sh
yarn add obj-to-inline-style
```

## Usage

```js
import objToInlineStyle from "obj-to-inline-style";
```

Example Object

```js
const style = {
  background: "#eee",
  padding: [3, 4, 10, 2],
  marginLeft: 10,
  marginRight: 10,
  marginBottom: 0,
  boxShadow: [1, 1, 3, 4, "black"]
};
```

And convert

```js
const inlineStyle = objToInlineStyle(style);

console.log(inlineStyle);

// "background:#eee;padding:3px 4px 10px 2px;margin-left:10px;margin-right:10px;margin-bottom:0;box-shadow:1px 1px 3px 4px black;"
```

---

## Trick

```js
const style = {
  boxShadow: [1, 1, 3, 4, "black"]
};
```

or

```js
const style = {
  boxShadow: "1px 1px 3px 4px black"
};
```
