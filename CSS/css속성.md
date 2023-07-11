### 속성
#### 너비(width, height)

>auto(기본값): 브라우저가 너비를 계산<br>
단위: px,em,vw 등 단위로 지정

max-width, max-height
>요소가 커질 수 있는 최대 가로/세로 너비<br> 최대 너비 제한 없음<br> px,em,vw 등 단위로 지정

min-width, min-height
>요소가 작아질 수 있는 최소 가로/세로 너비<br> 최소 너비 제한 없음<br> px,em,vw 등 단위로 지정

### 단위
> px 픽셀<br>
> % 상대적 백분율<br>
> em 요소의 글꼴 크기(글꼴크기*em)<br>
> rem 루트(최상위) 요소(html)의 글꼴 크기<br>
> vw 뷰포트 가로 너비의 백분율<br>
> vh 뷰포트 세로 너비의 백분율

### margin
요소의 외부 여백을 지정하는 단축 속성
>음수를 사용할 수 있다<br>
0:외부 여백 없음<br> auto:브라우저가 여백을 계산<br>단위:px,em,vw 등 단위로 지정<br> %: 부모 요소의 가로 너비에 대한 비율로 지정
### padding
요소의 내부 여백을 지정하는 단축 속성
>요소의 크기가 커진다.<br>0: 내부 여백 없음 <br>단위: px,em,vw 등 단위로 지정<br> %: 부모 요소의 가로 너비에 대한 비율로 지정

### border
요소의 테두리 선을 지정하는 단축 속성
>요소의 크기가 커진다.<br>
border: 선-두께[border-width: medium 중간두께 thin 얇은 두께 thick 주꺼운 두께 단위: px,em,% 등 단위로 지정] <br>선-종류[border-style none:선 없음, solid 실선, dashed 파선 dotted 점선, double 두 줄 선 groove 홈이 파여있는 모양 ridge 솟은 모양 inset 요소 전체가 들어간 모양 outset 요소 전체가 나온 모양]<br>선-색상[border-color <br>색상표현<br>
1. 색상이름:브라우저 제공 색상 이름
2. Hex 색상코드:16진수 색상
3. RGB:빛의 삼원색
4. RGBA:빛의 삼원색 + 투명도
5. HSL:색상,채도,명도
6. HSLA:색상,채도,명도+투명도 <br>border-radius
]

### box-sizing
>content-box:요소의 내용으로 크기 계산<br>
border-box: 요소의 내용 + padding + border로 크기 계산

### overflow
요소의 크기 이상으로 내용이 넘쳤을 때, 보여짐을 제어하는 단축 속성<br>
>visible: 넘친내용을 그대로 보여줌<br>
hidden: 넘친내용을 잘라냄<br>
scroll:넘친 내용을 잘라내고, 스크롤바 생성<br>
auto:넘친 내용이 있는 경우에만 잘라내고 스크롤바 생성<br>
overflow-x/y:요소의 크기 이상으로 내용이 넘쳤을 때, 보여짐을 제어하는 개별 속성들

### display
요소의 화면 출력 특성
>block:상자(레이아웃)요소
inline:글자요소
inline-block:글자+상자요소
flex:플렉스박스(1차원 레이아웃)
grid:그리드(2차원 레이아웃)
none:보여짐 특성없음, 화면에서 사라짐
기타: table,table-row,table-cell 등

### opacity
> 1: 불투명
> 0~1: 0부터 1 사이의 소수점 숫자

###글꼴
font-style:글자의 기울기
>normal:기울기 없음<br>italic:이텔릭체<br>oblique:기울어진 글자

font-weight:글자의 두께(가중치)
>normal,400:기본두께<br>bold,700:두껍게<br>bolder:상위(부모) 요소보다 더 두껍게<br>lighter:상위(부모)요소보다 더 얇게<br>100~900:100단위의 숫자 9개, normal과 bold 이외 두께

font-size:글자의 크기
>16px:기본 크기<br>단위:px,em,rem 등 단위로 지정<br>% 부모 요소의 폰트 크기에 대한 비율<br>smaller:상위(부모)요소보다 작은 크기<br>larger:상위(부모)요소보다 큰 크기<br>xx-small~xx-large: 가장 작은 크기~가장 큰 크기까지, 7단계의 크기를 지정

