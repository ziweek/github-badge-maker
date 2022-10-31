# github-badge-maker

<p align="center">
  <img src="https://img.shields.io/badge/Nest.js-E0234E?style=flat-square&logo=Nestjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Heroku-430098?style=flat-square&logo=Heroku&logoColor=white"/>
</p>

## Introduction

<p align="left">
  <img src="https://github-badge-maker.herokuapp.com/badge?logo=likelion&name=Likelion&color=232F3E"/>
  <img src="https://github-badge-maker.herokuapp.com/badge?logo=bada&name=bada&color=232F3E"/>
  <img src="https://github-badge-maker.herokuapp.com/badge?logo=gdsc&name=Kugods&color=232F3E"/>
  <img src="https://github-badge-maker.herokuapp.com/badge?logo=brightics&name=Brightician&color=232F3E"/>
</p>

This backent web service is prepared for badges which are not provided by `simpleicons.org`. Therefore, in this service, it is possible to make customized badge with special icon, text and color.

<br/>



## How to Use

1. Prepare query for `logo`, `name`, `color`.

|Query|DType|
|--|--|
|logo|string|
|name|string|
|color|string|

2. Complete below tag.
```markdown
<img src="https://github-badge-maker.herokuapp.com/badge?logo=likelion&name=Likelion&color=232F3E"/>
```
<br/>


## How to Add
1. Prepare `.svg` file.
2. Encode the `.svg` file into `base64`.
3. Put the encoded `base64` file in `src/badge/assets` folder.
4. Add script to read asset file.

```typescript
  switch(logo) {
            ...
            case 'queryName':
                var logoDir = `./src/badge/assets/fileName.txt`;
                break;
            ...
        }
```
<br/>

## Reference

|name|link|
|--|--|
|logo|https://base64.guru/converter/encode/image/svg|
|heroku|https://dashboard.heroku.com/apps|
|heroku kaffeine|https://kaffeine.herokuapp.com/|
|Heroku Guide|https://velog.io/@kimbiyam/Nest-JS-Heroku%EB%A1%9C-%EB%B0%B0%ED%8F%AC%ED%95%98%EA%B8%B0|
