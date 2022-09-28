# 데이터 타입
ES6기준 자바스크립트는 7개의 데이터 타입을 갖는다. 


원시 타입
- 숫자
- 문자열
- 불리언
- unidentified
- null
- Symbol

객체 타입 : 객체, 함수 배열 등

&nbsp;  
### 숫자
**모든 수가 실수형이다.**  


```javascript
console.log(1 === 1.0);
//출력 결과 : true
```


&nbsp;  
ECMAScript 사양에 따라,   
메모리에 배정밀도 64비트 부동소수점 형식의 2진수로 저장된다.


&nbsp;  
**특수한 숫자 값**
- Infinity
- -Infinity
- Nan *Not-a-Number* : 산술 불가능한 값



&nbsp;  
### 문자열
문자열 연산자 '+'를 이용해 문자열을 결합할 수 있다.

따옴표는 ', ", `를 모두 사용할 수 있는데,-> '는 템플릿 리터럴인듯  
일반적으로 작은따옴표(')를 사용한다.  

자바스크립트 문자열은 자바와 달리 원시 타입이다.
자바와 마찬가지로 변경 불가능하다 *immutable* .

**[템플릿 리터럴]**  
ES6부터 추가되었다.  
`를 사용한다.  
런타임에 일반 문자열로 변환된다.
- **멀티라인 문자열** *multi-line String*  
일반 문자열과 달리 줄바꿈을 허용한다.

- **표현식 삽입** *expression interpolation*  
${}를 이용해 파이썬에서 했던 것처럼 문자열과 표현식을 결합할 수 있다.
    ```javascript
    var first = 'Ryan';
    var last = 'Reynolds';

    console.log(`My name is ${first} ${last}.`);
    //My name is Ryan Reynolds.
    ```

    ```javascript
    console.log(`1 + 2 = ${1 + 2}`);
    //1 + 2 = 3
    ```
- **태그드 템플릿** *tagged template*