line-height:한줄의 높이,행간과 유사

>normal:브라우저의 기본 정의를 사용<br>숫자:요소의 글꼴 크기의 배수로 지정<br>단위:px,em,rem등의 단위로 지정<br>%:요소의 글꼴 크기의 비율로 지정
### 문자
> color: 글자의 색상<br>
> text-align:문자의 정렬방식<br>
> text-decoration: 문자의 장식(선)[none,underline,overline,line-through]
> text-ident:문자 첫줄의 들여쓰기

### 배경
background-color
> transparent:투명함<br> 색상:지정 가능한 색상
background-image:none <br>이미지 없음: url("경로"):이미지 경로

background-repeat
>repeat: 이미지를 수직,수평 반복<br> repeat-x:이미지를 수평반복<br>repeat-y:이미지를 수직 반복<br> no-repeat: 반복없음

background-position
요소의 배경 이미지 위치<br>
>0% 0%:0%~100% 사이의 값<br>
방향:top,bottom,left,right,center 방향<br>단위:px,em,rem등 단위로 지정

### background-size
요소의 배경 이미지 크기
>auto:이미지의 실제 크기<br>단위:px,em,rem 등 단위로 지정<br>cover:비율을 유지,요소의 더 넓은 너비에 맞춤<br>contain:비율을 유지,요소의 더 짧은 너비에 맞춤

### background-attachment
요소의 배경 이미지 스크롤 특성
>scroll: 이미지가 요소를 따라서 같이 스크롤<br>fixed:이미지가 뷰포트에 고정,스크롤X<br>local:요소 내 스크롤 시 이미지가 같이 스크롤

### 배치
## position
>요소의 위치 지정 기준 <br>static:기준없음<br>relative: 요소 자신을 기준 <br> absolute: 위치 상 부모 요소를 기준 <br>fixed: 뷰포트 기준 <br>sticky:스크롤 영역 기준
>!! position 속성의 값으로 absolute,fixed가 지정된 요소는 display 속성이 block으로 변경됨

### 요소 쌓임 순서(Stack order)
어떤 요소가 사용자와 더 가깝게 있는지(위에 쌓이는지)결정
1. 요소에 position 속성의 값이 있는 경우 위에 쌓임 (기본값 static 제외)
2. 1번 조건이 같은 경우 z-index 속성의 숫자 값이 높을 수록 위에 쌓임
3. 1번과 2번 조건까지 같은 경우 HTML의 다음 구조일 수롯 위에 쌓임

### z-index
>auto: 부모 요소와 동일한 쌓임 정도<br>숫자:숫자가 높을 수록 위에 쌓임 

### 플렉스(정렬)
1차원 레이아웃
display
>flex: 블록 요소와 같이 flex container 정의<br>inline-flex: 인라인 요소와 같이 flex container 정의

flex-direction: 주축을 설정
>row: 행 축(좌->우)<br>row-reverse: 행 축(우->좌)<br>columm: 열 축 (위->아래)<br>columm-reverse: 열 축 (아래->위)

flex-wrap: flex items 묶음(줄 바꿈)여부
>nowrap: 묶음(줄바꿈) 없음<br>warp: 여러 줄로 묶음(칸이 모자르면 넘겨라)<br>wrap-reverse: wrap의 반대 방향으로 묶음

justify-content :주 축(수평정렬)의 정렬방법
>flex-start:flex items를 시작점으로 정렬<br>flex-end:flex items를 끝점으로 정렬<br>center:flex items를 가운데 정렬<br>space-between: 각 flex item 사이를 균등하게 정렬<br>space-around: 각 flex item의 외부 여백을 균등하게 정렬

align-content: 교차 축의 여러 줄 정렬방법(수직정렬)
>stretch: flex items를 시작점으로 정렬<br>flex-start:flex items를 시작점으로 정렬<br>flex-end:flex items를 끝점으로 정렬<br>center: flex items를 가운데 정렬<br>space-between:각 flex item 사이를 균등하게 정렬<br>space-around: 각 flex item의 외부 여백을 균등하게 정렬

