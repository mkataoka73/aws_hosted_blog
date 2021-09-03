---
layout: post
title: GASの暗黙の型変換調べ
date: 2021-03-14 01:58 +0900
not_to_list: true
---
## きっかけ
GASの中級講座で、`if()`のカッコの中にはいるものは暗黙の型変換で`Boolean`になるよんという話をした。たとえば、

```js
if (123) {
  // here will be executed
}
```
ということ。

同様に、

```js
if ("foo") {
  // this also will be executed
}
```

である。

これ、やりだすと当然、「空文字はどうなるんだろう？」とか気になります、よね？

ということで、調べました。

##### test_stringsInBooleanContext.gs
```js
function test_string_in_boolean_context() {
  const str = "this is a string";
  console.log(Boolean(str)); // true
}

function test_empty_string_in_boolean_context() {
  const str = "";
  console.log(Boolean(str)); // false
}

function test_literal_space_in_boolean_context() {
  const str = "   ";
  console.log(Boolean(str)); // true(!!)
}

function test_tab_character_in_boolean_context() {
  const str = "\t";
  console.log(Boolean(str)); // true(!)
}

function test_newline_character_in_boolean_context() {
  const str = "\n";
  console.log(Boolean(str)); // true
}
```

満足。
