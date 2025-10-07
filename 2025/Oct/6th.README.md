### My solution

***100% match, 118 characters***
```html
<p><style>*{background:var(--m,#588A95);*{width:140;height:140;margin:20%auto;--m:#222;*{--m:#fff;transform:skew(45deg
```
![alt text](6th.png)

#### Explanation:
- Make sure you [understand the CSSBattle environment](./6th.README.md)
- The ungolfed version looks like this:

```html
<style>
* {
  background: var(--m, #588A95);
  * {
    width: 140px;
    height: 140px;
    margin: 20% auto;
    --m: #222;
    * {
      --m: #fff;
      transform: skew(45deg);
    }
  }
}
</style>
<p></p>
```

#### Syntax Overview

The syntax:
```css
* {
  * {
    * {
    }
  }
}
```
is called [CSS nesting](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_nesting/Using_CSS_nesting)

#### Step-by-Step Breakdown
1. First Level

```css
* { 
  background-color: var(--m, #588A95);
}
```
This styles the html, body, and p elements with a background color set to the variable --m, or #588A95 if --m is not defined.

2. Second Level
```css
* {
  width: 140px;
  height: 140px;
  margin: 20% auto;
  --m: #222;
}
```
At this level:

- The `width` and `height` of `body` and `p` are set to `140px`.

- The elements are centered horizontally with margin: `20% auto`.

- The variable `--m` is now defined as `#222`, which will be used as the background color for these elements.

3. Third Level
```css
* { 
  --m: #fff;
  transform: skew(45deg);
}
```
Finally:

The `--m` variable is updated to `#fff`, so the `p` element now has a white background.

The element is also transformed with a `45-degree` skew.

✅ Summary:
This nested structure allows each level of the cascade `(html → body → p)` to inherit and override the CSS variable `--m`, resulting in a layered color change and transformation effect.

### Top 10 solutions:
1. [Ilya Streltsyn](https://cssbattle.dev/player/selenit)
```html
<style>*{background:#588A95;color:#222;outline:solid 75q;margin:37.5%50%;*{color:fff;transform:skew(45deg
```
2. [emohdaziz](https://cssbattle.dev/player/emohdaziz)
```html
<stYle>&{background:#222;border:138Q solid#588a95;scale:1 3.5;*{background:#fff;margin:0;transform:skew(74deg
```

3. [Mister Magoo](https://cssbattle.dev/player/mistermagoo)
```html
<p><style>*{background:var(--b,#588A95)}&>*{margin:80 130;--b:#222}p{--b:#fff;height:140;transform:skew(45deg
```

4. [Seth Kuhn](https://cssbattle.dev/player/mrdeathray)
```html
<style>&{border:138q solid#588A95;background:#222;margin:-50 0;*{background:#fff;margin:0;transform:skew(45deg
```

5. [Ludvig](https://cssbattle.dev/player/ludvig)
```html
<STYLE>&{background:#222;margin:-50 0;border:138q solid#588A95;*{background:#FFF;margin:0;transform:skew(45deg
```

6. [H_Bliertz](https://cssbattle.dev/player/h_blierzt)
```html
<p><stylE>&{margin:142 192;*{background:#588A95;outline:solid 75q;color:#222;*{color:#FFF;transform:skew(45deg
```

7. [Martijn](https://cssbattle.dev/player/f9KZ3V3bdfaQx0oOfxY5VYVvLGW2)
```html
<style>&{background:#222;border:138q solid#588A95;margin:-50 0;*{background:#fff;margin:0;transform:skew(45deg
```

8. [David Eguiluz](https://cssbattle.dev/player/eguiluz)
```html
<style>&{background:#222;border:138q solid#588a95;margin:-50 0;*{background:#fff;margin:0;transform:skew(45deg
```

9. [Kieron](https://cssbattle.dev/player/kieron)
```html
<style>&{margin:-58-8;background:#222;border:46vh solid#588a95;*{margin:0;background:#fff;transform:skew(45deg
```

10. [Sascha Adams](https://cssbattle.dev/player/saschaadams)
```html
<stYle>&{background:#222;border:138q solid#588A95;margin:-50 0;*{margin:0;background:#fff;transform:skew(45deg
```