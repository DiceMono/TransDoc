# TransDoc (가제)

- 내가 필요해서 만드는 개발 문서 번역 툴
- [AWS Translate](https://aws.amazon.com/ko/translate/) 를 이용해 문서 번역을 도와주는 크롬 익스텐션
- [파파고 크롬 익스텐션](https://chrome.google.com/webstore/detail/papago-translate/enddgifdbfoefnelepppgaabobdfbcpe?hl=ko)과 주요 기능은 동일

## 개선점

### 1. `<code></code>` 코드 블럭을 드래그 해도 번역이 자연스럽게 
    
![x](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/00b44b7a-5ea8-4662-9d79-fc4c1d5b1e20/screenshot.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221024%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221024T093716Z&X-Amz-Expires=86400&X-Amz-Signature=fb593d55fd43e40fe795aa41b1320ecef2f3111131058e9c610e46e9017c24f3&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22screenshot.png%22&x-id=GetObject)
    
```html
To do that, use the standard Python type hint <code>typing.Union</code>
```
To do that, use the standard Python type hint `typing.Union`

---

### 2. pdf 번역 지원

`<embed type="application/pdf">` 는 불가능

[mozilla/pdf.js](https://mozilla.github.io/pdf.js/web/viewer.html)는 가능

---
### 3. 번역 api 성능 차이

#### 1) "--" 처리

Fluent Python 2nd edition Ch.19

> This may involve concurrent or parallel programming—even academics who are keen on jargon disagree on how to use those terms.
> 

* 파파고

이것은 동시 또는 병렬 프로그래밍을 포함할 수 있다.

* AWS Translate

여기에는 동시 또는 병렬 프로그래밍이 포함될 수 있습니다. 전문 용어에 관심이 있는 학자들도 해당 용어를 사용하는 방법에 동의하지 않습니다.


--- 