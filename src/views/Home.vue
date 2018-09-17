<template>
<div>
    <div class="row homeblock">
        <img src="@/assets/img/homeimg.png" alt="homeimg" class="homeblock__homeimg">
        <router-link to="/products" class="homeblock__shopbtn text-nowrap">SHOP MEN'S COLLECTION</router-link>
    </div>
    <div class="container-fluid midnavBlock">
        <hr>
        <div class="row">
          <div class="col-md-1"></div>
            <div class="col-md-6 row">
              <div class="col">popular</div>
              <div class="col">new arrivals</div>
              <div class="col">best sellers</div>
              <div class="col">special offers</div>
              <div class="col">coming soon</div>
            </div>
            <div class="col-md-5">coming soon</div>
        </div>
    </div>
    <div class="container-fluid productBox">
        <div class="row">
            <div class="col-md-1"></div>
            <div class="col-md-5">
                <div class="row mb-4">
                    <div class="col-md-6 productBox__Item"><img src="@/assets/img/photo_avenue.png" alt="product" class="productBox__sImg"></div>
                    <div class="col-md-6 productBox__Item"><img src="@/assets/img/photo_mad.png" alt="product" class="productBox__sImg"></div>
                </div>
                <div class="row">
                    <div class="col-md productBox__Item "><img src="@/assets/img/photo_bluish.png" alt="product" class="productBox__bImg"></div>
                </div>
            </div>
            <div class="col-md-5">
              <div class="row mb-4">
                  <div class="col-md productBox__Item "><img src="@/assets/img/photo_sweater.png" alt="product" class="productBox__bImg"></div>
               </div>
               <div class="row mb-4">
                    <div class="col-md-6 productBox__Item"><img src="@/assets/img/photo_avenue.png" alt="product" class="productBox__sImg"></div>
                    <div class="col-md-6 productBox__Item"><img src="@/assets/img/photo_dark.png" alt="product" class="productBox__sImg"></div>
                </div>
             </div>
            <div class="col-md-1"></div>
        </div>
    </div>
    <hr>
    <div class="container-fluid mb-5">
      <div class="row lookbooks">
        <div class="col mr-4 lookbook row">
          <div class="col"><img src="@/assets/img/lookbook1.png" alt="person" class="align-bottom"></div>
          <div class="col mt-5">
            <p class="lookbook__hl lookbook__hl mr-4"><b>MEN'S</b><br>lookbook</p>
            <div class="lookbook__btn mr-4 align-middle">View now</div>
          </div>
        </div>
        <div class="col lookbook row">
          <div class="col"><img src="@/assets/img/lookbook2.png" alt="person" class="align-bottom"></div>
           <div class="col mt-5">
            <p class="lookbook__hl lookbook__hl mr-4"><b>Womens'S</b><br>lookbook</p>
            <div class="lookbook__btn mr-4 align-middle">View now</div>
          </div>        
        </div>
        <div class="col ml-4 lookbook row">
          <div class="col"><img src="@/assets/img/lookbook3.png" alt="person" class="align-bottom"></div>
          <div class="col mt-5">
            <p class="lookbook__hl lookbook__hl mr-4"><b>your</b><br>lookbook</p>
            <div class="lookbook__btn mr-4 align-middle">View now</div>
          </div>   
        </div>
      </div>
    </div>
</div>
</template>

<script>
export default {
    name: "Home"
};
</script>
