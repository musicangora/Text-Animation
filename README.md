# Text Animation

## 🔨 作ったもの

Vannila JS と CSS で文字のエフェクトを作成

## ✊ ポイント

```JS
const text = document.querySelector(".fancy");
const strText = text.textContent;
const splitText = strText.split("");
text.textContent = "";

for (let i = 0; i < splitText.length; i++) {
  text.innerHTML += "<span>" + splitText[i] + "</span>";
}
```

文字を一つ一つ分割して`<span>`をつけて

```JS
function onTick() {
  const span = text.querySelectorAll("span")[char];
  span.classList.add("fade");
  char++;
  if (char === splitText.length) {
    complete();
    return;
  }
}
```

`setInterval()`で各文字に class を付与する

## 👍 学んだこと

- 自分で分割しなくても JS には`split()`がある

## 🔗 参考

[![](https://img.youtube.com/vi/GUEB9FogoP8/0.jpg)](https://www.youtube.com/watch?v=GUEB9FogoP8)

[Youtube](https://www.youtube.com/watch?v=GUEB9FogoP8)
