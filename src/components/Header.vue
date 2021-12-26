
<template>
    <header>
         <div class="header">
            <div class="container header-menu-contain">
              <div>
                   <img src="../assets/img/dc-logo.png" alt="Logo DC">
              </div>
             <div class="contain-menu">
                  <ul class="menu">
                      <li v-for="link, index in links" :key="index">
                            <a href="#">{{link.nameLink}}</a>
                       </li>
                 </ul>
             </div>
        </div>
    </div>
    </header>
</template>


<script>
export default {
  name: "Header",
  data: function() {
      return {
          links: [
              {
                  nameLink: 'CHARACTERS',
              },
              {
                  nameLink: 'COMICS',
              },
              {
                  nameLink: 'MOVIES',
              },
              {
                  nameLink: 'TV',
              },
              {
                  nameLink: 'GAMES',
              },
              {
                  nameLink: 'COLLECTIBLES',
              },
              {
                  nameLink: 'VIDEOS',
              },
              {
                  nameLink: 'FANS',
              },
              {
                  nameLink: 'NEWS',
              },
              {
                  nameLink: 'SHOP',
              }
          ]
      }
  }
};
</script>


<style lang="scss">
@import '../styles/common.scss';
@import '../styles/variables.scss';
.header {
    height: 100px;
    background-color: #ffffff;
    height: 100px;
    .header-menu-contain {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
}
.menu {
    display: flex;
    li {
        list-style: none;
        margin-left: 20px;
        height: 100px;
    }
}
a {
    font-size: 12px;
    text-decoration: none;
    line-height: 100px;
    padding-bottom: 40px;
    color: black;
    &:hover {
        color: $primary_color;
        border-bottom: 3px solid $primary_color;
    }
}
img {
    width: 70px;
}
</style>