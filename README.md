# 아이패드 반응형 데스크탑 모드

[참고자료 - 깃헙](https://github.com/ParkYoungWoong/apple-ipad-app)

## 오픈 그래프 & 트위터 카드

- 오픈 그래프 url `og:url`은 사이트 주소가 아니라 페이지 주소를 입력해야함

## reset css

[reset.css jsdelivr](https://www.jsdelivr.com/package/npm/reset-css)

## 구글 폰트

[폰트.구글.com](https://fonts.google.com/)
[Roboto(영문)](https://fonts.google.com/specimen/Roboto)
[Noto Sans Korean(한글)](https://fonts.google.com/noto/specimen/Noto+Sans+KR)

기본적으로 Roboto를 적용하고 적용이 되지 못하는 한글은 다음 폰트인 Noto Sans를 적용

```CSS
font-family: "Roboto", "Noto Sans KR", sans-serif;
```

## CSS 속성

### word- break 속성

단어 단위로 줄바꿈 처리를 결정하는 속성

- 기본적으로 영문은 단어 단위로 줄바꿈이 일어남
- 한글은 단어 단위를 인식못함
- word-break: keep-all : 한중일 텍스트는 단어 단위로 줄바꿈 처리 / 나머지 텍스트는 노멀로 처리(단어 단위로 처리 ). 결국 모든 텍스트를 단어 단위로 처리하게 됨(단어 단위처리이므로 빠져나갈수 있음)
- word-break: break-all : 오버플로우가 되지 않도록 자동 줄바꿈 처리 / 영어의 경우 단어 단위가 아니라 중간에 짤려서 줄바꿈. 간단히 말하면 오버플로우가 되지 않도록 단어 단위가 아니라 알아서 잘라서 처리.

* [MDN| word-break](https://developer.mozilla.org/ko/docs/Web/CSS/word-break)

```CSS
word-break: keep-all;
word-break: break-all;
```
