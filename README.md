---
createdAt: 2021-03-26 09:15:00+09:00
updatedAt: 2021-04-07 17:29:00+09:00
---

# 개요
프로그래밍을 공부하면서 단순한 지식부터 시작하여 지식의 응용, 여러가지 프로젝트를 만들어보면서 시행착오를 기록하는 공간을 마련하기 위해 TIL을 만들었다.

프로그래밍을 할 때마다 이 곳에 기록할 것을 염두하고 좀 더 생산적인 작업을 할 수 있으면 좋겠다. 누군가 이 TIL을 볼 수 있다는 것과 상관 없이 남들에게 막히지 않고 설명할 수 있는 연습을 하기위해서라도 꾸준히 건드려볼 생각이다.

그것을 위해 기초적인 언어 복습을 할 생각이다.

---

## 무엇을 다루는가
우리는 프로그래밍을 위한 언어를 배울 것이다. 그것들을 개발자들은 프로그래밍 언어라고 한다. 프로그래밍 언어는 상당히 많다. 그 중에서 우리가 다룰 것은 웹 프로그래밍을 위한 언어들이다.

웹 프로그래밍을 위한 언어들도 상당히 많고 대다수의 프로그래밍 언어들이 웹 개발에 발을 담그고 있다. 하지만 우리는 가장 기본적인 언어들을 배울 것이다. HTML부터 시작해서 CSS를 거쳐 자바스크립트에 대한 다양한 기술을 배워 나갈 것이다.

프로그래밍은 무엇이고 프로그래밍 언어는 무엇인지에 대해서는 아래의 **[시작하기 전에](intro/README.md)** 문서를 확인해보면 좋을 것 같다.

중요한 것은 이것은 강의가 아니라는 점이다. 나와 함께 공부를 하는 일종의 스터디라고 생각하자. 함께 공부를 한다는 생각으로 공부에 임하면 조금이라도 덜 지루할 것이다.

사실 지루할 틈은 없을지도 모른다. 처음 프로그래밍을 배우는 사람은 복잡하다는 이유로 미칠 정도로 팔짝 뛰거나 새로운 세상에 대한 감탄으로 신기할테니 말이다.

---

## 목차
이 아래의 목차는 되도록이면 순차적으로 보는 것을 추천한다. 우선적으로 알아두면 좋은 사실은 아래의 기술들이 항상 매번 전부 사용되지는 않는다는 것이다. 그렇기 때문에 모든 것을 외울 필요는 없다.

현직 개발자들도 모든 것을 외우지는 않는다. 필요하고, 자주 쓰는 것만을 우선적으로 외우는 것이 좋다.

* **시작하기 전에**
  * [프로그래밍과 프로그래밍 언어](intro/1-what-is-programing.md)
  * [웹과 웹 프로그래밍](intro/2-what-is-web-programing.md)
  * [목표의 중요성](intro/3-your-purpose.md)
