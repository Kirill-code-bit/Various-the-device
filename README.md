<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
  <style>
    *,
  *::after,
  *::before {
    padding: 0;
    margin: 0;
    list-style: none;
    text-decoration: none;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    -webkit-tap-highlight-color: transparent;
    scroll-behavior: smooth;
  }
  
  html {
    scroll-behavior: smooth;
  }
  
  body {
    scroll-behavior: smooth;
  }
  
  body {
    background-color: var(--bg-color);
  }
  
  .container {
    padding: 0 60px;
    margin: 0 auto;
    width: 100%;
    max-width: 1440px;
  }
  
  :root {
    --link-active-color: #118da8;
    --link-color: #ffffff;
    --bg-color: #191919;
    --section-bg-color: #000000;
    --star-color: #fcff51;
  }
  
  ::-webkit-scrollbar {
    width: 15px;
  }
  
  ::-webkit-scrollbar-thumb {
    border-radius: 10px;
    cursor: pointer;
    background-color: var(--section-bg-color);
  }
  /* ****BASIC TO THE CODES END**** */
  
  /* ****SECRET NAVBAR**** */
  .secret__navbar {
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    position: fixed;
    z-index: 2;
    top: 0;
    right: 0;
    -webkit-transform: translateY(-100%);
    -ms-transform: translateY(-100%);
    transform: translateY(-100%);
    -webkit-transition: all 0.5s linear;
    -o-transition: all 0.5s linear;
    transition: all 0.5s linear;
  }
  
  .secret__navbar.active {
    -webkit-transform: translateY(0);
    -ms-transform: translateY(0);
    transform: translateY(0);
  }
  
  .secret__navbar__list {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    height: 0%;
    min-height: 100%;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
  }
  
  .secret__navbar__list .secret__navbar__item .secret__navbar__link {
    color: var(--link-color);
    font-size: 35px;
    line-height: 50px;
    text-align: center;
    font-family: sans-serif;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
  }
  
  .secret__navbar__list .secret__navbar__item .secret__navbar__link:hover {
    color: var(--link-active-color);
  }
  /* ****SECRET NAVBAR END**** */
  
  /* ****HEADER START**** */
  .header {
    background-color: var(--bg-color);
    height: 119px;
    width: 100%;
    position: sticky;
    top: 0;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
    z-index: 1;
  }
  
  .header.active {
    height: 75px;
    background-color: var(--link-color);
  }
  
  .header.active .nav .nav__list .nav__item .nav__link {
    color: var(--bg-color);
    font-weight: 600;
  }
  
  .header.active .nav .nav__list .nav__item .nav__link:hover {
    color: var(--link-active-color);
  }
  
  .header.active .nav__intro {
    color: var(--bg-color);
  }
  
  .header.active .nav .nav__list .nav__item .nav__link.active {
    color: var(--link-active-color);
  }
  
  .header.active .nav {
    background-color: var(--link-color);
    height: 75px;
  }
  /* ****HEADER END**** */
  
  /* ****NAV START**** */
  .nav {
    background-color: var(--bg-color);
    max-width: 1200px;
    height: 119px;
    width: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
  }
  
  .nav__intro {
    color: var(--link-color);
    font-family: sans-serif;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
  }
  
  .nav .nav__list .nav__item {
    display: inline-block;
    padding: 0 20px;
  }
  
  .nav .nav__list .nav__item .nav__link.active {
    color: var(--link-active-color);
  }
  
  .nav .nav__list .nav__item .nav__link {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 17px;
    color: var(--link-color);
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
  }
  
  .nav .nav__list .nav__item .nav__link:hover {
    color: var(--link-active-color);
  }
  
  .header.active .fa-bars {
    color: var(--link-active-color);
  }
  
  .fa-bars {
    font-size: 30px;
    color: var(--link-color);
    cursor: pointer;
    display: none;
  }
  
  .fa-times {
    font-size: 30px;
    color: var(--link-color);
    position: fixed;
    right: 55px;
    top: 45px;
    cursor: pointer;
  }
  /* ****NAV END**** */
  
  /* ****MAIN START**** */
  .main {
    margin: 43px 0 0 0;
  }
  
  .main__container {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    gap: 60px;
  }
  
  .main__box.active {
    margin: 300px 0 0 0;
  }
  
  .main__box_img {
    height: 873px;
    width: 650px;
    -o-object-fit: cover;
    object-fit: cover;
    border-radius: 16px;
  }
  
  .main__box_title {
    max-width: 535px;
    width: 100%;
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 70px;
    line-height: 88px;
    color: var(--link-color);
    letter-spacing: 3.2px;
  }
  
  .main__box_icon {
    margin: 90px 0 0 0;
  }
  
  .main__box_icons_paragraph {
    font-family: sans-serif;
    letter-spacing: 1px;
    font-style: normal;
    font-weight: 400;
    font-size: 15px;
    line-height: 24px;
    color: var(--link-color);
    margin: 0 0 16px 0;
  }
  
  .main__box_icons {
    gap: 17px;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  
  .main__box_icons_img {
    height: 32px;
    width: 32px;
    border-radius: 50%;
  }
  /* ****MAIN END**** */
  
  /* ****SECTION START****  */
  .section__content {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    margin: 93px 0 66px 0;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  
  .section__content_title {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 64px;
    line-height: 79px;
    color: var(--link-color);
    letter-spacing: 2.88px;
  }
  
  .section__content_link {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 17px;
    background-color: var(--link-active-color);
    display: block;
    width: 178px;
    height: 51px;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    border-radius: 6px;
    color: var(--link-color);
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
    border: 1px solid var(--link-active-color);
  }
  
  .section__content_link:hover {
    background-color: var(--bg-color);
    color: var(--link-active-color);
  }
  
  .section__container {
    border-radius: 32px;
    background-color: var(--section-bg-color);
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    padding: 40px 0 40px 40px;
    gap: 53px;
    min-height: 545px;
    max-width: 1300px;
    width: 100%;
    margin: 60px 0;
  }
  
  .section__box_img {
    height: 465px;
    width: 389px;
  }
  
  .section__box_img.active {
    width: 389px;
    height: 432px;
  }
  
  .section__box_content_bold {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 27px;
    color: var(--link-color);
    background-color: var(--bg-color);
    margin: 8px 0 0 0;
    width: 73px;
    height: 27px;
    border-radius: 6px;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  
  .section__box_content_bold.active {
    width: 136px;
    height: 27px;
  }
  
  .section__box_content_blue {
    color: var(--link-active-color);
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 17px;
    line-height: 27px;
    margin: 48px 0 18px 0;
  }
  
  .section__box_content_title {
    font-family: sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 64px;
    line-height: 70px;
    color: var(--link-color);
    width: 100%;
    max-width: 701px;
    letter-spacing: 2.56px;
  }
  
  .section__box_content_title.active {
    max-width: 650px;
    width: 100%;
  }
  
  .section__box_content_paragraph {
    font-family: sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 33px;
    color: rgba(255, 255, 255, 0.7);
    margin: 28px 0 18px 0;
    max-width: 757px;
    width: 100%;
  }
  
  .section__box_content_link {
    font-family: sans-serif;
    font-style: normal;
    letter-spacing: 0.5px;
    font-weight: 400;
    font-size: 18px;
    line-height: 27px;
    color: var(--link-color);
    background-color: var(--link-active-color);
    width: 208px;
    height: 51px;
    border-radius: 6px;
    display: block;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
    border: 1px solid var(--link-active-color);
  }
  
  .section__box_content_link:hover {
    background-color: var(--section-bg-color);
    color: var(--link-active-color);
  }
  
  .section__contact {
    margin: 260px 0 0 0;
  }
  
  .section__contact_container {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    gap: 94px;
  }
  
  .section__contact_box_icon {
    height: 112px;
    width: 112px;
    border-radius: 50%;
  }
  
  .section__contact_box_link {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    height: 27px;
    display: block;
    max-width: 140px;
    width: 100%;
    line-height: 27px;
    color: var(--link-active-color);
    margin: 20px 0 25px 0;
  }
  
  .section__contact_box_title {
    font-family: sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 65px;
    line-height: 79px;
    color: var(--link-color);
    letter-spacing: 2.88px;
    margin: 0 0 28px 0;
  }
  
  .section__contact_box_paragraph {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 33px;
    color: rgba(255, 255, 255, 0.7);
    max-width: 570px;
    width: 100%;
  }
  
  .section__contact_box_paragraph.active {
    margin: 33px 0 0 0;
  }
  
  .section__contact_box_img {
    max-width: 575px;
    border-radius: 14px;
    -o-object-fit: cover;
    object-fit: cover;
    height: 743px;
  }
  
  .section__form_container {
    min-height: 350px;
    max-width: 1300px;
    width: 100%;
    margin: 200px 0 0 0;
    background-color: var(--section-bg-color);
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    padding: 60px;
    border-radius: 32px;
  }
  
  .section__form_box_link {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 27px;
    color: var(--link-active-color);
  }
  
  .section__form_box_title {
    font-family: sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 72px;
    line-height: 79px;
    color: var(--link-color);
    max-width: 431px;
    width: 100%;
    letter-spacing: 2.88px;
  }
  
  .form {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
  }
  
  .form__input {
    font-family: "DM Sans";
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    width: 522px;
    outline: none;
    padding: 13px;
    color: rgba(255, 255, 255, 0.7);
    background: var(--bg-color);
    border: 1px solid var(--bg-color);
    border-radius: 6px;
    margin: 10px 0;
  }
  
  .form__submit {
    height: 48px;
    width: 87px;
    background: var(--link-active-color);
    border-radius: 6px;
    cursor: pointer;
    font-family: sans-serif;
    margin: 10px 0 0 0;
    border-radius: 6px;
    font-style: normal;
    font-weight: 700;
    font-size: 15px;
    line-height: 29px;
    color: rgba(255, 255, 255, 0.7);
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
    border: 1px solid var(--link-active-color);
  }
  
  .form__submit:hover {
    background-color: transparent;
    color: var(--link-active-color);
  }
  
  .section__user_container {
    display: -ms-grid;
    display: grid;
    -ms-grid-columns: auto 16px auto 16px auto;
    grid-template-columns: repeat(3, auto);
    gap: 16px;
    margin: 200px 0 0 0;
  }
  
  .section__user_box {
    height: 321px;
    max-width: 423px;
    width: 100%;
    background-color: var(--section-bg-color);
    border-radius: 32px;
    padding: 50px;
  }
  
  .fa-star {
    color: var(--star-color);
    margin: 18px 0 20px 0;
  }
  
  .section__user_box_title {
    font-family: sans-serif;
    color: var(--link-color);
    font-style: normal;
    font-weight: 400;
    font-size: 26px;
    line-height: 40px;
    margin: 18px 0 20px 0;
  }
  
  .section__user_box_paragraph {
    font-family: sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 23px;
    line-height: 29px;
    color: rgba(255, 255, 255, 0.7);
  }
  /* ****SECTION END**** */
  
  /* ****FOOTER START**** */
  .footer {
    margin: 200px 0 0 0;
    display: -ms-grid;
    display: grid;
    -ms-grid-columns: (auto);
    grid-template-columns: repeat(3, auto);
    height: 292px;
  }
  
  .footer__container {
    display: -ms-grid;
    display: grid;
    -ms-grid-columns: auto 146px auto 146px auto;
    grid-template-columns: repeat(3, auto);
    gap: 146px;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
  }
  
  .footer__container_box_title {
    color: var(--link-color);
    font-family: sans-serif;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    margin: 0 0 25px 0;
  }
  
  .footer__box .footer__box_item {
    padding: 5px 0;
  }
  
  .footer__container_box_icons i {
    color: var(--link-color);
    width: 22px;
    height: 17.94px;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
    cursor: pointer;
  }
  
  .footer__container_box_icons i:hover {
    color: var(--link-active-color);
  }
  
  .footer__box .footer__box_item .footer__box_link {
    font-family: sans-serif;
    color: var(--link-color);
    font-style: normal;
    font-weight: 400;
    font-size: 17px;
    line-height: 27px;
    -webkit-transition: all 0.3s linear;
    -o-transition: all 0.3s linear;
    transition: all 0.3s linear;
  }
  
  .footer__box .footer__box_item .footer__box_link:hover {
    color: var(--link-active-color);
    text-decoration: underline;
  }
  
  .footer__box_img {
    padding: 0 8.5px;
    border-radius: 50%;
  }
  /* ****FOOTER END**** */
  
  /* ****MEDIA RESPONSIVE START**** */
 





  
  @media (max-width: 1320px) {
    .main__container {
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      gap: 60px;
    }
  
    .main__container {
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      gap: 0;
    }
  
    .main__box_img {
      display: none;
    }
  
    .main__box.active {
      margin: 200px 0 100px 0;
    }
  
    .section__contact_box_img {
      display: none;
    }
  
    .section__contact {
      margin: 200px 0 0 0;
    }
  }
  
  @media (max-width: 1300px) {
    .section__user_container {
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: auto 16px auto;
      grid-template-columns: repeat(2, auto);
      gap: 16px;
      margin: 200px 0 0 0;
      -webkit-box-pack: center;
      -ms-flex-pack: center;
      justify-content: center;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 40px 0 40px 40px;
      gap: 0;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  }
  
  @media (max-width: 1290px) {
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 40px 0 40px 40px;
      gap: 0;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  
    .section__box_img {
      display: none;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      -webkit-box-pack: start;
      -ms-flex-pack: start;
      justify-content: flex-start;
      padding: 40px 0 40px 40px;
      gap: 53px;
      min-height: 545px;
      width: 1300px;
      margin: 60px 0;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 40px 0 40px 40px;
      gap: 0;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 40px 0 40px 40px;
      gap: 53px;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  }
  
  @media (max-width: 1192px) {
    .section__form_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 72px;
      line-height: 79px;
      color: var(--link-color);
      max-width: 431px;
      width: 100%;
      letter-spacing: 2.88px;
      margin: 0 0 50px 0;
    }
  }
  
  @media (max-width: 1100px) {
    .footer {
      margin: 200px 0 0 0;
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: (auto);
      grid-template-columns: repeat(1, auto);
      height: 292px;
      -webkit-box-pack: start;
      -ms-flex-pack: start;
      justify-content: flex-start;
    }
  
    .footer__container {
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: auto;
      grid-template-columns: repeat(1, auto);
      gap: 146px;
      -webkit-box-pack: start;
      -ms-flex-pack: start;
      justify-content: flex-start;
    }
  
    .footer__container_box_icons i {
      color: var(--link-color);
      width: 22px;
      height: 17.94px;
      -webkit-transition: all 0.3s linear;
      -o-transition: all 0.3s linear;
      transition: all 0.3s linear;
      cursor: pointer;
      margin: 0 0 25px 0;
    }
  }
  
  @media (max-width: 960px) {
    .section__box_content_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 50px;
      line-height: 60px;
      color: var(--link-color);
      width: 100%;
      max-width: 701px;
      letter-spacing: 2.56px;
    }
  
    .section__box_content_paragraph {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 20px;
      line-height: 33px;
      color: rgba(255, 255, 255, 0.7);
      margin: 28px 0 18px 0;
      max-width: 757px;
      width: 100%;
    }
  }
  
  @media (max-width: 930px) {
    .section__user_container {
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: auto;
      grid-template-columns: repeat(1, auto);
      gap: 16px;
      margin: 200px 0 0 0;
      -webkit-box-pack: center;
      -ms-flex-pack: center;
      justify-content: center;
    }
  }
  
  @media (max-width: 858px) {
    .section__content_title {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 40px;
      line-height: 79px;
      color: var(--link-color);
      letter-spacing: 2.88px;
    }
  
    .section__content_link {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 17px;
      background-color: var(--link-active-color);
      display: block;
      max-width: 178px;
      width: 100%;
      height: 51px;
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      -webkit-box-pack: center;
      -ms-flex-pack: center;
      justify-content: center;
      -webkit-box-align: center;
      -ms-flex-align: center;
      align-items: center;
      border-radius: 6px;
      color: var(--link-color);
      -webkit-transition: all 0.3s linear;
      -o-transition: all 0.3s linear;
      transition: all 0.3s linear;
      border: 1px solid var(--link-active-color);
    }
  
    .section__content {
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      -webkit-box-pack: start;
      -ms-flex-pack: start;
      justify-content: flex-start;
      -ms-flex-wrap: wrap;
      flex-wrap: wrap;
      margin: 93px 0 66px 0;
      -webkit-box-align: center;
      -ms-flex-align: center;
      align-items: center;
    }
  }
  
  @media (max-width: 600px) {
    .main__box_title {
      max-width: 535px;
      width: 100%;
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 40px;
      line-height: 70px;
      color: var(--link-color);
      letter-spacing: 3.2px;
    }
  }
  
  @media (max-width: 655px) {
    .main__box.active {
      margin: 100px 0 0 0;
    }
  
    .main__box_title {
      max-width: 535px;
      width: 100%;
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 60px;
      line-height: 88px;
      color: var(--link-color);
      letter-spacing: 3.2px;
    }
  }
  
  @media (max-width: 768px) {
    .nav .nav__list .nav__item .nav__link {
      display: none;
    }
  
    .fa-bars {
      display: block;
    }
  }
  
  @media (max-width: 715px) {
    .form__input {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 24px;
      width: 400px;
      outline: none;
      padding: 13px;
      color: rgba(255, 255, 255, 0.7);
      background: var(--bg-color);
      border: 1px solid var(--bg-color);
      border-radius: 6px;
      margin: 10px 0;
    }
  
    .section__form_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 50px;
      line-height: 60px;
      color: var(--link-color);
      max-width: 431px;
      width: 100%;
      letter-spacing: 2.88px;
      margin: 0 0 25px 0;
    }
  
    .section__user_container {
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: auto;
      grid-template-columns: repeat(1, auto);
      gap: 16px;
      margin: 100px 0 0 0;
      -webkit-box-pack: center;
      -ms-flex-pack: center;
      justify-content: center;
    }
  
    .section__form_container {
      min-height: 350px;
      max-width: 1300px;
      width: 100%;
      margin: 100px 0 0 0;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      -ms-flex-wrap: wrap;
      flex-wrap: wrap;
      -webkit-box-pack: justify;
      -ms-flex-pack: justify;
      justify-content: space-between;
      padding: 30px;
      border-radius: 32px;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 40px 0 40px 40px;
      gap: 0;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  }
  
  @media (max-width: 560px) {
    .form__input {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 24px;
      width: 350px;
      outline: none;
      padding: 13px;
      color: rgba(255, 255, 255, 0.7);
      background: var(--bg-color);
      border: 1px solid var(--bg-color);
      border-radius: 6px;
      margin: 10px 0;
    }
  }
  
  @media (max-width: 555px) {
    .container {
      padding: 0 50px;
      margin: 0 auto;
      width: 100%;
      max-width: 1440px;
    }
  
    .section__box_content_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 40px;
      line-height: 60px;
      color: var(--link-color);
      width: 100%;
      max-width: 701px;
      letter-spacing: 2.56px;
    }
  
    .section__contact_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 50px;
      line-height: 79px;
      color: var(--link-color);
      letter-spacing: 2.88px;
      margin: 0 0 28px 0;
    }
  
    .section__form_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 30px;
      line-height: 60px;
      color: var(--link-color);
      max-width: 431px;
      width: 100%;
      letter-spacing: 2.88px;
      margin: 0 0 25px 0;
    }
  
    .form__submit {
      height: 48px;
      max-width: 87px;
      width: 100%;
      background: var(--link-active-color);
      border-radius: 6px;
      cursor: pointer;
      font-family: sans-serif;
      margin: 10px 0 0 0;
      border-radius: 6px;
      font-style: normal;
      font-weight: 700;
      font-size: 15px;
      line-height: 29px;
      color: rgba(255, 255, 255, 0.7);
      -webkit-transition: all 0.3s linear;
      -o-transition: all 0.3s linear;
      transition: all 0.3s linear;
      border: 1px solid var(--link-active-color);
    }
  }
  
  @media (max-width: 514px) {
    .form__input {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 24px;
      max-width: 350px;
      outline: none;
      width: 100%;
      padding: 13px;
      color: rgba(255, 255, 255, 0.7);
      background: var(--bg-color);
      border: 1px solid var(--bg-color);
      border-radius: 6px;
      margin: 10px 0;
    }
  
    .section__user_box {
      min-height: 380px;
      max-width: 423px;
      width: 100%;
      background-color: var(--section-bg-color);
      border-radius: 32px;
      padding: 50px;
    }
  }
  
  @media (max-width: 475px) {
    .section__content_title {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 30px;
      line-height: 79px;
      color: var(--link-color);
      letter-spacing: 2.88px;
    }
  
    .section__user_box {
      min-height: 380px;
      max-width: 423px;
      width: 100%;
      background-color: var(--section-bg-color);
      border-radius: 32px;
      padding: 50px;
    }
  }
  
  @media (max-width: 415px) {
    .container {
      padding: 0 20px;
      margin: 0 auto;
      width: 100%;
      max-width: 1440px;
    }
  
    .section__user_box {
      min-height: 380px;
      max-width: 423px;
      width: 100%;
      background-color: var(--section-bg-color);
      border-radius: 32px;
      padding: 50px;
    }
  }
  
  @media (max-width: 400px) {
    .container {
      padding: 0 15px;
      margin: 0 auto;
      width: 100%;
      max-width: 1440px;
    }
  
    .main__box_title {
      max-width: 535px;
      width: 100%;
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 30px;
      line-height: 45px;
      color: var(--link-color);
      letter-spacing: 3.2px;
    }
  
    .section__content_title {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 25px;
      line-height: 79px;
      color: var(--link-color);
      letter-spacing: 2.88px;
    }
  
    .main__box.active {
      margin: 50px 0 0 0;
    }
  
    .section__box_content_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 25px;
      line-height: 40px;
      color: var(--link-color);
      width: 100%;
      max-width: 701px;
      letter-spacing: 2.56px;
    }
  
    .section__container {
      border-radius: 32px;
      background-color: var(--section-bg-color);
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      padding: 20px;
      gap: 0;
      min-height: 545px;
      max-width: 1135px;
      width: 100%;
      margin: 60px 0;
    }
  
    .section__box_content_paragraph {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 15px;
      line-height: 33px;
      color: rgba(255, 255, 255, 0.7);
      margin: 28px 0 18px 0;
      max-width: 757px;
      width: 100%;
    }
  
    .section__box_content_link {
      font-family: sans-serif;
      font-style: normal;
      letter-spacing: 0.5px;
      font-weight: 400;
      font-size: 15px;
      line-height: 27px;
      color: var(--link-color);
      background-color: var(--link-active-color);
      width: 208px;
      height: 51px;
      border-radius: 6px;
      display: block;
      display: -webkit-box;
      display: -ms-flexbox;
      display: flex;
      -webkit-box-pack: center;
      -ms-flex-pack: center;
      justify-content: center;
      -webkit-box-align: center;
      -ms-flex-align: center;
      align-items: center;
      -webkit-transition: all 0.3s linear;
      -o-transition: all 0.3s linear;
      transition: all 0.3s linear;
      border: 1px solid var(--link-active-color);
    }
  
    .section__contact_box_icon {
      height: 75px;
      width: 75px;
      border-radius: 50%;
    }
  
    .section__contact_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 30px;
      line-height: 50px;
      color: var(--link-color);
      letter-spacing: 2.88px;
      margin: 0 0 25px 0;
    }
  
    .section__contact_box_paragraph {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 18px;
      line-height: 33px;
      color: rgba(255, 255, 255, 0.7);
      max-width: 570px;
      width: 100%;
    }
  
    .section__form_box_title {
      font-family: sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 25px;
      line-height: 40px;
      color: var(--link-color);
      max-width: 431px;
      width: 100%;
      letter-spacing: 2.88px;
      margin: 0 0 25px 0;
    }
  
    .form__input {
      font-family: "DM Sans";
      font-style: normal;
      font-weight: 400;
      font-size: 18px;
      max-width: 350px;
      outline: none;
      width: 100%;
      padding: 13px;
      color: rgba(255, 255, 255, 0.7);
      background: var(--bg-color);
      border: 1px solid var(--bg-color);
      border-radius: 6px;
      margin: 10px 0;
    }
  
    .section__user_box_title {
      font-family: sans-serif;
      color: var(--link-color);
      font-style: normal;
      font-weight: 400;
      font-size: 20px;
      line-height: 43px;
      margin: 21px 0 19px 0;
    }
  
    .footer__container {
      display: -ms-grid;
      display: grid;
      -ms-grid-columns: auto;
      grid-template-columns: repeat(1, auto);
      gap: 5px;
      -webkit-box-pack: start;
      -ms-flex-pack: start;
      justify-content: flex-start;
    }
  
    .footer {
      margin: 150px 0 0 0;
    }
  
    .nav__intro {
      color: var(--link-color);
      font-family: sans-serif;
      font-size: 25px;
      font-style: normal;
      font-weight: 600;
    }
  }
    </style>
