# Markdown (마크다운)
Markdown Documentation (마크다운 문서)

[Tutorial](https://github.com/kctzstyle/markdown-tutorial/blob/main/Tutorial.md)

---

# Header (헤더)
```
해시태그 `#`는 html에서의 `h1` 태그 역할과 같으며,
html에서 `h1` ~ `h6` 까지 존재하는데, `#` 역시 6개까지 가능합니다.
```

## Example
```
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

# h1
## h2
### h3
#### h4
##### h5
###### h6
####### h7은 없습니다.

# Headline (헤드라인)
```
대시(Hyphen) 기호를 세번 `---` 이상 붙이면 html에서의 `hr` 태그 역할을 합니다.
하지만 `---` 위에 문장이 들어가면 `h1` 태그와 동일합니다.
`---` 뿐만 아니라 `- - -`, `* * *`, `***`, `===`, `= = =` 역시 가능합니다.
```

## Example
```
---

`---` 위에 문장이 들어가면 h1이 됩니다.
---
```

---

`---` 위에 문장이 들어가면 h1이 됩니다.
---

# List (목록)
## 순서 있는 리스트 만들기
```
html에서의 `ol` 태그(Ordered List) 안의 `li` 태그 역할을 합니다.
숫자와 점(Dot; `.`) 기호를 사용합니다.
```

### Example
```
1. 예시1
2. 예시2
3. 예시3
```

1. 예시1
2. 예시2
3. 예시3

## 순서가 필요없는 리스트 만들기
```
`-`, `+`, `*` 기호 뒤에 문장을 작성하면 `ul` 태그(Unordered List) 안의 `li` 태그 역할을 합니다.
공백(Space; 스페이스)이 2개가 추가될 때마다 상위 항목에 종속됩니다.
```

### Example
```
- 예시1
  - 예시1-1
  - 예시 1-2
- 예시2
  - 예시 2-1
  - 예시 2-2
    - 예시 2-2-1
    - 예시 2-2-2
    - 예시 2-2-3
- 예시3
  - 예시 3-1
  - 예시 3-2
  - 예시 3-3
```

- 예시1
  - 예시1-1
  - 예시 1-2
- 예시2
  - 예시 2-1
  - 예시 2-2
    - 예시 2-2-1
    - 예시 2-2-2
    - 예시 2-2-3
- 예시3
  - 예시 3-1
  - 예시 3-2
  - 예시 3-3

# Block Quote (인용문)
```
html에서의 `blockquote` 태그 역할과 동일하며 `>` 기호를 사용합니다.
`>` 기호가 추가될 때마다 상위 인용문에 종속됩니다.
```

## Example
```
> 인용문1
>> 인용문2
>>> 인용문3
>>>> 인용문4
...
> 인용문5
> 인용문6
>> 인용문7
>> 인용문8
>>> 인용문9
```

> 인용문1
>> 인용문2
>>> 인용문3
>>>> 인용문4

> 인용문5
> 인용문6
>> 인용문7
>> 인용문8
>>> 인용문9

# Code (코드 강조 문법)
```
html에서의 `code` 태그와 동일하며 ` 기호를 사용합니다.
```

### Example
```
`code` 강조 문법
```

`code` 강조 문법

## Block Code (블럭 코드 강조 문법)
````
html에서의 `pre` 태그와 동일하며 ` 기호를 3번 이상 사용합니다.
``` 옆에 프로그래밍 언어를 적으면 해당 언어의 코드 문법 강조로 변환되어 보여줍니다.
````

### Example
````

```
This is Code Block
이것은 코드 블럭 입니다.
```

```console
$ console
git clone https://github.com/kctzstyle/Markdown.git
```

```html
<html>
<body>
  <h1>Hello, Markdown!</h1>
</body>
</html>
```

```python
# Python
print('Hello, Markdown!')
```

````

```
This is Code Block
이것은 코드 블럭 입니다.
```

```console
$ console
git clone https://github.com/kctzstyle/Markdown.git
```

```html
<html>
<body>
  <h1>Hello, Markdown!</h1>
</body>
</html>
```

```python
# Python
print('Hello, Markdown!')
```

# Link (링크)
```
html에서의 `a` 태그 역할과 동일하며 `[문장](링크 "설명<옵션>")` 형식으로 사용합니다.
설명은 선택사항(옵션)이며, 추가하게 되면 마우스 커서를 올렸을 때 표시되는 문구입니다.
`a` 태그의 `title` 속성과 동일합니다.
```

## Example
```
[My GitHub](https://github.com/kctzstyle "나의 깃허브 프로필")
```

[My GitHub](https://github.com/kctzstyle "나의 깃허브 프로필")


# Image (이미지)
```
html에서의 `img` 태그 역할을 하며 `![문장](이미지 링크 "설명")` 형식으로 사용합니다.
설명은 선택사항이며, 위의 `Link (링크)`의 사용법과 동일합니다.
```

## Example
```
![My Avatar](https://avatars0.githubusercontent.com/u/77194159?s=460&u=adc2823db5e5045fc6efe12fbdf88d5669e313fb&v=4 "My Avatar")
```

![My Avatar](https://avatars0.githubusercontent.com/u/77194159?s=460&u=adc2823db5e5045fc6efe12fbdf88d5669e313fb&v=4 "My Avatar")

# 혼합해서 사용하기
```
html에서의 `img` 태그와 `a` 태그를 같이 사용하는 것과 동일합니다.
[![문장](이미지 링크)](링크) 형식을 사용합니다.
```

## Example
```
[![My Avatar](https://avatars0.githubusercontent.com/u/77194159?s=460&u=adc2823db5e5045fc6efe12fbdf88d5669e313fb&v=4)](https://github.com/kctzstyle)
```

[![My Avatar](https://avatars0.githubusercontent.com/u/77194159?s=460&u=adc2823db5e5045fc6efe12fbdf88d5669e313fb&v=4)](https://github.com/kctzstyle)

# Font (글꼴)
```
`*문장*` 혹은 `_문장_`, `**문장**` 혹은 `__문장__`, `~~문장~~`은
각각 html에서의 `i` 태그(italic; 기울임), `b` 태그(bold; 굵게), `s` 태그(specifies; 취소선)과 동일합니다.
```

## Example
```
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__

~~cancelline~~
```

*single asterisks*

_single underscores_

**double asterisks**

__double underscores__

~~cancelline~~

# Table (표)
```
html에서의 `table` 태그와 동일하며 다음과 같이 사용합니다.
| Column1 | Column2 |
| ------- | ------- |
| Row1    | Row1    |
| Row2    | Row2    |
...
```

## Example
```
| Column1 | Column2 |
| ------- | ------- |
| Row1    | Row1    |
| Row2    | Row2    |
```

| Column1 | Column2 |
| ------- | ------- |
| Row1    | Row1    |
| Row2    | Row2    |
