[<<메인으로](https://github.com/AtomicLiquors/Javascript_Wiki_Chb)

&nbsp;  

# typeof

- 값이 null인지 확인할 때는 ===를 사용해야 한다.   
    typeof로 null 값을 연산해보면 "null"이 아닌 "object"를 반환한다.  
이건 이유가 있어서 그런 게 아니라,   
자바스크립트 초판부터 있었던 버그다.

    기존 코드에 영향을 줄 수 있어 아직까지도 수정되지 않고 잇다.



- 선언하지 않은 식별자에 typeof를 사용하면,   
연산 결과는 ReferenceError가 아닌 undefined가 된다.