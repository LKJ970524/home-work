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

    