# Today I Learned (TIL)
>내가 직접 배운 내용을 정리해두는 학습 저장소 

>이해한 만큼만 직접 작성하겠습니다!!!!

>틀린 부분이 있으면 언제든지 말해주세요!!
-------------------------------------------------------------------------------------------------------------------


## Responsive Web

#### 반응형 웹 만들 때 팁!!

##### Typography
```
pretty important, easy to read

headline&title - 60~90px

body-15~25px 

line spacing - 120~150% easy to read

per line - 45~90 characters!

good fonts - sans-serif(더 자주 쓰임), serif ==>구글 폰트토 쓸만한게 많다
```

##### Color
```
flat ui colors

adobe cc color

never use original black color- not natural

red-energetic
orange- draw attention, creativity, confidence
yellow- happiness, liveness, curiosity
green- harmony, money
blue-patience, peace, trust, honor, professional
purple- nobility, wealth
pink- romance, affection
brown- relxation, confidenct, comfort, reliablity

무조건 아이콘을 사용해라- 모든내용을 함축시킬수있다
```

##### Spacing&Layout
```
whitespace를 줌으로써 페이지를 더 깔끔하고 보기 정갈하게 만들어준다
```
##### UX
>It' not just what it looks like and feels like. Design is how it work. -Steve Jobs 


-------------------------------------------------------------------------------------------------------------------

## HTML

#### 텍스트 관련 태그!
```
<h1>~<h6> 텍스트 굵기!
<h1>이 가장 큰 제목
<h6>이 가장 작은 제목

<p> 단락

<br> break 줄 바꿈

<hr> horizon 수평 줄 넣기 , css를 이용해 가로선 없애기 가능

<blockquote> 인용문 줄이 바뀌이어도 안으로 들여써짐 일반 텍스트보다 들여 써지므로 구별가능

<q> 인용문 줄바꿈없이 한줄로 표시 된다

<pre> 입력하는 그대로 화면에 표시하기 예를들면 공백을 넣어도 보여짐(소스코드 표기할때 좋음)

<strong> -굵게 강조할 텍스트(경고나 주의사항)

<b> - 굵게 표시할 텍스트(키워드)

<em> - 문장에서 특정부분 강조하고싶을때

<i> - 마음속 생각, 꿈, 기술적인 용어, 관용구에 사용 

<mark> -  형관펜 효과 내기. css로 배경색 바꾸기가능

<span>- 텍스트 단락 안에서 줄바꿈 없이 일부 텍스트만 묶어 스타일 적용할떄 사용

<abbr>-약자 표시

<cite>- 웹문서나 포스트에서 참고 내용표시

<code>- 컴퓨터 인식을 위한 소스코드

<kbd>- 키보드 입력내용 F5같은거

<small>- 부가정보 작게 표시할 때 사용

<sub>- 아래 첨자

<sup>- 위 첨자

<s> - 취소선

<u> - 밑줄

<a> anchor태그 - href=hypertext reference -링크 걸때
```

#### 목록을 만드는 태그!
```
<ul> - 순서가 필요하지 않은 목록을 만들때

<ol> - 순서 있는 목록	

<li> - <ul> 또는 <ol> 태그안에 사용해 각항목 표시

<dl> - 설명 목록

<dt> - 제목

<dd> - 설명

<nav>- 네비게이션(사이드바)

<section> 섹션 나눠주는 태그

<article> 뉴스기사이런거

<aside> 사이드바에 보통 사용많이함 

<header>, <footer> = 상단, 하단

<time>-시간을 나타내줄때 사용하는 태그
```

#### 표를 만드는 태그!
```
<th> - 제목 셀 (굵게 표시)

<tr> 열

<td> - 일반 셀

<td colspan="합칠 셀의개수"> - 가로로 합침

<td rowspan="합칠 셀의개수"> - 세로로 합침

<caption> - 표에 제목을 붙일 때 사용 <table>태그 바로 다음에 사용, 중앙에 바로 표시

<figcaption> - 표에 제목을 붙임 <figure>태그로 감싸고 제목 입력. 중앙에 정렬 XXX <table>태그 앞에 사용

<thead> - 표의 제목부분

<tbody> - 표의 본문 부분

<tfoot> - 표의 요약 부분
```

#### 그 외 태그들!
```
<img src="경로 및 파일이름">, alt 속성은 이미지에대한 설명

<a href="링크주소">

<input> type은 checkbox or radio

<fieldset>은 하나의 영역으로 묶고 외곽선을 그려구고 그룹에 제목(<legend>태그이용)을 붙여줄 수 있음

<label> input의 id 설정을 같이하면 <input>태그와 짝을 이룰 수있다.

<textarea> 글 작성할수있는 공간
```
-------------------------------------------------------------------------------------------------------------------

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
