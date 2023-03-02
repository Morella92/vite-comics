<template>
    <footer class="footer">

      <div class="container">

        <div class="row-footer">
          <button class="footer-button">Sign-up now!</button>
        
        <div class="col-footer">
          <h4 class="footer-title">follow us</h4>
          <ul class="footer-list">
            <li>
                <a href="#">
                    <img class="footer-list-items" src="../../public/footer-facebook.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img class="footer-list-items" src="../../public/footer-twitter.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img class="footer-list-items" src="../../public/footer-youtube.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img class="footer-list-items" src="../../public/footer-pinterest.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img class="footer-list-items" src="../../public/footer-periscope.png" alt="">
                </a>
            </li>
          </ul>

        </div>
        </div>
      </div>
  
    </footer>
  </template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.footer{
  background-color: #303030;
}
.row-footer{
  display: flex;
  justify-content: space-between;
  align-items: center;
  min-height: 70px;
}

.footer-button{
  color: $white;
  text-transform: uppercase;
  background-color: #303030;
  border: 4px solid $main-blue;
  line-height: 40px;

  &:hover{
    transform: scale(1.1);
  }
}

.footer-title{
  color: $main-blue;
  text-transform: uppercase;

  &:hover{
    color: $white;
  }
}
.col-footer{
  display: flex;
  align-items: center;
  gap: 20px;
  color: $white;
}

.footer-list{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}

.footer-list-items{

  &:hover{
    transform: scale(1.1);
  }
}

</style>