* **마크업 언어**
  * **HTML**
    * [개요](html/README.md)
    * [기본적인 문법](html/1-syntax.md)
    * [태그의 특징](html/2-block-and-inline.md)
    * [태그와 태그의 관계](html/2-parent-child-sibling.md)
    * [정비 - 개발환경 구축](html/3-coding-environment.md)
    * [HTML의 기본적인 구조](html/4-html-default.md)
    * [시맨틱 태그](html/4-semantic-tags.md)
    * [주석](html/9-comment.md)
    * [공간 분할 태그(div, span)](html/8-division-tags.md)
    * **텍스트 관련 태그**
      * [제목 태그(h1~h6)](html/text/1-heading-tag.md)
      * [문단 태그(p)](html/text/2-paragraph-tag.md)
      * [정비 - Visual Studio Code 사용하기](html/6-vscode-download.md)
      * [정비 - VSCode 추천 확장 프로그램](html/7-vscode-extension.md)
      * [굵기와 기울기 태그(b, strong, i, em)](html/text/3-bold-italic.md)
      * [개행 태그와 가로줄 태그(br, hr)](html/text/4-br-hr-tag.md)
      * [윗첨자와 아랫첨자 태그(sup, sub)](html/text/5-sup-and-sub.md)
      * [텍스트의 추가, 제외 태그(ins, del)](html/text/6-ins-and-del.md)
      * [취소선과 밑줄 태그(s, u)](html/text/7-line-tags.md)
      * [인용 태그(q, blockquote)](html/text/8-quote-tags.md)
      * [하이라이트 태그(mark)](html/text/9-mark-tag.md)
      * [small 태그](html/text/10-small-tag.md)
      * [code, pre 태그](html/text/11-code-pre-tag.md)
      * [abbr 태그](html/text/12-abbr-tag.md)
      * 그 외의 텍스트 태그들 - 미작성
    * [파일 경로](html/10-file-path.md)
    * [링크 태그(a)](html/11-link-tag.md)
    * **이미지 관련 태그**
      * [이미지 태그(img)](html/image/1-img-tag.md)
      * [심화 - 이미지맵 태그(map, area)](html/image/2-map-area-tag.md)
    * **목록 관련 태그**
      * [순차 목록과 비순차 목록 태그(ol, ul, li)](html/list/1-list-tags.md)
      * [용어 설명 목록 태그(dl, dt, dd)](html/list/2-description-list-tag.md)
    * **테이블 관련 태그**
      * [테이블 태그(table, tr, th, td)](html/table/1-table-tags.md)
      * **테이블 태그 심화**
        * [테이블 태그 심화 1) thead, tbody, tfoot](html/table/2-table-hard-1.md)
        * [테이블 태그 심화 2) colgroup, col, caption](html/table/3-table-hard-2.md)
    * **폼 관련 태그**
      * [form 태그](html/form/1-form-tag.md) - 작성예정
        * form 태그 심화 - 미작성
      * input 태그 1) 기본적인 속성 - 미작성
      * input 태그 2) 여러가지 타입 - 미작성
      * input 태그 3) 데이터 검증 - 미작성
      * textarea 태그 - 미작성
      * button - 미작성
      * select 태그 - 미작성
      * fieldset - 미작성
      * datalist - 미작성
    * **멀티미디어 관련 태그**
      * 멀티미디어 태그들(audio, video, source) - 미작성
      * iframe 태그 - 미작성
    * figure, figcaption 태그 - 미작성
    * **레이아웃 태그들**
      * 레이아웃 태그 1) header, nav, main - 미작성
      * 레이아웃 태그 2) aside, footer - 미작성
      * 레이아웃 태그 3) article, section - 미작성
    * 메타데이터 태그들(meta) - 미작성
    * 요약 태그(details, summary) - 미작성
    * **CSS 관련**
      * style 속성 - 미작성
      * style 태그 - 미작성
      * link 태그 - 미작성
    * **JS 관련**
      * script 태그 - 미작성
      * JS 이벤트와 관련된 속성들 - 미작성
    * **HTML 심화**
      * 커스텀 속성 사용하기 - 미작성
      * 섹션(Section)과 아웃라인(Outline) - 미작성
      * 웹표준에 대해 - 미작성
      * 브라우저 지원 고려하기 - 미작성
* **스타일 시트 언어**
  * 준비중
* **프로그래밍 언어**
  * 준비중

---

## 연락처
혹시라도 이 TIL의 내용을 어딘가에 가져가고 싶다면 아래의 연락처 중에서 편한 수단을 선택해 연락주시면 답변 드리겠습니다. 혹은 제가 작성한 내용들 중에서 수정되었으면 더 자연스러울 것 같은 내용이나 잘못된 내용이 있으면 누구라도 좋으니 지적해주시면 정말 감사하겠습니다.

* 이메일: [nihil_ncunia@naver.com](mailto:nihil_ncunia@naver.com)
* 인스타그램: [@nihil_illust](https://www.instagram.com/nihil_illust/)