<body>
    <div class="secret__navbar">
        <i class="fa fa-times"></i>
        <ul class="secret__navbar__list">
          <li class="secret__navbar__item">
            <a class="secret__navbar__link" href="#"> Home </a>
          </li>
          <li class="secret__navbar__item">
            <a class="secret__navbar__link" href="#Episodes"> Episodes </a>
          </li>
          <li class="secret__navbar__item">
            <a class="secret__navbar__link" href="#About"> About </a>
          </li>
          <li class="secret__navbar__item">
            <a class="secret__navbar__link" href="#Contact"> Contact </a>
          </li>
        </ul>
      </div>
      <!-- *****SECRET NAVBAR END***** -->
  
      <!-- ****HEADER START**** -->
      <header class="header">
        <div class="container">
          <nav class="nav">
            <a class="nav__intro" href="index.html">Castaway</a>
            <ul class="nav__list">
              <li class="nav__item">
                <a class="nav__link active" href="#">Home</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#Episodes">Episodes</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#About">About</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#Contact">Contact</a>
              </li>
            </ul>
            <i class="fa fa-bars"></i>
          </nav>
        </div>
      </header>
      <!-- ****HEADER END -->
  
      <!-- ****MAIN START**** -->
      <div class="container">
        <main class="main">
          <div class="main__container">
            <div
              class="main__box"
              data-aos="zoom-in"
              data-aos-duration="800"
              data-aos-delay="100"
            >
              <img
                class="main__box_img"
                src="./svg/main-img.jpg"
                alt="main-img"
              />
            </div>
            <div
              class="main__box active"
              data-aos="zoom-in"
              data-aos-duration="800"
              data-aos-delay="100"
            >
              <h1 class="main__box_title">Take your podcast to the</h1>
              <h1 class="main__box_title">next level</h1>
              <div class="main__box_icon">
                <p class="main__box_icons_paragraph">Listen on</p>
                <div class="main__box_icons">
                  <img
                    class="main__box_icons_img"
                    src="svg/icon1.png"
                    alt="icon1"
                  />
                  <img
                    class="main__box_icons_img"
                    src="svg/icon2.png"
                    alt="icon2"
                  />
                  <img
                    class="main__box_icons_img"
                    src="svg/icon3.png"
                    alt="icon3"
                  />
                  <img
                    class="main__box_icons_img"
                    src="svg/icon4.png"
                    alt="icon4"
                  />
                  <img
                    class="main__box_icons_img"
                    src="svg/icon5.png"
                    alt="icon5"
                  />
                </div>
              </div>
            </div>
          </div>
        </main>
      </div>
      <!-- ****MAIN END**** -->
  
      <!-- ****SECTION START**** -->
      <div class="container">
        <section class="section" id="Episodes">
          <div class="section__content">
            <h1 class="section__content_title">Latest episodes</h1>
            <a class="section__content_link" href="#"> View all episodes </a>
          </div>
          <div class="section__container">
            <div
              class="section__box"
              data-aos="fade-down"
              data-aos-duration="800"
              data-aos-delay="200"
            >
              <img
                class="section__box_img"
                src="./svg/section-img1.jpg"
                alt="section-img1"
              />
            </div>
            <div class="section__box">
              <div
                class="section__box_content"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <p class="section__box_content_bold">Gear</p>
                <p class="section__box_content_blue">Episode 3</p>
                <h1 class="section__box_content_title">
                  Should you get outboard audio gear?
                </h1>
                <p class="section__box_content_paragraph">
                  Is hardware really worth it when it comes to podcasting? The
                  answer is...it depends. Here’s our reasons on why you might want
                  to consider picking something up.
                </p>
                <a href="#" class="section__box_content_link">
                  View Episode Details
                </a>
              </div>
            </div>
          </div>
  
          <div class="section__container">
            <div
              class="section__box"
              data-aos="fade-down"
              data-aos-duration="800"
              data-aos-delay="200"
            >
              <img
                class="section__box_img active"
                src="./svg/section-img2.jpg"
                alt="section-img1"
              />
            </div>
            <div class="section__box">
              <div
                class="section__box_content"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <p class="section__box_content_bold active">Tips & Tricks</p>
                <p class="section__box_content_blue">Episode 2</p>
                <h1 class="section__box_content_title active">
                  Mic tricks to take you to the next level
                </h1>
                <p class="section__box_content_paragraph">
                  Stop rolling with those default settings on your mic. These
                  small tweaks will take you from sounding good to great.
                </p>
                <a href="#" class="section__box_content_link">
                  View Episode Details
                </a>
              </div>
            </div>
          </div>
  
          <div class="section__container">
            <div
              class="section__box"
              data-aos="fade-down"
              data-aos-duration="800"
              data-aos-delay="200"
            >
              <img
                class="section__box_img active"
                src="./svg/section-img3.jpg"
                alt="section-img3"
              />
            </div>
            <div class="section__box">
              <div
                class="section__box_content"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <p class="section__box_content_bold">Gear</p>
                <p class="section__box_content_blue">Episode 1</p>
                <h1 class="section__box_content_title active">
                  The best microphone under $200
                </h1>
                <p class="section__box_content_paragraph">
                  With so many microphones on the market, how are you supposed to
                  know what’s the best? Take a look at our top picks.
                </p>
                <a href="#" class="section__box_content_link">
                  View Episode Details
                </a>
              </div>
            </div>
          </div>
        </section>
      </div>
  
      <div class="container">
        <section class="section" id="About">
          <div class="section__contact">
            <div class="section__contact_container">
              <div
                class="section__contact_box"
                data-aos="zoom-in"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <img
                  class="section__contact_box_icon"
                  src="svg/1670770892_grizly-club-p-strelka-vpravo-png-19.jpg"
                  alt="right-icon"
                />
                <a class="section__contact_box_link" href="#">Meet your host</a>
                <h1 class="section__contact_box_title">Jacob Paulaner</h1>
                <p class="section__contact_box_paragraph">
                  Jacob has a background in audio engineering, and has been
                  podcasting since the early days.
                </p>
                <p class="section__contact_box_paragraph active">
                  He’s here to help you level up your game by sharing everything
                  he’s learned along the way.
                </p>
              </div>
              <div
                class="section__contact_box"
                data-aos="zoom-in"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <img
                  class="section__contact_box_img"
                  src="svg/02-_1_650x650.webp"
                  alt="contact-img"
                />
              </div>
            </div>
          </div>
        </section>
      </div>
  
      <div class="container">
        <section class="section" id="Contact">
          <div
            class="section__form"
            data-aos="flip-left"
            data-aos-duration="800"
            data-aos-delay="200"
          >
            <div class="section__form_container">
              <div class="section__form_box">
                <a class="section__form_box_link" href="#"> Email Newsletter </a>
                <h1 class="section__form_box_title">Subscribe for updates</h1>
              </div>
              <div class="section__form_box">
                <form class="form">
                  <input
                    class="form__input"
                    type="text"
                    placeholder="Name"
                    required
                  />
                  <input
                    class="form__input"
                    type="email"
                    placeholder="Email"
                    required
                  />
                  <input class="form__submit" type="submit" value="Submit" />
                </form>
              </div>
            </div>
          </div>
        </section>
      </div>
  
      <div class="container">
        <section class="section">
          <div class="section__user">
            <div class="section__user_container">
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <h1 class="section__user_box_title">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <br>
                  I can’t recommend this podcast enough
                </h1>
                <p class="section__user_box_paragraph">Betty Lacey</p>
              </div>
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <h1 class="section__user_box_title">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <br>
                  Jacob is the best in the business
                </h1>
                <p class="section__user_box_paragraph">Adam Driver</p>
              </div>
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <h1 class="section__user_box_title">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <br>
                  A wealth of audio knowledge
                </h1>
                <p class="section__user_box_paragraph">Marcus Brown</p>
              </div>
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                <h1 class="section__user_box_title">Every episode is a gem!</h1>
                <p class="section__user_box_paragraph">Jessica Knowl</p>
              </div>
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <h1 class="section__user_box_title">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <br>
                  Whoa whoa, let me take some notes!
                </h1>
                <p class="section__user_box_paragraph">Scott Adams</p>
              </div>
              <div
                class="section__user_box"
                data-aos="fade-down"
                data-aos-duration="800"
                data-aos-delay="200"
              >
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <h1 class="section__user_box_title">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <img src="svg/star_2yr76cddbiw0.svg" width="40px">
                  <br>
                  I’ve upped my game considerably since I started listening
                </h1>
                <p class="section__user_box_paragraph">Steven Blast</p>
              </div>
            </div>
          </div>
        </section>
      </div>
      <!-- ****SECTION END**** -->
  
      <!-- ****FOOTER START**** -->
      <div class="container">
        <footer class="footer">
          <div class="footer__container__box">
            <h1 class="footer__container_box_title">Castaway</h1>
            <div class="footer__container_box_icons">
              <i class="fab fa-instagram"><img src="svg/411cc415-2b74-4a13-bb5f-145f3795eb0e.png" width="30px"></i>
              <i class="fab fa-twitter"><img src="svg/609_original.jpg" style="border-radius: 10px;" width="30px"></i>
              <i class="fab fa-facebook"><img src="svg/linkedin-logo-hd-png-3.png" width="30px"></i>
              <i class="fab fa-facebook"><img src="svg/Viber_logo.svg.png" width="30px"></i>
            </div>
          </div>
          <div class="footer__container">
            <div class="footer__box">
              <li class="footer__box_item">
                <a class="footer__box_link" href="#">Home</a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#About">About</a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#Episodes">Episodes</a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#Contact">Contact</a>
              </li>
            </div>
            <div class="footer__box">
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Style Guide </a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Instructions </a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Changelog </a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Credit </a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Powered by Webflow </a>
              </li>
              <li class="footer__box_item">
                <a class="footer__box_link" href="#"> Licenses </a>
              </li>
            </div>
            <div class="footer__box">
              <img class="footer__box_img" src="svg/icon1.png" width="50px">
              <img class="footer__box_img" src="svg/icon2.png" width="50px">
              <img class="footer__box_img" src="svg/icon3.png" width="50px">
              <img class="footer__box_img" src="svg/icon4.png" width="50px">
              <img class="footer__box_img" src="svg/icon5.png" width="50px">
            </div>
          </div>
        </footer>
      </div>
      <!-- ****FOOTER END**** -->
  
  
      <!-- ****JAVASCRIPT LINKS**** -->
      <script src="./JS/utilits.js"></script>
      <script src="./JS/index.js"></script>
      <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
      window.addEventListener("load", () => {
  window.addEventListener("scroll", () => {
    $(".header").classList.toggle("active", window.scrollY > 0);
  });
  // AOS JAVASCRIPT LIBRARY
  AOS.init();
  // SECRET NAVBAR JAVASCRIPT TO THE CODES
  $(".fa-bars").addEventListener("click", () => {
    $(".secret__navbar").classList.add("active");
  });

  $(".fa-times").addEventListener("click", () => {
    $(".secret__navbar").classList.remove("active");
  });

  $$(".secret__navbar__link").forEach((item) => {
    item.addEventListener("click", () => {
      $(".secret__navbar").classList.remove("active");
    });
  });
});
    </body>
</body>
<script src="main.js"></script>
<script src="utilits.js"></script>
</html>
