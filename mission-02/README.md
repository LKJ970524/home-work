제일 큰상속자로 login을 주었고  제목은 h2태그를 이용해 login-title이라는 이름을 주었습니다.
실제 로그인 페이지라는것을 가정해 서버로 보내야하는 form태그를 이용했고 action은 아무동작 없게 만들었습니다.
아이디와 비밀번호를 분류해서 만들고 button태그를 이용해 로그인 버튼을 만들었고
아래의 회원가입은 form 태그가 아닌 div태그의 a태그로 작동하게 만들었습니다.


class=login;
login박스는 그라데이션 효과로 색상을 넣었고 모서리를 둥글게 만들었으며 box-shadow효과로 그림자 효과를 넣었습니다.


(h2) class=login-title
소제목인 '로그인'은 색상과 글자 사이즈15와 굵기700를 정했습니다.

class=login-form, sign
가운데 박스에 배경이 흰색이라 흰배경을 넣었습니다.

class=login-form
margin-top으로 제목과간격을주고 border-radius로 위쪽을 둥글게 만들었고 padding으로 내부 간격을 맞춰주었습니다.


login-form의 자식요소

fieldset : position relative로 요소를 배치하고 border-bottom으로 밑줄을 만들어주었습니다.

label : display를 inline-block으로바꿔주었습니다.

input : flex-direction row로 방향을 잡아주고 align-item center로 중아으로 잡아주고 border-radius로 둥글게 만들어 주었습니다.

login-button : position absolute로 요소를 제거하고 위치를 잡아주었습니다

class = sign(회원가입/아이디,비밀번호찾기)

sign : flex-flow로 정방향 한줄, 줄바꿈 금지로 만들었고 float를 줘 양옆으로 만들었습니다.