## HTML

**H**yper**T**ext 하이퍼텍스트를 가장 중요한 특징으로 하는

**M**arkup 마크업이라는 형식을 가진

**L**anguage 컴퓨터 프로그래밍 언어

- 웹페이지 표시를 위해 개발된 지배적인 마크업 언어
- HTML은 제목, 단락, 목록 등과 같은 본문을 위한 구조적 의미를 나타내는 것뿐만 아니라 링크, 인용과 그 밖의 항목으로 구조적 문서를 만들 수 있는 방법을 제공한다.
- 출처 : 위키피디아

---

## HTML 기본양식

```html
<!DOCTYPE html>
<!-- html5 문서 타입 선언 (태그가 어떠한 표준,약속에 따라 제정된 태그인지 브라우저에게 알려주는것)-->
<html>
  <head>
    <!-- 웹서버는 영어가 기본이므로 한글로 된 내용을 표시할 때는-->
    <!-- UTP-8이라는 문자세트를 사용-->
    <title>제목</title>
    <meta charset="utf-8" />
  </head>
  <body></body>
</html>
```

- html과 /html사이의 문자는 **웹 페이지를 표현**한다.
- body와 /body사이의 문자는 표시되는 **페이지의 내용**이다.
- head와 /head사이의 문자는 눈에는 보이지 않지만 웹 페이지를 표현하기 위해 필요한 **헤더 정보**를 담고 있다.
- title과 /title사이의 문자는 웹 브라우저의 **페이지 제목**을 정의하는데 사용된다.

## HTML 주요태그&속성

- **HTML 태그(tag)** 는 HTML 요소(element)라고도 부르며, HTML 문서를 구성하는 기본 단위입니다.
- **HTML 속성** 은 태그만 사용해서는 동작하기는 뭔가 아쉬운 부분들을 속성이라는 기능을 추가적으로 적용함으로써 태그가 정상적으로 동작 할 수 있도록 만들어 주는 기능입니다.

```html
---태그---
<h1> </h1> ~ <h6> </h6> : 머리말
<a> </a> : 다른 콘텐츠와 연결되는 하이퍼링크 정의
<li> </li> : list
<ol> </ol> : Orderd list
<ul> </ul> : Unordered list
<br> </br> : 행바꿈을 정의
<header> </header> : 문자나 특성 섹션의 헤더를 정의함
<input> </input> : 사용자로부터 입력을 받을 수 있는 입력 필드를 정의함.
<label> </label> : 사용자 인터페이스 요소의 라벨을 정의함
<textarea> </textarea> : 사용자가 여러 줄의 텍스트를 입력할 수 있는 텍스트 입력 영역을 정의함

HTML 태그 모음(필요할 때 확인용)
: http://www.tcpschool.com/html-tags/intro


---속성---
<a href="링크"> : 링크로 이동
<img src="파일명"> : 이미지
<input type="" name="" value=""> : 파일 제출 양식
<input type="submit"> : 제출

HTML 태그 및 속성 모음(필요할 때 확인용)
: https://heropy.blog/2019/05/26/html-elements/
```

## CSS

- HTML 등의 마크업 언어로 작성된 문서가 실제로 웹사이트에 표현되는 방법을 정해주는 **스타일 시트 언어**.

---

## 기본규칙

- 선택자(selector)와 선언부(declaration)
- 선언부 -> 속성, 속성값
- <Style> </Style>을 통해 작성
