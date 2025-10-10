### My solution
[Play the challenge](https://cssbattle.dev/play/hTcOgzNi1XUkGiJVQFXG)

### My solution

***100% match, 288 characters***
```html
<style>*{&::before,&::after{content:'';position:absolute;width:80;height:var(--n,80);background:var(--m,#F0CD48);top:60;left:240;}&::after{--n:60;--m:#5AA4B7;clip-path:polygon(0 0,75%50%,0 100%);}border:var(--b,solid)60px#243D83;margin:60 80;width: 120;height:60;*{background:#F0CD48;--b:
```

![alt text](./img/9th.png)

#### Explanation:
- Make sure you [understand the CSSBattle environment](https://github.com/bugb/css-battle/tree/main)
- The ungolfed version looks like this:

```html
<style>  
  * {
    &::before,
    &::after {
      content:'';
      position: absolute;
      width: 80px;
      height: var(--n, 80px);
      background:var(--m, #F0CD48);
      top: 60px;
      left: 240px;
    }
    &::after{
      --n: 60px;
      --m: #5AA4B7;
      clip-path: polygon(0 0, 75%50%, 0 100%);
    }
    border: var(--b,solid) 60px #243D83;
    margin: 60 80;
    width: 120px;
    height: 60px;
    * {
      background: #F0CD48;
      --b: none;
    }
  }
</style>
```

#### Syntax Overview

- We use [CSS nesting with the `var` function](../../README.md#css-nesting-with-the-var-function) and  [the `&` selector](../../README.md#the--selector)

#### Step-by-Step Breakdown
##### 1. Create a border for the `html` element and set a background color for the `body`.
```css
<style>
  * {
    border: var(--b,solid) 60px #243D83;
    margin: 60 80;
    width: 120px;
    height: 60px;
    * {
      background: #F0CD48;
      --b: none;
    }
  }
</style>
```
- I first adjusted the border size along with the margin to match the portion of the output.

- Then, I set the width and height to match the output border.

- a small tip: `--b: none` is the same as `--b:`
![alt text](./img/9-1.png)

Steps 2 and 3 use [Tree-Abiding pseudo-elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements#tree-abiding_pseudo-elements) so there's no need to add new elements to the DOM.

##### 2. Add a square element as an overlay above the HTML border
```diff
<style>  
+  * {
+    &::before,
+    &::after {
+      content:'';
+      position: absolute;
+      width: 80px;
+      height: var(--n,80px);
+      background:var(--m,#F0CD48);
+      top: 60px;
+      left: 240px;
+    }
    border: var(--b,solid) 60px #243D83;
    margin: 60 80;
    width: 120px;
    height: 60px;
    * {
      background: #F0CD48;
      --b: none;
    }
  }
</style>
```
![alt text](./img/9-2.png)


##### 3. Add the triangle
There will have many ways but I use: `clip-path: polygon(0 0, 75%50%, 0 100%);`

```diff
<style>  
  * {
    &::before,
    &::after {
      content:'';
      position: absolute;
      width: 80px;
      height: var(--n,80px);
      background:var(--m,#F0CD48);
      top: 60px;
      left: 240px;
    }
+    &::after{
+      --n: 60px;
+      --m: #5AA4B7;
+      clip-path: polygon(0 0, 75%50%, 0 100%);
+    }
    border: var(--b,solid) 60px #243D83;
    margin: 60 80;
    width: 120px;
    height: 60px;
    * {
      background: #F0CD48;
      --b: none;
    }
  }
</style>
```

![alt text](./img/9-3.png)

### Top 10 solutions (maximum 170 characters):
#### 1. [PINPAL](https://cssbattle.dev/player/pinpal)
```html
<style>*{background:#050044;border:solid+5ic#D62E65;border-radius:7lh/8pc;margin:34%56;*{corner-shape:notch;margin:-128-168-9in;font:6px/4'
```
#### 2. [H_Bliertz](https://cssbattle.dev/player/h_blierzt)
```html
<stylE>*{background:#050044;border-radius:21pc/21em;border:solid 5em#D62E65;margin:34%56;*{corner-shape:notch;margin:-128-336-800;font:38%'
```
#### 3. [James Whitehead](https://cssbattle.dev/player/wi328v9RQHXQ73SxzWKIKa6m6jg1)
```html
<style>*{background:#050044;border:solid 5em#D62E65;border-radius:7lh/8pc;margin:34%56;*{corner-shape:notch;margin:-128-168-250;font:6px/4'
```

#### 4. [Beo](https://cssbattle.dev/player/beo)
```html
<style>*{margin:34%56;border-radius:7lh/8pc;background:#050044;border:solid+5em#D62E65;*{margin:-128-612-300;corner-shape:notch;font:38%/14.39'
```

#### 5. [emohdaziz](https://cssbattle.dev/player/emohdaziz)
```html
<p>.<stYle>*{background:#050044;border:5em solid#d62e65}&{border-radius:5pc;margin:34%56;*{border-bottom:0;margin:0-185;*{margin:-36%155}font:2vh/8pc"
```

#### 6. [Veit Lehmann](https://cssbattle.dev/player/levito)
```html
<hr size=130><style>*{border:5em solid#D62E65;background:#050044}&{margin:34%56;border-radius:1in;*{margin:0-174;border-width:30 30 0;*{margin:-38%144
```

#### 7. [Ludvig](https://cssbattle.dev/player/ludvig)
```html
<hr size=130><STYLE>&{border-radius:5pc}*{background:#050044;margin:34%56;border:5em solid#D62E65;*{margin:0-166;border-width:30 30 0;*{margin:-158 136
```

#### 8. [David Eguiluz](https://cssbattle.dev/player/eguiluz)
```html
.....<a>. .......<style>&{border-radius:5pc;color:d62e65;border:5pc solid;margin:34%56;*{margin:-11-155;background:#050044;a{outline:32Q solid}font:17pc/8pc"
```

#### 9. [KoenH](https://cssbattle.dev/player/koenh)
```html
<p><style>&{border-radius:5em}*{background:#050044;border:var(--b,5em)solid#D62E65;margin:34%56;*{--b:32q;margin:0-200;height:8em;*{margin:-158 170;border-bottom:0
```

#### 10. [Martijn](https://cssbattle.dev/player/f9KZ3V3bdfaQx0oOfxY5VYVvLGW2)
```html
<p><style>*{background:#050044;border:var(--w,5pc)solid#D62E65;margin:136 56;border-radius:5em;*{margin:0-250;height:128;--w:32q;border-bottom:0;*{margin:-158 220;font:0'
```