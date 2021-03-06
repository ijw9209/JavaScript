# JavaScript Function 

자바스크립트 Function은 특정작업을 수행하도록 설계된 코드블록

ex1)
```JavaScript
function myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}
```


### JavaScript Function Syntax

```JavaScript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

### Function Invocation (함수 호출)
+ 이벤트 발생시
+ 자바스크립트 코드에서 호출될때
+ 자동(자기호출)


### Function Return

ex2)
```JavaScript
var x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}

//x의 결과 12

```

### Why Functions?

코드를 재사용 할 수 있다 : 한 번 코드를 정의하고 그것을 여러번 사용

다른결과를 생산하기위해 다른 인수와 동일한 코드를 여러 번 사용할 수 있음.

ex3)
섭씨 화씨 변환
```JavaScript
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius(77);
```

### The () Operator Invokes the Function

함수 결과 대신 함수의 정의를 반환함
ex4)
```JavaScript
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius;
```


### 변수 값으로 사용 기능

```JavaScript
// 대신 함수의 리턴값을 저장하는 변수를 사용 : 
var x = toCelsius(77);
var text = "The temperature is " + x + " Celsius";

// 변수 값으로 직접 기능을 사용할수도 있음
document.getElementById("demo").innerHTML = toCelsius;

```

### 지역 변수

지역변수는 선언된 함수내에서만 사용가능

ex5_Local Variables)

```JavaScript
// code here can NOT use carName

function myFunction() {
  var carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
```