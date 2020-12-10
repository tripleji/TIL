## CSS

#### 기본 CSS

```
css의 뜻은 cascading style sheet 이다.

형식  selector {
	property: value;
}

text-align: 글씨정렬

font-weight: 400-보통 700-굵게

text-decoration-밑줄 이런 효과 주는거(underline, overline, line-through, wavy)

line-height- 문단 간격

letter-spacing- 글자 간 간격

font-family -글씨 폰트

universal selector= *{	} 전체에 적용

element selector= 버튼같은거 선택한 부분에만 적용

id selector= 특정 부분만 효과 넣고 싶을때 사용하면 좋다 #~~~{	}

class selector=중복되는 부분을 동시에 적용하고 싶을때 사용하면 좋음  .~~~{	}

Descendent selector= 내부에 있는 태그에 효과를 적용하고 싶을때

Adjacent selector= 같은 섹션안에 바로 효과를 주고 싶을 때 ~~+~~{	}

Direct Child=전체 효과가 있는 상태서 특정부분만 효과주고 싶을때 ~~>~~{	}

Attribute selector= 타입이름을 넣어서 원하는 부분에만 효과주고 싶을때  ~~[~~="~~""]{	}
```

#### Pseudo Class

```
1. 효과를 줄때 겹치는거는 가장 밑에 부분에있는 효과가 적용된다!!!

2. 같은 클래스 및 타입에 효과를 줄때 더 디테일하게 설정한거가 먼저 적용된다!!!

 적용 순서 => inline>ID>CLASS>ELEMENT 

!important쓰면 다무시하고 우선순위 1위

:hover = 선택햇을때 명암생기는 효과

:active= 클릭햇을때 생기는 효과

:nth-of-type(숫자)= 선택한 번호에 해당하는 라인의 색깔을 바꿔줌. 단!숫자n으로하면 숫자의배수 라인의 색깔 넣어줌

::first-letter = 글자의 첫글자마다 효과 주는거

::selection =드래그할때 색깔 효과주는거

```

#### CSS Box Model

```
width= 가로

height= 세로

border= 경계선

border-raidus = 사각형을 동그랗게 만들어준다!

padding= border 안쪽 간격을 (개발자 툴로 확인했을때 그린부분)

padding:  top/right/bottom/left

margin= border 바깥 쪽 간격!

box-sizing: content-box  =width 속성 값을 콘텐츠 영역 너비 값으로 사용

box-sizing: border-box = width 속성 값을 콘텐츠 영역에 테두리까지 포함한 박스모델 전체 너비 값으로 사용

display:inline = 가로로 나열! (width, height 속성 무시 margin, padding 상하 간격은 반영 X  좌우 간격만 반영)

display:block; = 세로로 나열 (width, height, margin, padding 속성 반영)

display:inline-block =가로로 나열(모든 속성 다 반영!)

%, em, rem = 상대적이다!(relative)

rgba(red, green, blue, alpha) 의 alpha 부분을 조절하면 투명하게 만들어주지만 텍스트는 그대로!

opacity= 텍스트 포함 전체다 투명하게 만들어줌

position: static =기본!

position: relative = 속성 및 좌표 값을 사용해 위치를 지정(문서 흐름 따라)

position: absolute  = 속성 값 원하는 위치에 배치하기(문서 흐름 상관 X)

position: fixed = 완전고정(브라우저 창 기준)

position: sticky= 고정이지만 움직인다!

transition =효과를 줌을로써 변화는 과정을 다 보여준다!

transition-timing-function: linear, ease-in, ease-out, step, cubic-bezier

transform:rotate = 각도에따라 회전가능

transform:scale = 사이즈 축소/확대 가능

transform:translate = x축 y축 정해서 이동 가능

transform:skew = 기울이기

box-shadow = 그림자주는 효과!

background-image: url("주소")

background-size:cover =가져온 이미지 전체를 다넣어준다

background-size:contain = 이미지크기가 넘으면 일부분 더보여줌

background-position = 위치 정할 수 있음

```
