<template>
    <footer class="container">

      <div class="footer">

        <button class="footer-button">Sign-up now!</button>
        
        <div class="col-footer">
          <h4 class="footer-title">follow us</h4>
          <ul class="footer-list">
            <li>
                <a href="#">
                    <img src="../../public/footer-facebook.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../public/footer-twitter.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../public/footer-youtube.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../public/footer-pinterest.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../public/footer-periscope.png" alt="">
                </a>
            </li>
          </ul>

        </div>
      </div>
  
    </footer>
  </template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
.footer{
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #303030;
  min-height: 70px;
  padding-left: 20px;
  padding-right: 20px;
}

.footer-button{
  color: white;
  text-transform: uppercase;
  background-color: #303030;
  border: 4px solid #0282F9;
  line-height: 40px;
}

.footer-title{
  color: #0282F9;
  text-transform: uppercase;
}
.col-footer{
  display: flex;
  align-items: center;
  gap: 20px;
  color: white;
}

.footer-list{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}



</style>