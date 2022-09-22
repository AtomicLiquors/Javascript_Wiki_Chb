[<<메인으로](https://github.com/AtomicLiquors/Javascript_Wiki_Chb)

&nbsp;  

# Node.js
2009, 라이언 달

```
크롬 V8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임 환경.  
```

&nbsp;  
Node.js는 브라우저 외부에 자바스크립트 실행환경을 제공한다.  
브라우저에서만 동작하던 자바스크립트를, 브라우저 외부에서 작동하게 해 준다.


&nbsp;  
## 설치
[공식 홈페이지](https://nodejs.org/ko/)에서 설치 후 터미널에서 버전 확인.
```
node -v
npm -v
```

&nbsp;  
## REPL
*Read Eval Print Loop*  
간단한 자바스크립트 코드를 실행해 결과를 확인할 수 있다.  

&nbsp;  
### 터미널
```
node
```

&nbsp;  
프롬프트가 >로 변경되면 코드를 실행할 수 있다.
```
Welcome to Node.js v16.17.0.
Type ".help" for more information.
> 1+2
3
> Math.max(1,2,3)
3
> [1,2,3].filter(v => v % 2)
[ 1, 3 ]
```


&nbsp;  
자바스크립트 파일 실행
```
node filename.js
```

&nbsp;  
### 종료 
Ctrl + C 두번


&nbsp;  



&nbsp;  