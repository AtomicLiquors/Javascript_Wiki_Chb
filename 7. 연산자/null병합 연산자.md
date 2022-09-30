[<<메인으로](https://github.com/AtomicLiquors/Javascript_Wiki_Chb)

&nbsp;  

# null 병합 연산자 "??"
ES11에서 도입되었다.
```
좌항의 피연산자가 *null*이나 *undefined*라면 우항을 반환한다.  
그렇지 않다면 좌항을 반환한다.
```

```javascript
var foo = null ?? 'default string';
console.log(foo); //좌항이 null이므로 우항의 'default string'을 출력.
```

&nbsp;  
### 활용
- 변수에 기본값 설정  
  
  앞서 '단축 평가'파트에서 본 것처럼 논리 곱 ||를 활용할 때는 허점이 있다.   
  Falsy 값인 0이나 ' '도 유효한 값이 될 수 있다면,   
  예기치 못한 동작이 발생할 수 있다는 것이다.  

  Before
  ```javascript
  var foo = '' || 'default string';
  console.log(foo); 
  //좌항에 들어온 ''도 엄연히 출력될 수 있는 문자열이다. 
  //하지만 Falsy값이라 기본값으로 넣은 default string이 출력된다.
  ```
  ```javascript
  //0이 들어간 예제 추가해라.
  ```

  After
  ```javascript
  var foo = '' ?? 'default string';
  console.log(foo); 
  //좌항에 ''를 넣으면 문자열 ''가 잘 출력된다.
  ```

