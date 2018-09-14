<template>
<div>
    <div class="row registerblock">
        <img src="@/assets/img/headerimg_signup.png" alt="headimg" class="registerblock__headimg">
        <div class="imgtxt text-nowrap">
            <h1 class="imgtxt"><b>Welcome</b> to ave</h1>
            <h4 class="imgtxt"><br><br><br><br><br> Sign in or register</h4>
        </div>
    </div>
    <div class="row justify-content-md-center mt-5 mainblock">
        <div class="col-lg-4 formblock">
            <h4>SIGN IN</h4>
            <form action="" class="signin">
                <input  type="email" placeholder="Your Email" class="inputBox mt-3" v-validate="'required|email'" name="singinemail" data-vv-as="email"><br>
                <span class="text-danger">{{ errors.first('singinemail') }}</span>
                <input type="password" name="psw" placeholder="Your password" class="inputBox mt-3" v-validate="'required'" data-vv-as="password">
                <span class="text-danger">{{ errors.first('psw') }}</span>
             </form>
                <div class="row mt-3">
                    <div class="col align-left">
                        <div class="btnSign">Sign In</div>
                    </div>
                    <div class="col align-right align-middle resetTxt mt-3">Forgot your Password &rarr;</div>
                </div>
        </div>
        <div class="col-lg-4 vline formblock">
            <h4>REGISTER</h4>
            <form action="" class="signup">
                <input  type="email" placeholder="Your Email" class="inputBox mt-3" v-validate="'required|email'" name="email"><br>
                <span class="text-danger">{{ errors.first('email') }}</span>
                <input type="password" name="password" placeholder="Your password" class="inputBox mt-3" v-validate="'required'">
                <span class="text-danger">{{ errors.first('password') }}</span>
                <input type="password" name="password confirm" placeholder="Confirm password" class="inputBox mt-3" v-validate="'required'">
                <span class="text-danger">{{ errors.first('password confirm') }}</span>
                <input type="checkbox" name="news" value="news" class="check mt-3 mr-2">Sign up for exclusive updates, discounts, new arrivals, contest<br>
          </form>
                <div class="row mt-3">
                    <div class="col align-left">
                        <div class="btnSign">Create account</div>
                    </div>
                    <div class="col align-right text-nowrap">By clicking ‘Create Account’, you agree to our <p class="resetTxt">Privacy Policy &rarr;</p>
                    </div>
                </div>
        </div>
    </div>

</div>
</template>

