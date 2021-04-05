---
createdAt: 2021-04-03 17:20:00+09:00
updatedAt: 2021-04-04 17:00:00+09:00
---

# 링크 태그
이번 파트에서는 **링크**에 대해 알아보도록 하자. 링크는 웹의 근간이자 **웹의 꽃**이다. 링크는 **연결, 연결된**이라는 의미의 영단어이다. 웹에서의 링크는 이 영단어를 바탕으로 기능이 구현되어있다. 링크는 **`a`** 태그로 구현할 수 있다.

그리고 지금 다루는 링크라는 것이 바로 하이퍼 링크를 의미한다. **`a`** 태그는 상당히 중요한 위치에 있는 것이다. **`a`** 태그가 있기 때문에 지금의 웹이 존재할 수 있었다는 것을 생각해두자.

**`a`** 태그의 a는 닻을 의미하는 **Anchor**의 약자이다.

```html
<a href="url">링크</a>
```

![a 태그를 사용한 모습](https://i.postimg.cc/4469DmD2/K-20210404-043742.png)

**`a`** 태그는 기본 디자인이 마찬가지로 정해져 있는데, 파란 글씨에 밑줄이다. 클릭했던 링크는 보통 보라색이 된다. 이는 브라우저마다 다를 수 있는지 참고만 하자.

**`a`** 태그는 **`href`** 라는 속성을 사용한다. 이 안에는 파일의 경로가 들어간다. **`a`** 태그는 파일과 파일을 서로 연결하는 역할을 하는 웹에서 아주 중요한 태그이기 때문에 **이 속성이 가장 가장 가장 중요**하다고 할 수 있다.

여기서 파일의 경로라는 것은 로컬 주소일 수도 있고 웹 주소일 수도 있다. 파일 경로에 대한 이야기는 [파일 경로](./10-file-path.md) 파트를 참고하면 되겠다.

---

## 연습 시간
우리가 만든 index.html 파일을 다시 꺼내보자. 현재 이 파일의 상황은 다음과 같을 것이다.

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <link rel="stylesheet" href="./style.css">
  <title>웹 개발 기술들</title>
</head>
<body>
  <h1>웹 개발 기술들</h1>
  <h2>HTML</h2>
  <p>HTML이란 <em><strong>Hyper Text Mark-up Language</strong></em>의 약자로 마크업 언어를 말한다. 마크업 언어는 웹의 뼈대를 구성하는 언어라고 이해하면 되겠다. 웹을 구성하는 세가지 요소중 가장 중요한 요소이다.</p>
  <h2>CSS</h2>
  <p>CSS는 <em><strong>Cascading Style Sheets</strong></em>의 약자로, 스타일을 입히기 위한 언어이다. 디자인을 맡고 있다.</p>
  <h2>JavaScript</h2>
  <p><em><strong>JavaScript(이하 자바스크립트)</strong></em>는 웹을 동적으로 제어하기 위한 프로그래밍 언어 혹은 스크립트 언어이다. HTML과 CSS를 전부 조정할 수 있다.</p>
</body>
</html>
```

**`link`** 태그는 몰라도 된다. 지금 다루지 않을 것이다. 우리가 만든 이 문서에 링크를 추가해보도록 하자. 나는 각각의 **`h2`** 태그들에 링크를 입힐 것이다.

```html
<h2>HTML</h2>
```

이렇게 생긴 상태인데, **`h2`** 태그의 내부의 HTML 이라는 글자에 **`a`** 태그를 입혀줄 것이다. 그럼 이렇게 된다.

```html
<h2><a href="">HTML</a></h2>
```

**`a`** 태그에서 **`href`** 속성은 아주 중요하다고 했다. 이 상태에서 주소를 적어주면 되겠다. 나는 구글 검색 결과를 넣어주도록 하겠다. 제목을 누르면 구글 검색 결과창으로 넘어가도록 말이다.

```html
<h2><a href="https://www.google.co.kr/search?q=HTML&newwindow=1&bih=935&biw=1870&hl=ko&sxsrf=ALeKk01U7gGj3gCKsnPlnaGaXn1wVl_bgw%3A1617515174339&ei=plJpYPuhFOuQr7wP2Ymk4AE&oq=HTML&gs_lcp=Cgdnd3Mtd2l6EAMyBAgjECcyBAgjECcyBAgjECcyBwgAELEDEEMyBQgAELEDMgUIABCxAzIFCAAQsQMyAggAMgIIADICCAA6CAgAELEDEIMBOgQIABADOgcIIxDqAhAnUO0IWLUbYJ0eaARwAHgAgAGUAYgB-AeSAQMwLjmYAQCgAQGqAQdnd3Mtd2l6sAEKwAEB&sclient=gws-wiz&ved=0ahUKEwj7jIrL8ePvAhVryIsBHdkECRwQ4dUDCA0&uact=5">HTML</a></h2>
```

```html
<h2><a href="https://www.google.co.kr/search?q=CSS&newwindow=1&bih=935&biw=1870&hl=ko&sxsrf=ALeKk010qomzi4Y72vc9Jhg9lGdTRFFHMw%3A1617515178937&ei=qlJpYK_QOOiVr7wPocqqgAg&oq=CSS&gs_lcp=Cgdnd3Mtd2l6EAMyBAgjECcyBAgjECcyBwgAELEDEEMyBAgAEEMyBAgAEEMyBAgAEEMyBAgAEEMyBAgAEEMyBAgAEEMyBAgAEEM6BQgAELEDUPppWNJsYMJvaABwAngAgAH8AYgB-wSSAQUwLjMuMZgBAKABAaoBB2d3cy13aXrAAQE&sclient=gws-wiz&ved=0ahUKEwivzaLN8ePvAhXoyosBHSGlCoAQ4dUDCA0&uact=5">CSS</a></h2>
```

```html
<h2><a href="https://www.google.co.kr/search?q=JavaScript&newwindow=1&bih=935&biw=1870&hl=ko&sxsrf=ALeKk02wervRU39b323dnlIASjdru4dRLQ%3A1617515194037&ei=ulJpYLvnAaSmmAXnjrvYAw&oq=JavaScript&gs_lcp=Cgdnd3Mtd2l6EAMyBAgjECcyBAgjECcyBAgjECcyBwgAELEDEEMyBAgAEEMyBwgAEIcCEBQyBAgAEEMyBAgAEEMyBAgAEEMyBwgAELEDEEM6BggjECcQEzoFCAAQsQM6CAgAELEDEIMBUNZyWOaJAWCejAFoAXACeACAAbUBiAHXCpIBBDAuMTKYAQCgAQGqAQdnd3Mtd2l6wAEB&sclient=gws-wiz&ved=0ahUKEwi7rLzU8ePvAhUkE6YKHWfHDjsQ4dUDCA0&uact=5">JavaScript</a></h2>
```

검색 결과 페이지의 주소가 드럽게 길지만 일단 이렇게 넣어주고 저장을 한다. 그럼 제목들이 링크가 된다.

![a 태그 사용하기](https://i.postimg.cc/65rZhPhP/K-20210404-144724.png)

이미 다 방문했었던 페이지라서 보라색이지만, 여러분들은 아마 파란색으로 잘 뜰 것이다. 만들어진 링크를 클릭해보면 넘어가는 것을 볼 수 있다.

그런데 현재 페이지가 아니라 새로운 창 또는 새로운 탭에서 링크를 띄우고 싶어졌다. 어떻게 해야할까? 그럴 때에는 **`a`** 태그의 **`target`** 속성을 사용해야한다.

---

## 새 창(탭)에서 띄우기
```html
<a href="#" target="_blank|_self|_parent|_top">링크</a>
```

**`target`** 속성에는 네가지의 값이 들어갈 수 있다. 이 중에서 크게 두가지만 알아도 된다. **`_blank`** 와 **`_self`** 만 알아도 큰 불편함은 없다.

```html
<a href="#" target="_self">링크</a>
```

```html
<a href="#" target="_self" rel="noreferrer">링크</a>
```

이렇게 **`_self`** 로 설정하면 현재 창(탭)에서 링크가 열리게 된다. 그런데 이 값은 기본값이다. 입력하지 않아도 자동으로 현재 창에서 열리기 때문이다.

두번 째는 **`target`** 속성을 사용했을 때에 추가적으로 설정을 해주어야 하는 속성이다. **`rel`** 속성이 추가된 것을 볼 수 있는데, 상세한 의미는 몰라도 된다. 어떤 사람들은 링크를 클릭할 때를 노려 악의적인 수작을 부리는 경우도 있기 때문에 그것을 막는 역할을 한다는 것으로 이해하면 된다.

현재창에서 링크를 여는 것이 기본값이기 때문에 **`target`** 속성을 쓰지 않는다면, 저 추가적인 설정을 하지 않아도 되지만, 기본값이지만 굳이 **`target`** 속성을 쓰고 싶다면 저 설정도 해주어야 한다.

쉽게 말하면 **`target`** 속성의 **`_self`** 값을 사용한다면 그냥 두번째 코드처럼 설정하면 된다.

```html
<a href="#" target="_blank">링크</a>
```

```html
<a href="#" target="_blank" rel="noreferrer noopener">링크</a>
```

이렇게 **`_blank`** 를 설정하면 새로운 창 혹은 새로운 탭에서 열리게 된다. 이게 더 편할 것이다. 나는 이 값을 자주 사용한다. 새 창으로 띄우기 위해선 이 값을 사용하면 되는 것이다.

**`target="_blank"`** 속성을 사용할 때에는 알아둬야 할 것이 있다. 추가적으로 설정을 해줘야 보안적으로 안전하다는 것이다. rel 속성을 추가적으로 설정해서 보안을 높여줄 수 있다.

**`rel`** 속성에 **`noreferrer`** 뿐만 아니라 **`noopener`** 도 같이 적용해주는 것을 웹 표준에서 권장하고 있기 때문에 새 창 혹은 새 탭에서 링크가 띄워지길 원하는 분들은 두번째 코드처럼 설정하면 된다.

---

## 다른 html 파일 링크하기
그럼 이제 마지막으로 로컬 경로 안에 있는 다른 파일을 링크해보도록 하자. 우리의 개발 폴더에 **test.html** 파일을 하나 만들어보자. vscode에서 간단하게 파일을 추가할 수 있다.

![새 파일을 누르면 새로운 파일을 만들 수 있다](https://i.postimg.cc/VvxVckZm/K-20210404-151633.png)

![파일 이름을 입력하면 사용할 수 있다](https://i.postimg.cc/SRCwR9MJ/K-20210404-151518.png)

왼쪽의 파일 탐색기에서 우클릭하고, 새 파일을 누르면 파일 하나가 만들어지는데, 이름을 입력하면 그때부터 사용할 수 있다.

파일을 만들었으면 기본적인 구조를 만들어준다. 이제 이 기본적인 구조는 다 알 것이라고 생각한다. 모른다면 [HTML의 기본적인 구조](./4-html-default.md) 파트를 참고하도록 하자. 되도록이면 익혀두자.

test.html 파일의 body 태그의 내부에 다음과 같은 코드를 작성해보자.

```html
<p>
  <a href="/">메인 페이지</a>
</p>
```

이 코드는 메인페이지를 링크하는 코드이다. **서버 환경에서는 슬래시 하나가 루트 디렉토리**라고 했다. 루트 디렉토리의 index.html을 의미하는 것이다. 단, 여러분이 이 효과를 제대로 보기 위해서는 **라이브 서버**를 작동시켜야한다.

우리는 vscode를 설치하면서 라이브 서버라는 확장 프로그램을 설치했는데, 하단에 **Go Live**라는 버튼이 있을 것이다. 그것을 눌러서 테스트를 하면 되겠다.

서버 환경이 아닌 로컬 환경에서 더블 클릭으로 실행하고 있었다면 이제부터는 라이브 서버를 이용해서 연습을 진행하도록 하자. 왜 그래야하는 것인가 하면 단장에 저 코드가 적용된 파일을 더블 클릭해서 실행하게 되면 루트 디렉토리가 아니라 **드라이브의 최상위 폴더로 이동**하기 때문이다. 우리가 원하는 것은 그런 게 아니다.

아무튼, index.html 에서도 test.html 을 링크시켜야 하는데, 아래의 코드를 추가적으로 작성해주었다. 기존의 코드의 아래에 이어서 작성하는 것이다.

```html
<hr />

<p>
  <a href="/test.html">테스트 페이지</a>
</p>
```

이것을 추가하고 라이브 서버를 돌려보면 아래와 같이 잘 추가되었다면 성공이다. 이제 테스트 페이지라는 링크를 눌러보자. 우리가 만든 test.html 이 나타나면 성공이다.

![index.html](https://i.postimg.cc/xqDVP2mp/K-20210404-165241.png)

![test.html](https://i.postimg.cc/52WFXQXL/K-20210404-165532.png)

축하한다. 여러분은 처음으로 웹 사이트를 만들었다. 웹의 꽃을 배웠으니 이번 파트의 내용은 확실하게 기억하고 있길 바란다.