# JavaScript Object

실제 생활에서 비유하자면 자동차는 하나의 객체이다

차의 속성은 무게 , 색깔 등이있고 , 메소드로 정의하자면 출발이나 정지 등이 있다.

Object도 마찬가지로 변수에 넣어서 정의할 수 있다

```JavaScript
var car = {type:"Fiat", model: "500" , color :"white"}
```



### Object Definition
예)
```JavaScript
var person = {firstName:"John",lastName:"Doe",age:50,eyeColor:"Blue"}
```


### 객체 속성 액세스

두가지 방법으로 액세스 할 수 있음

```
objectName.peroertyName

or

objectName["propertyName"]

예 1
person.lastName;

예 2

person["lastName"];
```

### Object Methods

오브젝트도 또한 메서드를 가질수 있다

```javascript
var person = {
    firstName : "John",
    lastName : "Doe",
    id : 5566,
    fullName : function() {
        return this.firstName + " " + this.lastName;
    }
}

```

### this keyword

정의된 함수에서 **this**는 함수의 "주인"을 의미합니다.

위의 예에서의 **this**는 fullName 함수의 "주인"인 person object를 의미한다

다시말하면 **this.firstName**은 이 오브젝트의 firstName 속성을 의미합니다.


### Accessing Object Methods

다음 구문처럼 메서드에 액세스할수있다.
```javascript
objectName.methodName()

예 1
name = person.fullName();
//John Doe 리턴 

예 2 
//()를 붙이지 않았을 경우
name = person.fullName;
// function() { return this.firstName + " " + this.lastName; } 리턴
```

### Do Not Declare Strings, Numbers, and Booleans as Objects!
When a JavaScript variable is declared with the keyword **"new"**, the variable is created as an object:

**new**를 사용하여 object형태로 Strings, Numbers, and Booleans을 선언하면 좋지않음.

```javascript
var x = new String();        // Declares x as a String object
var y = new Number();        // Declares y as a Number object
var z = new Boolean();       // Declares z as a Boolean object
```
Avoid **String**, **Number**, and **Boolean** objects. They complicate your code and slow down execution speed.