---
createdAt: 2021-04-05 00:54:00+09:00
updatedAt: 2021-04-05 01:20:00+09:00
---

# 이미지 관련 태그
웹에는 수많은 이미지들이 존재한다. 그 이미지들은 어떻게 구현되어 우리의 눈에 보이는 것일까? 배경 이미지도 사실 이미지지만 그것은 CSS가 필요한 영역이기 때문에 HTML 파트에서는 다루지 않을 것이다.

우리는 이번 파트에서 이미지를 구현하는 태그에 대해서 알아볼 것이다.

웹 상에서 이미지를 나타내는 태그는 **`img`** 태그 이다. 당연하게도 **`img`** 태그는 **Image**라는 단어의 약자이다.

**`img`** 태그는 닫는 태그가 없다. 따라서 홀로 닫는 태그이다. 또한 하나의 필수 속성을 가진다. 사실상 필수 속성은 두가지인데, 속성에 대해서는 아래에서 살펴보도록 하고 지금은 어떻게 보이는지에 대해서 한 번 알아보도록 하자.

```html
<img src="주소" alt="보이지 않을 때 이미지" />
```

아무 html 파일이나 만들고 기본 구조를 만든 후에 위의 코드를 작성해보자. 그리고 라이브 서버를 통해 실행을 해보면 아래와 같이 뜰 것이다.

![img 태그의 주소가 제대로 되지 않았을 때](https://i.postimg.cc/tJ8VWdFG/K-20210405-013730.png)

보이지 않을 때 이미지 라는 글씨만 보일 뿐 이미지는 보이지 않는다. 당연하다. **`src`** 속성에 주소를 입력하지 않았다. 웹상에는 주소라는 이미지 따위 없기 때문에 이미지로 인식하지 못한 것이다.

이미지가 깨졌을 때에 저렇게 나오는데, 글씨가 나오는 이유는 **`alt`** 속성 때문이다. **`alt`** 속성은 이미지가 혹여나 보이지 않을 때에 어떤 이미지인지 유추라도 가능하도록 적어둔 설명을 적는다.

**`src`** 속성은 위의 코드에서 적은 것처럼 주소를 의미한다. 이미지의 주소를 적으면 된다. 로컬에 있는 이미지든 웹 상의 주소든 무엇이든 들어가면 실행했을 때에 보이게 된다.

그럼 이제 제대로 작성해서 띄워보도록 하자.

```html
<img src="https://i.pinimg.com/originals/ae/5e/58/ae5e58ef6434c5d61cb7bf996141cb80.jpg" alt="호텔 델루나 장만월" />
```

![img 태그를 제대로 활용했을 때](https://i.postimg.cc/PxQjmdZX/K-20210405-013721.png)

이미지가 보이긴 한다! 그런데 내가 넣은 이미지가 사이즈가 너무 큰 모양이다. 하지만 이는 매우 일부러 의도한 결과이다. 또 다른 속성을 배우기 위함이다.

이미지의 사이즈를 설정할 수 있는 두 가지의 속성에 대해서 알아보자. 가로 사이즈를 조정하는 **`width`** 속성과 세로 사이즈를 조정하는 **`height`** 속성을 알아보도록 하자. 이 두가지의 속성에는 픽셀 단위가 들어간다.

```html
<img src="https://i.pinimg.com/originals/ae/5e/58/ae5e58ef6434c5d61cb7bf996141cb80.jpg" alt="호텔 델루나 장만월" width="500px" />
```

![이미지의 사이즈를 줄인 모습](https://i.postimg.cc/T1DycLd8/K-20210405-015610.png)

사이즈가 조절되니 이미지가 잘 보인다. 그렇다. 역시 아이유이다. 위의 코드처럼 가로 크기만 정하면 세로 크기는 알아서 자동으로 설정되고, 세로 크기만 정하면 가로 크기가 알아서 설정된다. 당연한 말이지만 둘 다 설정할 수도 있다. 둘 다 설정하게 되면 비율이 깨질 수도 있다는 점은 알아두자. 옆으로 늘어난 형태가 되거나 찌그러진 형태가 될 수도 있을 것이다.

하지만 보통은 CSS를 이용해서 사이즈를 조절하는 편이다. 그게 더 편리한 편이다.

---

## 이미지와 함께 사용할 수 있는 태그들
위에서 기본적인 속성들은 알아봤다. **`img`** 태그의 사용 방법은 여기에서 끝나지 않는다. 몇가지의 다양한 기술을 활용할 수 있다. 조금 머리가 아플 수도 있으니 천천히 알아보도록 하자.

다음 파트에서는 **`img`** 태그와 함께 사용할 수 있는 다른 태그들에 대해서 추가적으로 알아볼까 한다.

[map 태그, area 태그](./2-map-area-tag.md): img 태그에 심화적으로 접근하면 이미지맵이라는 개념을 빼놓을 수 없다. 이미지맵이라는 것은 하나의 이미지 안에 여러 개의 링크를 설정하는 것이다. 이미지의 어떠한 곳을 클릭하면 설정된 곳으로 링크 된다고 생각하면 된다.