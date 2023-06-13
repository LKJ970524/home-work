# mission-04 Grid README

## HTML코드

    <section class="news">
    <h2 class="title">새소식</h2>
      <article class="item">
        <h3 class="re">W3C 사이트가 리뉴얼 되었습니다.</h3>
        <p class="date">2022.07.18</p>
        <p class="brief">
          디자인 및 다양한 view 환경을 고려하여 구성되어 있으며,
          기존보다 최신 정보 및 개발자를 위한 기술 가이드도
          찾기 쉽도록 구성되어 있습니다.
        </p>
        <figure class="photo">
          <img src="news.gif" alt="W3C 리뉴얼">
          <figcaption>W3C 리뉴얼</figcaption>
        </figure>
      </article>
    <a href="/" class="more">더보기</a>
    </section>

## CSS 코드 및  설명

    /* 공통속성 */
    * {
    line-height: 150%;
    font-size: 14px;
    margin: 0;
    padding: 0;
    }

    a {
    text-decoration: none;
    color: inherit;
    }

section태그를 inline-block으로 바꿨습니다.

    .news {
    font-family: pretendard;
    margin-left: 30px;
    margin-top: 30px;
    position: relative;
    display: inline-block;
    }

가상요소를 주어 배경에 그라디언트 실선하나를 주고 위치에 맞게 배치하였습니다.

    .news::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 1px;
    background: #aaa linear-gradient(to right, #aaa, #fff);
    top: 35px;
    left: 0;
    }


relative와 inline-block으로 새소식과 더보기를 배치하였습니다.

    .title {
    font-weight: 700;
    color: #ed552f;
    }

    .more {
    position: absolute;
    top: -8px;
    right: -8px;
    padding: 8px;
    }


grid 속성을 사용하여 12열을 만들고 행은 auto로 주어 배치하였습니다.

    .item {
    width: 380px;
    height: auto;
    margin-top: 35px;
    position: relative;
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    grid-template-rows: auto;
    grid-template-areas: 
    "img re"  
    "img date"
    "img brief"
    ;
    }

    .re {
    font-weight: 700;
    margin-bottom: 10px;
    grid-area: re;
    }

    .date {
    grid-area: date;
    margin-bottom: 12px;
    }

    .photo {
    width: 112px;
    height: 66px;
    grid-area: img;
    padding-right: 30px;
    text-align: center;
    }

    .brief {
    margin-top: 10px;
    grid-area: brief;
    text-align: justify;
    width: 230px;
    }


이미지에 명암같은 효과가 있어 box-shadow효과로 처리하였습니다.

    .img {
    width: 112px;
    height: 66px;
    box-shadow: 0 15px 10px 5px #eee;
    margin-bottom: 15px;
    }