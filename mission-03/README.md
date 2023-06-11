# mission-03 README

<p align="center">
  <img src="https://github.com/LKJ970524/home-work/assets/115642699/9a3a7496-2cb2-4553-8c85-ca3745cd718c">
</p>

## HTML코드

    <div class="main">
    <h2 class="main-title">관련 <span class="site">사이트</span></h2>
    <ul class="main-list">
      <li><a href="/">제로베이스</a></li>
      <li><a href="/">MDN</a></li>
      <li><a href="/">웹접근성 연구소</a></li>
      <li><a href="/">Web Standards</a></li>
      <li><a href="/">W3C</a></li>
    </ul>
    </div>

## CSS코드

    .main {
      width: 190px;
      height: auto;
      margin-top: 50px;
      margin-left: 30px;
      border: 1px solid #A3A3A3;
      border-radius: 5px;
      padding: 8px 12px 12px 12px;
      background: linear-gradient(180deg, #CCCCCC 0%, #EEEEEE 100%);
      font-family: 'Pretendard';
    }

    .main-title {
      font-size: 15px;
      font-weight: 700;
    }

    .site { 
      color: #ED552F;
    }

    .main-list {
      margin-top: 10px;
      background: #fff;
      border: 1px solid #aaa;
      border-radius: 5px;
      height: 27px;
      overflow: hidden;
      transition: height .4s, padding .4s .4s;
    }

    .main-list:hover, .main-list:focus {
      height: 147px;
      padding: 10px 0;
    }

    li {
      font-style: normal;
      font-weight: 400;
      font-size: 14px;
    }

    .main-list a {
      display: block;
      line-height: 30px;  
      text-indent: 25px; /*들여쓰기*/
      text-decoration-line: none;
      color: black;
    }

### 코드설명
list 속성에 overflow: hidden 속성을 줘서 겹침 효과를 주었고 transition으로 아래로 스르륵 내려가는 효과를 주었습니다.

:hover와 :focus로 마우스가 focus될 때 아래로 얼마나 내려갈지 그리고 padding으로 내려간후 위아래가 조금씩 모아지도록 효과를 주었습니다.

a태그는 text-indent로 들여쓰기 효과를 넣어줬고 a태그로 글씨 작성시 밑줄이 그어지는 효과가 생겨 밑줄을 지워주는 코드를 적었습니다.