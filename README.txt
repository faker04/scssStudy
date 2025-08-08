# sass 컴파일 하기 

>npx sass ./scss:./css -w

# live sass compire 중지방법 
✅ 방법 2: 커맨드 팔레트에서 중지
Ctrl + Shift + P (또는 Cmd + Shift + P on Mac) → Command Palette 열기

Live Sass: Stop Watching Sass 검색

클릭해서 중지

→ 다시 시작하려면 Live Sass: Watch Sass 실행



--------------------------
변수에는 어떤 값 담을수 있다.
"값" 종류엔 여러가지 있음

#숫자 : + - * / 연산하기 위해 쓰이는 값
3px * 3px = 성립 안됨
3px * 3 = 9 성립됨

#문자: + 연산만 가능

-----------------------------
변수
다른파일 변수도 사용가능

변수 이름 규칙
- $ 로 시작 
- _-abcd(알파벳)1234567(숫자) 이렇게만 작성 가능, 다른 특수문자 불가능
- $로 시작하는데 $다음에 숫자는 안됨

#{} - interpolation 끼워넣기


-------------------------
sass-Partials(파셜)
소스에 반복되는 부분들을 분리 분산시켜서 모듈화 시키는 기능
@import @use @forward

파셜의 파일명은 _로 시작
Sass는 _로 시작하는 파일은 컴파일 하지 않음
불러들일때는 @import '파일명' (_,확장자 없이)

@use 변수중복 방지
ㄴ
  @use './var' as v2;
  @use './var2';











----------------------
home commit