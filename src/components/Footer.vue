<template>
  <footer class="top-footer">
        <div class="footer-bar">
          <div class="flex">
            <h1 class="header-logo">estra inc.</h1>
            <nav class="header-nav" :class="{'open':isClass}">
              <ul>
                <li><a href="#">home</a></li>
                <li><a href="#">about</a></li>
                <li><a href="#">service</a></li>
                <li><a href="#">works</a></li>
                <li><a href="#">price</a></li>
                <li><a href="#">contact</a></li>
              </ul>
            </nav>
          </div>
        </div>
        <small>Copyright 2019 estra inc. All Rights Reserved.</small>
      </footer>
</template>

<script>
export default {
  data() {
    return {
      isClass: false
    };
  }
};
</script>


<style scoped>

.header-logo {
  font-size: 20px;
  font-weight: bold;
  margin-left: 35px;
  color: #fff;
  line-height: 70px;
}

.footer-bar {
  height: 70px;
  line-height: 70px;
}

.top-footer {
  background: #000;
  text-align: center;
}

.top-footer small {
  text-align: center;
  color: #fff;
}

.header-nav a {
  color: #fff;
  text-decoration: none;
}

.header-nav li {
  display: inline-block;
  margin-right: 35px;
  font-size: 16px;
}
.flex {
  display: flex;
  justify-content: space-between;
  line-height: 70px;
}
@media screen and (max-width: 768px) {
  .top-footer {
    margin: 0;
    width: 100%;
    text-align: center;
  }
  .header-nav a {
  display: none;
}
.header-logo {
    margin: 0;
    width: 100%;
    text-align: center;
  }
}
</style>