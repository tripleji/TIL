## JavaScript

#### Basic

```
1. Variables
var = 변수 선언할때 문제점이많아서 ES6 이후로 잘사용 X
let = 변수 선언하고 재선언하면 값을 바꿀 수 있다
const = 한번 선언하면 절대로 값을 바꿀 수 없다 undefined뜸

2. Types
primitivies/value type = String, Number, Boolean, undefined, null
referenced type = Object, Array, Function

3. Object 

형식
let person = {
    name: 'Ji',
    age: 27	
};

- Dot Notation -
peson.name = 'Lee'; 변경 가능

- Bracket Notation -
person['name] = 'Kim'; 변경가능

4. Array

형식
let color = ['red', 'blue'];

5. Function

형식
function greet() {
	console.log('Hellow World');
}

greet();
```

#### Operators
```
1. Arthimetic Operators

let x = 10;
let y = 3;
 
종류는 +,-,*,/,%,**

이경우에는 선처리
console.log(++x);  => 11

이경우에는 후처리
console.log(x++);  => 10
console.log(x); => 11

2. Assigntment Operators

let x = 10;
x = x + 5;  => x += 5;
x = x * 3; => x *= 3;

3. Comparison Operators

let x = 1;
console.log(x>0); true

4. Equality Operators

데이터 타입과 값이 같아야합
console.log(1 === 1);

데이터 타입 상관없이 값만!
console.log(1 == 1);

5. Ternary Operators

let points = 110;
let type =points > 100 ? 'gold' : 'silver' ;
참이면 골드 거짓이면 실버

6. Logical Operators with Non-booleans

let abcd = true;
let efgh = true;
let alphabet = abcd && efgh;

console.log(alphabet);  => true   &&는 둘다 참일때만 참이나옴
		        반대로 || 는 하나만 참이여도 참이나옴
```

#### Control Flow

```
1. if~else 

if(condition)
    console.log();
else if
    console.log();	

2. Switch~case

let role;

switch(role) {

case 'guest';
console.log('Guest User');
break;
}

3. For
Loops= For, While, Do..while, For..in, For..of

for(let i = 0; i < 5; i++){
   console.log('Hello World');  
}

4. While = 실행결과가 거짓이면 실행이 안된다

let i = 0;

while(i<5) {
if(condition) console.log(i);
i++;
}

5. Do-While = 실행결과가 거짓이어도 최소한번은 실행된다

let i = 0 ;
do{
if(condition) console.log(i);
i++;
}while (i<5);

6. infinite loops
여러가지 방식으로 무한루프 가능
(1) let i = 0;
    while (i < 5) {
    console.log(i);	
}

(2) while(true) {
}

(3) let x = 0; 
do {

} while (x<5);

for( let i = 0; i<10;)

7. function 2개 변수 리턴하는 형식

let number = max(5, 3);
console.log(number);

function max(a, b) {
    return (a>b) ? a : b;
}
```