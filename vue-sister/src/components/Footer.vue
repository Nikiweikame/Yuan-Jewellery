<template>
  <footer class="footer">
    <div class="copyright">
      <span>Copyright 2023</span><span class="chinese"> © 苑・飾物</span
      ><span> All rights reserved.</span>
    </div>
    <div class="social-software">
      <a
        class="nav-link"
        href="https://www.facebook.com/yuanjewellery"
        target="_blank"
        ><svg
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M36.6666 20C36.6666 10.8 29.2 3.33333 20 3.33333C10.8 3.33333 3.33331 10.8 3.33331 20C3.33331 28.0667 9.06665 34.7833 16.6666 36.3333V25H13.3333V20H16.6666V15.8333C16.6666 12.6167 19.2833 10 22.5 10H26.6666V15H23.3333C22.4166 15 21.6666 15.75 21.6666 16.6667V20H26.6666V25H21.6666V36.5833C30.0833 35.75 36.6666 28.65 36.6666 20Z"
            fill="#ffffff"
          />
        </svg>
      </a>
      <a
        class="nav-link"
        href="https://www.instagram.com/yuan_jewellery/"
        target="_blank"
        ><svg
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M13 3.33333H27C32.3333 3.33333 36.6666 7.66667 36.6666 13V27C36.6666 29.5638 35.6482 32.0225 33.8353 33.8354C32.0225 35.6482 29.5637 36.6667 27 36.6667H13C7.66665 36.6667 3.33331 32.3333 3.33331 27V13C3.33331 10.4362 4.35176 7.97749 6.16461 6.16464C7.97747 4.35178 10.4362 3.33333 13 3.33333ZM12.6666 6.66667C11.0753 6.66667 9.54922 7.29881 8.42401 8.42403C7.29879 9.54924 6.66665 11.0754 6.66665 12.6667V27.3333C6.66665 30.65 9.34998 33.3333 12.6666 33.3333H27.3333C28.9246 33.3333 30.4507 32.7012 31.576 31.576C32.7012 30.4508 33.3333 28.9246 33.3333 27.3333V12.6667C33.3333 9.35 30.65 6.66667 27.3333 6.66667H12.6666ZM28.75 9.16667C29.3025 9.16667 29.8324 9.38616 30.2231 9.77686C30.6138 10.1676 30.8333 10.6975 30.8333 11.25C30.8333 11.8025 30.6138 12.3324 30.2231 12.7231C29.8324 13.1138 29.3025 13.3333 28.75 13.3333C28.1974 13.3333 27.6675 13.1138 27.2768 12.7231C26.8861 12.3324 26.6666 11.8025 26.6666 11.25C26.6666 10.6975 26.8861 10.1676 27.2768 9.77686C27.6675 9.38616 28.1974 9.16667 28.75 9.16667ZM20 11.6667C22.2101 11.6667 24.3297 12.5446 25.8925 14.1074C27.4553 15.6702 28.3333 17.7899 28.3333 20C28.3333 22.2101 27.4553 24.3298 25.8925 25.8926C24.3297 27.4554 22.2101 28.3333 20 28.3333C17.7898 28.3333 15.6702 27.4554 14.1074 25.8926C12.5446 24.3298 11.6666 22.2101 11.6666 20C11.6666 17.7899 12.5446 15.6702 14.1074 14.1074C15.6702 12.5446 17.7898 11.6667 20 11.6667ZM20 15C18.6739 15 17.4021 15.5268 16.4644 16.4645C15.5268 17.4021 15 18.6739 15 20C15 21.3261 15.5268 22.5979 16.4644 23.5355C17.4021 24.4732 18.6739 25 20 25C21.3261 25 22.5978 24.4732 23.5355 23.5355C24.4732 22.5979 25 21.3261 25 20C25 18.6739 24.4732 17.4021 23.5355 16.4645C22.5978 15.5268 21.3261 15 20 15Z"
            fill="#ffffff"
          />
        </svg>
      </a>
    </div>
  </footer>
</template>

<style scoped lang="scss">
.footer {
  padding: 15px 30px;
  background-color: #39598c;
  color: white;
  display: flex;
  flex-direction: column-reverse;
  justify-content: space-between;
  align-items: center;
  .copyright {
    margin-top: 30px;
    span {
      font-family: "Comfortaa", "Noto Sans TC", Arial, sans-serif;
    }
    // .chinese {
    //   font-family: "Noto Sans TC", sans-serif;
    // }
  }
  .social-software {
    margin-right: -15px;
    display: flex;
    a {
      padding: 0 15px;
    }
  }
}
@media screen and (min-width: 576px) {
  .footer {
    flex-direction: row;
    .copyright {
      margin-top: 0px;
    }
  }
}
@media screen and (min-width: 992px) {
  .footer {
    padding: 15px 150px;
  }
}
</style>

<script></script>
