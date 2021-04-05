---
createdAt: 2021-04-04 14:00:00+09:00
updatedAt: 2021-04-04 14:00:00+09:00
---

# 파일 경로
텍스트 태그들을 알아본 다음에는 링크를 구현하는 **`a`** 태그에 대해 알아보려고 했는데, 그 전에 **파일의 경로**에 대해서 알아보고 넘어가는 게 좋을 수도 있다는 생각이 들었다.

프로그래밍에 처음 입문하는 분들은 뭐 경로, 주소 이런 말들을 들어봤을 것이다. 로컬 주소는 뭐고 웹 주소는 뭐고 참 헷갈린다. 이 개념에 대해 잘 알고 넘어가지 않으면 정말 헷갈리기 때문에 알아두는 게 좋다.

우리는 지금 HTML을 공부하고 있기 때문에 파일은 HTML에 기준을 두고 이야기하도록 하자. 다른 파일들도 다 마찬가지인데, 우리는 html이라는 확장자만을 이해할 수 있는 상태이니 html로 이야기하는 게 좋겠다.

대부분의 입문자들은 **로컬 주소**와 **웹 주소**가 무엇인지 잘 모를 것이다. 함께 알아보도록 하자.

일단 **주소**는 **경로**와 같은 말이다. 우리의 현실에서도 집 주소라고 하면 사실 집으로 가는 길과 같은 말이라는 걸 이해할 수 있다. 이처럼 경로와 주소는 같은 의미를 갖고 있다.

웹 개발에서는 경로라고도 하고 주소라고도 한다. 영어로는 **path**라고 한다. 그래서 이 경로에는 로컬 경로가 있고 웹 경로가 있다. 

---

## 로컬 주소
로컬 주소는 말 그대로 하드에 위치한 파일의 경로를 말한다. F 드라이브에 test.html 이라는 파일이 있다고 해보자. 그럼 로컬 주소는 **f:\test.html** 라는 주소가 된다.

주소 상에서 **슬래시(/)** 혹은 **역슬래시(\\)** 는 폴더의 내부를 의미한다. **f:/test.html**로 적을 수도 있는 셈이다. 아무튼 이 주소는 F 드라이브 안에 test.html라는 파일이 있다는 의미다.

```
f:\MultiMC\accounts.json
```

그렇다면 위의 주소는 어떤 의미일까. F:는 F 드라이브를 의미한다. 그리고 슬래시가 있으니 F 드라이브 내부를 의미할 것이다. MultiMC라는 경로가 있는데 **확장자가 없다.** 그리고 그 뒤에 슬래시가 있다. 이러면 **폴더라는 의미**이다. MultiMC 라는 폴더 안으로 들어간다. 라는 의미이다. 그리고 들어갔더니 accounts.json이라는 파일이 있는 것이다.

주소의 중간에 파일이 들어갈 수는 없다. 파일은 폴더가 아니기 때문이다. 파일은 항상 가장 끝에 위치한다. 중간 중간에 슬래시가 있다면 전부 폴더로 들어가는 것이다. 이 점을 기억해두자.

---

## 웹 주소
웹 주소의 경우도 사실 로컬 주소와 비슷하다. **웹상의 모든 페이지는 사실 다 파일이기 때문이다.** 이전 파트들중에서 이 말을 했던 파트가 있을 것이다.

```
https://www.naver.com
```

자, 위의 주소는 네이버의 메인 페이지 주소이다. 보통 메인 페이지라고 하면 다른 말로는 **개발폴더의 최상위 경로**라고 이해하면 된다. **루트 디렉토리**라고도 부른다.

우리가 우리의 프로젝트를 위해 개발폴더를 만든 것처럼, 네이버도 자기들 프로젝트를 위해서 개발폴더를 만들어놓은 것이다. 그리고 그 폴더가 **서버에 올라가 있기 때문**에 저렇게 이렇게 동작이 가능하다.

서버라는 단어를 꺼내긴 했지만, 서버가 무엇인가에 대해서는 지금 우리는 몰라도 된다. 지금 이야기하기엔 어려운 이야기이기 때문에 잠시만 넘어가도록 하자. 뭔지는 모르겠지만 **서버라는 것에 올라가야지만 웹에 보여질 수 있다.** 라는 것만 알아두면 된다.

또한 위의 주소는 **/index.html** 라는 부분이 제외된 것이다. **index.html**은 각 폴더의 메인 HTML 파일을 의미한다. 그렇기 때문에 제외해도 상관이 없다. 알아서 index.html을 찾아서 띄워주기 때문이다.

```
https://www.naver.com/index.html
```

그렇다면 지금까지 잘 이해가 되었다면 개발폴더의 최상위 경로에 index.html을 의미한다는 것을 알 수 있을 것이다. 왜 그런 것인지 생각해보자.

