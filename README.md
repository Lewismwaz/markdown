# MARKDOWN TEXT CHEAT SHEET

Here are the main concepts needed to get started documenting your ideas using Markdown Language.

---

## 1. Blank Lines & Headings
- Add a blank line between content/text blocks. Use hashes (`#`) for headings:

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

## 2. Line Breaks
- Press Space twice, then Enter to force a line break without starting a new paragraph:

```markdown
This is the first line.  
And this is the second line.
```

### Comments
Use double %% to enclose text/content:

```markdown
%%This is a comment and won't be rendered%%
```

### Code Phrases
- Use double tick marks (`) to enclose inline code:

```markdown
This is a `code phrase`.
```

### Emphasis
- Italicized text — use single asterisk (*): *italic*

- Bold text — use double asterisk (**): **bold**

- Bold and Italicized — use triple asterisk (***): ***bold italic***

### Strikethrough
- Use double tildes (~~) to enclose content:

```markdown
~~I take back what I said~~
```

### Highlighting
- Use double equals (==) to enclose content, or the <mark> HTML tag:

```markdown
==Highlighted text==
<mark>Highlighted text</mark>
```

 ### Emojis
- Use a colon : followed by the emoji name:

```markdown
I love programming! :star: :computer:
```

For more emojis, check out: [rxaviers Emojis](https://github.com/rxaviers/emoji-cheat-sheet)

### Blockquotes
- Use > in front of a paragraph:

```markdown
> James was arrested for collecting a lost wallet from a boggy man.
```

### Blockquotes with Multiple Paragraphs
- Add > on the blank lines between paragraphs:

```markdown
> Am loving this markdown lesson.
>
> And this one is about blockquotes with multiple paragraphs.
```

### Nested Blockquotes
- Add > in front of the paragraph you want to nest:

```markdown
> You want to know something funny.
>
>> This is a nested paragraph; a paragraph inside another paragraph.
```


### Blockquotes with Other Elements
```markdown
> The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> 1. Everything's great but am not okay with that.
> 2. What do I do about that?
```

## Lists
### (i) Ordered Lists
- Add line items with numbers followed by periods:

```markdown
1. This is item number 1
2. Item number 2
3. Item number 3
Nesting List Items
Indent items 1 tab or 4 spaces:
```

```markdown
Components of a Computer:
1. Software
    1. Application software
    2. System software
2. Data
3. Hardware
    1. Monitor
    2. Central Processing Unit (CPU)
    3. Mouse/Touchpad
    4. Motherboard
    5. Speakers
    6. Network Interface Card (NIC)
```


### (ii) Unordered Lists
- Add dashes (-), asterisks (*), or plus signs (+) in front of line items:

```markdown
- James was not paid after working for Mr. Wotman.
- I don't know why I am so broke yet money flows by my hands every single day.
- I would like to visit Kentucky one day.
- My name is not Samuel.
- Don't judge someone you don't know quite well.
```


### Nesting List Elements
- Indent the items one tab or four spaces:

```markdown
- This is the first item
- Second item
- Third item
    - Third sub-item 1
    - Third sub-item 2
    - Third sub-item 3
        - Third sub-item 3: sub-item 1
        - Third sub-item 3: sub-item 2
        - Third sub-item 3: sub-item 3
```

## Images
- Standard Markdown image syntax:

```markdown
![Alt text](path/to/image.png)
```

### Centered & Resized Images (HTML trick)
- Use HTML <p> and <img> tags to center and resize images. This is how you can control dimensions (width, height) and alignment:

```html
<p align="center">
    <img src="images/logo.png" width="80" alt="Diary-AI Logo">
</p>
```

### Centered Heading
```html
<h2 align="center">Diary AI</h2>
```

> [!TIP]
> You can combine align="center", width, and height attributes to control layout inside your README or docs. HTML tags work alongside Markdown.

### Image with a Caption (using HTML)
```html
<p align="center">
    <img src="images/google-oauth.png" width="496" alt="Configure Google OAuth"><br>
    <em>Configure Google OAuth</em>
</p>
```


## Horizontal Rules
- Use 3+ asterisks (***), dashes (---), or underscores (___) on a line by themselves:

```markdown
***
```

## Links & Titles
- Enclose the link text in brackets [Link Text] and follow immediately with the URL in parentheses (URL):

```markdown
[EAppoint Master](https://eappointmaster.com)
Visit Github today to review our services.
```

### Reference-style Links
```markdown
[Diary AI][1]

[1]: https://github.com/Lewismwaz/Diary-AI
```

### URLs and Email Addresses
- To quickly turn a URL or email address into a link, enclose it in angle brackets:

```markdown
<https://github.com>
<eappointmaster@gmail.com>
```

## Code Blocks
### 1. With Syntax Highlighting
- Use 3 tildes (~~~) followed by the name of the language, and close with 3 tildes:

```markdown
```python
def logout_user(request):
    logout(request)
    if request.user.is_authenticated:
        request.user.set_last_logout()  # Update last logout time
    messages.success(request, 'Logout successful!')
    return redirect('login')```
```

### 2. Fenced Code Block (No Syntax Highlighting)
- Use 3 tildes to enclose content:

```markdown
```{ "firstName": "James", "lastName": "Bennet", "age": 25 }```
```


## Alerts
- Use GitHub-flavored alert syntax (> [!TYPE]):

```markdown
> [!NOTE]
> Useful information that ought to be known.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information needed to achieve something.

> [!WARNING]
> Urgent information that needs immediate attention to avoid problems.

> [!CAUTION]
> Warns about risks or negative outcomes of specific actions.
```

> [!NOTE]
> Useful information that ought to be known.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information needed to achieve something.

> [!WARNING]
> Urgent information that needs immediate attention to avoid problems.

> [!CAUTION]
> Warns about risks or negative outcomes of specific actions.


## Tables
- Use 3 or more hyphens (---) to create each column header, and pipes (|) to separate each column:
```markdown
| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
```

### Syntax	Description
Header	Title
Paragraph	Text
Table Alignment

- Align text in columns to the left, right, or center by adding a colon (:) to the left, right, or both sides of the hyphens within the header row:

Left Alignment: :---

Right Alignment: ---:

Center Alignment: :---:


| Left      | Center    | Right     |
| :-------- | :-------: | --------: |
| Header    | Title     | Text      |
| Paragraph | Text      | Text      |


Left	Center	Right
Header	Title	Text
Paragraph	Text	Text


## Task List
- Use - [x] or - [ ] to create checkable to-do items:

```markdown
- [x] Monday
- [ ] Tuesday
- [ ] Wednesday
- [ ] Thursday
- [ ] Friday
- [ ] Saturday
- [ ] Sunday
```

☑ Monday
□ Tuesday
□ Wednesday
□ Thursday
□ Friday
□ Saturday
□ Sunday


## Footnotes
- Add footnotes for additional information or references:

```markdown
Here is a footnote reference[^1].

[^1]: Refer to footnote.
Here is a footnote reference[^1].

[^1]: Refer to footnote.
```

## Math Blocks
### Basic Math
23 + 2 = 25


### Fractions
- Use `\frac{numerator}{denominator}`:

- `$\frac{1}{4}$` for $\frac{1}{4}$


### Powers / Superscripts
- Use `$number^{power}$ or number<sup>power</sup>`:

- '$3^{x}$` + `3<sup>y</sup>` for $3^{x}$ + 3<sup>y</sup>


### Subscripts
- Use `$number_{character}$` or `number<sub>character</sub>`:

- `$\log_{2}16 = 4$` for $\log_{2}16 = 4$  and  `log<sub>2</sub>16 = 4` for log<sub>2</sub>16 = 4


### Square Root
- Use `\sqrt{number}`:

- `$\sqrt{10}$` for $\sqrt{10}$


### Higher Order Roots
- Use `\sqrt[root]{number}`:
  
- `$\sqrt[3]{10}$` for $\sqrt[3]{10}$
​
 
### Recurring Decimals / Overlines
- Use `\overline{number/character}`:

- `$2.\overline{3}$` for $2.\overline{3}$
 

### Plus or Minus
Use `\pm`:

- `$\sqrt[4]{16} = \pm 2$` for $\sqrt[4]{16} = \pm 2$


### Quadratic Formula
- `$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$` for $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$


### Practical Example
Given the linear equations below, find the exact values for p, x, m, and y: (6 Marks)

![Practical example](example.png)

### Markdown
```markdown
## Solution
- Let's use $x$ as the subject in the first equation:

$$
3x = 33 - 4p
$$

$$
x = 11 - \frac{4p}{3}
$$

Substitute $x$ into equation (ii):

$$
5p - 6\left(11 - \frac{4p}{3}\right) = 2
$$

Hence,

$$
5p - 66 + 8p = 2
$$

Collect like terms together:

$$
\rightarrow 5p + 8p = 2 + 66
$$

$$
\therefore 13p = 68
$$

$$
p = \frac{68}{13} = 5\frac{3}{13}
$$

$$
x = 11 - \frac{4\left(5\frac{3}{13}\right)}{3}
$$

$$
x = 11 - \left(4 \cdot \frac{68}{13}\right)\left(\frac{1}{3}\right)
$$

$$
\therefore x = 11 - \frac{272}{39} = \frac{157}{39}
$$

$$
\rightarrow m = 13\left(\frac{68}{13}\right)^2 - \frac{13}{3}\left(\frac{157}{39}\right)^2
$$

$$
\therefore m = 13\left[\left(\frac{68}{13}\right)^2 - \frac{1}{3}\left(\frac{157}{39}\right)^2\right]
$$

$$
m = 285\frac{164}{351}
$$

Simplify:

$$
\frac{y}{m - (p + x)} = 351,
$$

$$
y = 351\left[m - (p + x)\right]
$$

$$
y = 351\left[285\frac{164}{351} - \left(5\frac{3}{13} + 4\frac{1}{39}\right)\right]
$$

$$
\therefore y = 351\left(285\frac{164}{351} - 9\frac{10}{39}\right)
$$

$$
y = 351\left(130\frac{100}{117}\right)
$$

$$
y = 351\left(\frac{15,310}{117}\right)
$$

$$
y = 45,930
$$
```

## Solution
- Let's use $x$ as the subject in the first equation:

$$
3x = 33 - 4p
$$

$$
x = 11 - \frac{4p}{3}
$$

Substitute $x$ into equation (ii):

$$
5p - 6\left(11 - \frac{4p}{3}\right) = 2
$$

Hence,

$$
5p - 66 + 8p = 2
$$

Collect like terms together:

$$
\rightarrow 5p + 8p = 2 + 66
$$

$$
\therefore 13p = 68
$$

$$
p = \frac{68}{13} = 5\frac{3}{13}
$$

$$
x = 11 - \frac{4\left(5\frac{3}{13}\right)}{3}
$$

$$
x = 11 - \left(4 \cdot \frac{68}{13}\right)\left(\frac{1}{3}\right)
$$

$$
\therefore x = 11 - \frac{272}{39} = \frac{157}{39}
$$

$$
\rightarrow m = 13\left(\frac{68}{13}\right)^2 - \frac{13}{3}\left(\frac{157}{39}\right)^2
$$

$$
\therefore m = 13\left[\left(\frac{68}{13}\right)^2 - \frac{1}{3}\left(\frac{157}{39}\right)^2\right]
$$

$$
m = 285\frac{164}{351}
$$

Simplify:

$$
\frac{y}{m - (p + x)} = 351,
$$

$$
y = 351\left[m - (p + x)\right]
$$

$$
y = 351\left[285\frac{164}{351} - \left(5\frac{3}{13} + 4\frac{1}{39}\right)\right]
$$

$$
\therefore y = 351\left(285\frac{164}{351} - 9\frac{10}{39}\right)
$$

$$
y = 351\left(130\frac{100}{117}\right)
$$

$$
y = 351\left(\frac{15,310}{117}\right)
$$

$$
y = 45,930
$$


# Extra Tricks
## Badges
- Use shields.io or similar to generate badges:


![License](https://img.shields.io/badge/license-GPL-blue)
![Version](https://img.shields.io/badge/version-0.1.0-green)
https://img.shields.io/badge/license-GPL-blue
https://img.shields.io/badge/version-0.1.0-green

# Table of Contents with Anchor Links
## Contents
- [Features](#features)
- [System Demo](#system-demo)
- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [License](#license)


## Collapsible Sections (HTML `<details>`)
Wrap long content in a collapsible block:

```html
<details>
<summary>Click to expand</summary>

Hidden content goes here.

</details>
<details> <summary>Click to expand</summary>
Hidden content goes here.

</details>
```

## Keyboard Shortcuts
- Use `<kbd>` tags:
```markdown
Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.
```

Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.

### Directory Tree with text Code Block
- Use a text fenced block with tree-like characters:

```text
.
├── app/
├── components/
├── lib/
├── prisma/
│   ├── migrations/
│   └── schema.prisma
└── package.json
```

## Inline HTML for Line Breaks / Spacing
```html
<br>
Use <br> for line breaks inside paragraphs and tables, or to add spacing.
```


## Escaping Markdown Characters
- Use backslash \ to escape special characters:

\*Not italic\*  \_Not underlined\_  \# Not a heading
*Not italic* _Not underlined_ # Not a heading