align-items: 교차 축의 한줄 정렬 방법(수직정렬)
>stretch:flex items를 교차 축으로 늘림
<br>flex-srart:flex items를 각 줄의 시작점으로 정렬<br>flex-end:flex items를 각 줄의 끝점으로 정렬<br>center:flex items를 각 줄의 가운데 정렬<br>baseline: flex items를 각 줄의 문자 기준선에 정렬

order:flex item의 순서
>0:순서X,숫자가 작을수록 먼저

flex-grow: flex item의 증가 너비 비율
>0:증가 비율 없음,숫자:증가비율

flex-shrink:flex item의 감소 너비 비율
>1:flex Container 너비에 따라 감소 비율 적용,숫자:감소비율

flex-basis:flex item의 공간 배분 전 기본 너비 
>auto:요소의 content 너비, 단위:px,em,rem등 단위로 지정

!!display:flex;가 지정된 요소:flex Container,의 자식요소:flex items
### 전환
transition:요소의 전환(시작과 끝)효과를 지정하는 단축 속성
>transition: 속성명 지속시간(단축형으로 작성할 때, 필수 포함 속성!) 타이밍 함수 대기시간;

transition-property: 전환효과를 사용할 속성이름을 지정
>all:모든 속성에 적용<br>속성이름: 전환 효과를 사용할 속성 이름 명시

transition-duration: 전환효과의 지속시간을 지정
>0s:전환 효과 없음<br> 시간:지속시간(s)를 지정

transition-timing-function:전환 효고의 타이밍(easing)함수를 지정
>ease:느리게-빠르게-느리게=cubic-bezier(0.25,0.1,0.25,1)<br>linear:일정하게=cubic-bezier(0,0,1,1)<br>ease-in:느리게-빠르게=cubic-bezier(0.42,0,1,1)<br>ease-out:빠르게-느리게=cubic-bezier(0,0,0.58,1)<br>ease-in-out:느리게-빠르게-느리게=cubic-bezier(0.42,0,0.58,1)<br>자신만의 값을 정의(0~1):cubic-bezier(n,n,n,n)<br>n번 분할된 애니메이션:steps(n)<br>!!참고:easing functions,easing functions mdn,tweenmax easing

transition-delay: 전환 효과가 몇 초 뒤에 시작할지 대기시간 지정
>0s:대기시간 없음<br>시간:대기시간(s)를 지정

### 변환
2D 변환 함수
>translate(x,y):이동(x축,y축)<br>
translateX(x):이동(x축)<br>
translateY(y):이동(y축)<br>
scale(x,y):크기(x축,y축)<br>
scaleX(x):크기(x축)<br>
scaleY(y):크기(y축)<br>
rotate(degree):회전(각도)<br>
skew(x,y):기울임(x축,y축)<br>
skewX(x):기울임(x축)<br>
skewY(y):기울임(y축)<br>
matrix(n,n,n,n,n,n):2차원 변환 효과

3D 변환 함수
>translateZ(x):이동(z축)<br>
translate3d(x,y,z):이동(x축,y축,z축)<br>scaleZ(z):크기(z축)<br>scale3d(x,y,z):크기(x축,y축,z축)<br>perspective(n):원근법(거리),가장 앞에 작성<br>matrix3d(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n):3차원 변환 효과<br>rotateX(x):회전(x축)<br>rotateY(y):회전(y축)<br>rotateZ(z):회전(z축)<br>rotate3d(x,y,z,a):회전(x축,y축,z축,각도)

perspective:하위 요소를 관찰하는 원근거리를 지정
>단위:px 등 단위로 지정

perspective 속성과 함수 차이점
|속성/함수|적용 대상|기준점 설정|
|---|---|---|
|perspective: 600px;|관찰 대상의 부모|perspective-origin|
|transform: perspective(600px)|관찰 대상|transform-origin|
<br><br>
backface-visibility:3D 변환으로 회전된 요소의 뒷면 숨김 여부

>visible:뒷면보임<br>hidden:뒷면숨김