**https://www.naver.com** 이 부분을 최상위 폴더라고 생각하면 된다. 조금 많이 다른 비유지만 지금은 그렇게 생각하는 게 편하다. 그리고 이 폴더의 뒤에 슬래시가 있다 이 말은 폴더의 내부로 들어간다는 말이고 그 안의 **index.html**을 찾는다는 의미이다. 그래서 그 결과 메인 페이지가 띄워지는 것이다.

그렇다면 이제 다른 주소를 예로 들어보자. 내가 만들었던 사이트의 주소를 가져와보겠다.

```
https://random-keyword.github.io/keyword/character
```

이런 주소가 있다면, 어디가 최상위 폴더일까? **https://random-keyword.github.io** 바로 이 부분이다. 그 다음에 슬래시가 있고, 확장자가 없는 글자가 있다. 폴더이다. **keyword** 라는 폴더로 진입한다는 의미다. 그 다음에 또 슬래시가 있다.

어? 마지막에 위치하면 반드시 파일이라고 했는데 마지막인데도 불구하고 확장자가 없다. 이런 경우에 **/index.html** 가 생략 되어있다는 말이다.

```
https://random-keyword.github.io/keyword/character/index.html
```

이렇게 들어가도 잘 들어가지는 것을 볼 수 있다. 처음에는 어려울 수도 있는데, 이 점을 파악하고 있어야한다.

---

## 정리
1. 프로젝트의 최상위 폴더는 루트 디렉토리라고 부른다.
2. 로컬 주소나 웹 주소나 가장 마지막에 오면 파일이다. 웹 주소의 경우의 한정으로 가장 마지막에 오는 글자에 확장자가 없다면 **/index.html** 가 생략된 것이다.

---

## 상대 경로와 절대 경로
마지막으로 **상대 경로**와 **절대 경로**에 대해서 알아보도록 하자. 절대 경로는 일반적으로 인식하는 웹 주소이다. **https://random-keyword.github.io/keyword/character/index.html** 이런 주소가 절대 경로이다.

```
root
└ a.html
└ b.html
```

상대 경로는 살짝 복잡한데, 위처럼 루트 디렉토리에 두개의 파일이 있다고 가정해보자. 하나는 **a.html** 이고 다른 하나는 **b.html** 이다.

a.html 에서 아래와 같이 코딩하면 b.html이 링크된다.

```html
<a href="./b.html">B</a>
```

이런 것이 상대경로이다. 가장 앞의 **점(.)** 은 파일의 입장에서 **자신이 속한 폴더를 의미**한다. 그리고 **/b.html** 은 위에서 말했던 것처럼 해당 폴더 내의 파일을 찾는 것이다. 그래서 b.html이 선택되는 것이다.

그렇다면 같은 폴더가 아니라 루트 디렉토리의 바깥에 있는 파일은 어떻게 링크해야할까? 상대 경로에서 **./** 는 위에서 설명한 것처럼 자신이 속한 폴더를 의미하는데, **../** 는 상위 폴더를 의미한다.

```
a.html
root
└ b.html
```

그럼 이번에는 루트 디렉토리 안에 b.html 이 있고 루트 디렉토리가 있는 폴더에 a.html 이 있다고 가정해보자.

a.html 에서 b.html을 링크하려면

```html
<a href="./root/b.html">B</a>
```

이렇게 하면 된다. 지금까지 알게 된 것들이 적용되어 있다. 하지만 b.html 에서 a.html을 링크하려면 이렇게 해야한다.

```html
<a href="../a.html">A</a>
```

**../** 는 상위 폴더를 의미한다고 했다. **../** 를 이용해서 상위 폴더에 있는 a.html 을 찾는 것이다.

마지막으로 웹 환경에서 서버가 구동되고 있고 서버의 안에 프로젝트가 돌아가고 있을 때의 이야기이다. 서버의 아래에서 돌아가고 있다면 어떤 파일에서 링크를 하더라도 루트 디렉토리를 링크할 수 있는 방법이 있다.

```html
<a href="/">root</a>
```

그냥 이렇게 슬래시를 넣는 것이다. 슬래시는 루트 디렉토리를 의미한다. 정확히는 루트 디렉토리의 index.html을 의미한다.

루트 디렉토리 내의 파일들을 링크해야 할 때에는 **./** 가 아니라 **/**로 시작해도 된다. 프로그래밍에서 **./** 나 **../** 같은 상대 경로를 사용하는 이유는 루트 디렉토리가 아닌 곳에서 주소를 간략화해서 표현하기 위함이다. 시간 절약도 하고 말이다.

여기까지가 절대 경로와 상대 경로에 대한 이야기이다. 그럼 이제 링크 태그를 알아보러 갈 시간이다. 다음 파트로 넘어가도록 하자.