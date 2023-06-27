# mission-05 Sprite README

## 완성 이미지
<p align="center">
  <img src="https://github.com/LKJ970524/home-work/assets/115642699/52d7fd61-c0d8-4bd3-8679-83ec3b94b44a">
</p>

### HTML 코드

    <section class="favorite">
      <h2 class="title">인기 <span class="site">사이트</span></h2>
      <ol class="list">
        <li><a href="/">W3C</a><em class="up" aria-label="순위 상승"></em></li>
        <li><a href="/">Web Standards</a><em class="down" aria-label="순위 하락"></em></li>
        <li><a href="/">MDN</a><em class="stop" aria-label="순위 변동없음"></em></li>
        <li><a href="/">CSS ZenGarden</a><em class="up" aria-label="순위 상승"></em></li>
      </ol>
      <a href="/" class="more" title="인기 사이트">더보기</a>
    </section>

### CSS 코드 및 설명

    /* 메인박스 만들기 */
    .sprite{
      border: 1px solid #aaa;
      border-radius: 5px;
      background: #ccc linear-gradient(to bottom, #ccc, #eee);
      width: 190px;
      height: 147px;
      padding: 12px;
      margin-top: 20px;
      margin-left: 20px;
    }

    /* 제목 */
    .title{
      font-size: 15px;
      font-weight: 700;
      width: 166px;
      height: auto;
    }

    .site{
      color: #ed552f;
    }

겉 박스와 제목을 피그마에 적혀있는 코드를 보고 만들었습니다

    /* 더보기 배치 및 style 변경 */
    .more{
      position: absolute;
      top: 0;
      right: 0;
      padding: 12px;
    }

    a {
      text-decoration: none;
      color: inherit;
      font-size: 14px;
    }

position값을 absolute로 주어서 원하는 위치에 배치하도록 만들었습니다

    /* list 만들기 */
    .list{
      list-style: none;
      margin-top: 10px;
      counter-reset: number;
      padding-top: 4px;
    }
 
    .list li{
      counter-increment: number;
      margin-top: 8px;
      display: flex;
      align-items: center;
      font-size: 11px;
      padding: 2px;
    }

    .list li::before{
      content: counter(number);
      color: #fff;
      background-color: #aaa;
      border-radius: 5px;
      width: 16px;
      font-size: 11px;
      font-weight: 400;
      line-height: 150%;
      text-align: center;
      margin-right: 4px;
    }

list-style을 제거하고 counter-increment와 content로 li태그에 번호를 매겨 피그마에 있는 예제랑 비슷하게 구현하였습니다.

    /* 이미지 sprite */
    .list em{
      background: url("./rank.png") no-repeat;
      width: 9px;
      height: 11px;
      margin-left: auto;
    }

    .list .up {
      background-position: 0 0;
    }

    .list .stop{
      background-position: 0 -22px;
    }

    .list .down{
      background-position: 0 -44px;
    }

이미지 스프라이트 기법으로 a태그에 원하는 사진을 알맞게 배치하였습니다.