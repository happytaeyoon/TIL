``` 
선택자 {
   속성: 값;
   속성: 값;
 }
 ```

 ### CSS 선언 방식
1. 내장방식 : ```<style></style```의 내용으로 스타일을 작성하는 방식
```
<style>
  div{
    color: red;
    margin: 20px;
     }
<style>
```
2. 링크방식: ```<link/>```로 외부 CSS 문서를 가져와서 연결하는 방식
3. 인라인방식: 요소의 style 속성에 직접 스타일을 작성하는 방식(선택자 없음)
```
<div style="color: red; margin: 20px;"><div>
```
4. @import 방식: CSS의  @import 규칙으로 CSS 문서 안에서 또 다른 CSS 문서를 가져와 연결하는 방식
### CSS 선택자
1. 기본: <br>

1-1: 전체 선택자
 ```
 모든 요소 선택
*{
  color: red;
}
 ```
1-2.태그 선택자
```
같은 태그 선택
li{
  color: red;
}
```
1-3.클래스 선택자
```
class 속성의 값이 같은 태그 선택
.orange{
  color: red;
}
```
1-4.아이디 선택자
```
id 속성의 값이 같은 태그 선택
#orange{
  color: red;
}
```
2. 복합<br>

2-1.일치 선택자
```
선택자 ABC와 XYZ를 동시에 만족하는 요소 선택
span.orange{
  color: red;
}
```
2-2.자식 선택자
```
선택자 ABC의 자식 요소 XYZ 선택
ul > .orange{
  color: red;
}
```
2-3.하위(후손) 선택자
```
선택자 ABC의 하위 요소 XYZ 선택. 띄어쓰기가 선택자의 기호
div .orange{
  color: red;
}
```
2-4.인접 형제 선택자
```
선택자 ABC의 다음 형제 요소 XYZ 하나를 선택
.orange + li{
  color: red;
}
```
2-5.일반 형제 선택자
```
선택자 ABC의 다음 형제 요소 XYZ 모두를 선택
.orange ~ li{
  color: red;
}
```
3. 가상 클래스
<br>

3-1.HOVER
```
선택자 ABC 요소에 마우스 커서가 올라가 있는 동안 선택
a:hover{
  color: red;
}
```
3-2.active
```
선택자 ABC요소에 마우스를 클릭하고 있는 동안 선택
a:active{
  color: red;
}
```
3-3.FOCUS
```
선택자 ABC요소가 포커스되면 선택
input:focus{
  background-color: orange;
}

tabindex 속성을 통해 focus가 될수 있는 요소를 만들 수 있다 -1 넣는걸 권장
```
3-4.first child
```
선택자 ABC가 형제 요소 중 첫째라면 선택
.fruits span:first-child{
  color: red;
}
```
3-5.last child
```
선택자 ABC가 형제 요소 중 막내라면 선택
.fruits h3:last-child{
  color: red;
}
```
3-6.NTH child
```
선택자 ABC가 형제 요소 중 (n)째라면 선택
.fruits *:nth-child(2){
  color: red;
} 
2n일시 0부터 2의배수(짝수요소)
2n+1일시 1부터 홀수배수
```
3-7.부정 선택자
```
선택자 XYZ아닌 ABC요소 선택
.fruits *:not(span){
  color: red;
}
```
4. 가상 요소

4-1:before
```
선택자 ABC 요소의 내부 앞에 내용을 삽입(inline요소)
.box::before{
  content:"앞!";
}
```
4-2:after
```
선택자 ABC 요소의 내부 뒤에 내용을 삽입(inline요소)
.box::after{
  content:"뒤!";
}
```
5. 속성

5-1.ATTR
```
속성 ABC를 포함한 요소 선택
[disabled]{
  color: red;
}
```
5-2.ATTR=VALUE
```
속성 ABC을 포함하고 값이 XYZ인 요소 선택
[type="password"]{
  color: red;
}
```
### 상속되는 CSS 속성들
#### 모두 글자/문자 관련 속성들 (모든 글자/문자 속성은 아님 주의!!!)
1. font-style :글자 기울기
2. font-weight :글자 두께
3. font-size :글자 크기
4. line-height :줄 높이
5. font-family :폰트(서체)
6. color :글자 색상
7. text-align :정렬
강제상속 inherit: 부모요소에 상속

### 선택자 우선순위
우선순위란 같은 요소가 여러 선언의 대상이 된 경우, 어떤 선언의 CSS 속성을 우선 적용할지 결정하는 방법
1. 점수가 높은 선언이 우선함!
2. 점수가 같으면, 가장 마지막에 해석된 선언이 우선함!
```
전체 선택자-0점, 태그 선택자-1점, Class 선택자-10점,  ID 선택자-100점,인라인 선언-1000점,!important-무한점
```
