English | [简体中文](https://github.com/NotYoojun/Pangulas/blob/main/README.zh-cn.md)

# Pangulas CJK Text Formatting Guidelines

Pangulas is a set of formatting standards that ensures optimal reading experience when mixing Chinese text with Western characters. It is similar to [Pangu Spacing](https://github.com/vinta/pangu.js), but more rigorous and standardized. You can think of Pangulas as an upgraded version of Pangu Spacing.

> **From [Pangu.js](https://github.com/vinta/pangu.js?tab=readme-ov-file#%E7%82%BA%E4%BB%80%E9%BA%BC%E4%BD%A0%E5%80%91%E5%B0%B1%E6%98%AF%E4%B8%8D%E8%83%BD%E5%8A%A0%E5%80%8B%E7%A9%BA%E6%A0%BC%E5%91%A2):**
> If you’re like me and feel uneasy every time you see Chinese characters, English, numbers, and symbols squeezed together on a webpage, and can’t resist adding a space between them, then this extension (supported by Chrome and Firefox) is exactly what you need for navigating the online world. It automatically inserts spaces between all Chinese characters and half-width English, numbers, and symbols on the page.
>
> Sinologists call this space “Pangu’s white,” as it splits the chaos between full-width and half-width characters. Research also shows that people who don’t like to add spaces between Chinese and English while typing tend to have tough love lives, with 70% of them marrying someone they don’t love by the age of 34, while the remaining 30% end up leaving their inheritance to their cats. After all, both love and writing require leaving space at the right time.


## Rule Content

### Add a space between CJK and Latin characters

Between CJK (Chinese, Japanese, Korean) characters and other characters, such as letters, numbers, punctuation marks, etc., a space should be added. For example, the following text demonstrates the effect before and after applying this rule:

```csharp
中文English => 中文 English
你好，我是Walt，我喜歡使用emacs。=> 你好，我是 Walt，我喜歡使用 emacs。
```

The table below summarizes when to use spaces. Of course, this rule is only a reference, and rules such as hyperlink spaces are subject to debate, depending on the habits.

| Combination      | Rule    | Example
| ---------------- | ------- | ----
| Chinese and English | Space required | 我使用 Google 搜索引擎
| Chinese and numbers | Space required | 今天 20 摄氏度
| English and numbers | Space required | 最近更新了 iOS 13.5 版本的系统
| Numbers and units | Space required | 香蕉 1.99 美元一磅
| Numbers and percentages | No space required | 谷歌浏览器市场占比高达 58.4% 了
| Date | No space required | 今天是 2020 年 1 月 1 日
| Full-width punctuation and characters | No space required | 喂！你在干什么？！
| Ellipsis | No space required | 这...有问题吗

### Always use English brackets and quotation marks

Regardless of the language, English brackets and quotation marks should be used, following the specified spacing rules below.

- Chinese brackets and quotation marks (prohibited): `（）【】 “” ‘’ `

- Instead, use English brackets and quotation marks: ` () [] "" '' `

When using English brackets and quotation marks, a space should be added outside the brackets and quotation marks, and no space should be added inside them:

- Spaces for ` ( [ ` should be added on the left side, and spaces for ` ) ] ` should be added on the right side

- Spaces for ` " ' ` should be added outside the content being wrapped (since English quotes cannot distinguish between opening and closing, the author needs to judge for themselves)

In some cases, `【】` and `「」` are allowed, and no spaces should be added before or after them.

If this description is not clear enough, you can refer to the examples below. First, replace all Chinese brackets and quotation marks with English brackets and quotation marks:

```csharp
中文括号（啊是的）没错的“啊是的”对对对 => 中文括号(啊是的)没错的"啊是的"对对对
```

Next, add spaces outside the brackets and quotation marks:

```csharp
中文括号(啊是的)没错的"啊是的"对对对 => 中文括号 (啊是的) 没错的 "啊是的" 对对对
```

Except for parentheses and quotation marks, other punctuation marks should use Chinese punctuation (`，。、；：？！`) in Chinese text and English punctuation (`,.:;?!`) in English text.

### Some Chinese punctuation marks should not have spaces

Some Chinese punctuation marks should not have spaces around them. For example, the ellipsis (`……`) should not have spaces around it. Here are some examples:

```csharp
你好， Walt 是我， 我喜歡使用 emacs。=> 你好，Walt 是我，我喜歡使用 emacs。
```

### Do not use a single ellipsis

In Chinese text, a single ellipsis symbol `…` should not be used. Instead, use three dots `...` to form an ellipsis. There should be no space before the ellipsis; if the ellipsis is at the end of a sentence, a space should be added after it. If the text after the ellipsis is still part of the current sentence, no space should be added. For example:

```csharp
这...有问题吗？ => 这...有问题吗？
今天买了好多东西：苹果、葡萄、橙子...啊，橙子最好吃。=> 今天买了好多东西：苹果、葡萄、橙子... 啊，橙子最好吃。
```

### Do not add spaces around some Chinese punctuation marks

When encountering Chinese punctuation marks such as commas, pauses, periods, semicolons, colons, exclamation marks, and question marks, no spaces should be added before or after them, even if they are followed by English characters. For example:

```csharp
你好， Walt 是我， 我喜歡使用 emacs。=> 你好，Walt 是我，我喜歡使用 emacs。
```

### Contributon welcomed

This is a guideline I hastily drafted. If you have better suggestions, or if you find any flaws or errors, feel free to submit a PR or an Issue.

Attribution - NonCommercial - NoDerivatives 3.0 Unported (CC BY-NC-ND 3.0)