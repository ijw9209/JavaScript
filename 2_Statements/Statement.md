# JavaScript Statement

### 자바스크립트 문

ex)
```JavaScript
document.getElementById("demo").innerHTML = "Hello Dolly.";
```


<hr>

### 세미콜론;

세미콜론은 자바스크립트 문을 구분합니다
```JavaScript
var a, b, c ;   // Declare 3 variables
a = 5;           // Assign the value 5 to a
b = 6;           // Assign the value 6 to b
c = a + b;       // Assign the sum of a and b to c

```

세미콜론으로 구분하면, 한 줄에 여러 개의 문이 허용됩니다 :

```JavaScript
a = 5; b = 6; c = a + b;
```

### 자바스크립트 공백

자바 스크립트는 여러 공백을 무시합니다.

```JavaScript
var person = "Hege";
var person="Hege";
```

### 자바 스크립트 라인의 길이와 줄 바꿈

최적의 가독성을 위해, 종종 같은 프로그래머는 80 자보다 긴 코드 라인을 방지 할 수 있습니다.

```JavaScript
document.getElementById("demo").innerHTML =
"Hello Dolly!";
```

### 자바 스크립트 코드 블록

자바 스크립트 문은 중괄호 {...} 내부 코드 블록에서 함께 그룹화 할 수 있습니다.
코드 블록의 목적은 함께 실행되는 문을 정의하는 것입니다.

```JavaScript
function myFunction() {
  document.getElementById("demo1").innerHTML = "Hello Dolly!";
  document.getElementById("demo2").innerHTML = "How are you?";
}
```