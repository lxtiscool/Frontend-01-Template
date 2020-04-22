# 本周作业

## 写一个正则表达式 匹配所有 Number 直接量

```js
/^-?\d+$|^(-?\d+)(\.\d+)?$|^0[bB][01]+$|^0[oO][0-7]+$|^0[xX][0-9a-fA-F]+$/g;```

## 写一个 UTF-8 Encoding 的函数

```js
function encodingStr(str){
  return str.split('').map((s) => `\\u${s.codepointAt().tostring()}`)
}
```

## 写一个正则表达式，匹配所有的字符串直接量，单引号和双引号

```js
/[\u0021-\u007E]{6,16}|[\x21-\x7E]{6,16}|(['"])(?:(?!\1).)*?\1/g;
```

