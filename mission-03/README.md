# mission-03 README

## 코드

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
      background: linear-gradient(180deg, #CCCCCC 0%, #EEEEEE 100%);;
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

