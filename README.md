# Layout_FinalHW
## 問題總集
**1. 在 banner 區塊，要將 logo 圖和 文字的高度切齊不太容易，
需要刻意的手動將高度拉齊。**
<img src="assets/images/README/banner.png" width="400"/>

**2. 客製化 class 和 直接寫在 css 裡面的抉擇?** <br/>
假設專案裡面以下這個對 img 設定的組合，寫了超過 3 以上，我決定把它改成一個共用的 class:

```
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```
**兩種客製化的流派**
1. atomic css
```
.object-cover {
  object-fit: cover;
}
.w-full {
  width: 100%;
}
.h-full {
  height: 100%;
}
```
2. components
```
.img-cover {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```
會如何抉擇呢?
