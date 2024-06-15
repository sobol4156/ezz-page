<script setup></script>

<template>
  <div class="wrapper">
    <div class="left__part">
      <div class="left__content">
        <h1 class="left__title">Welcome to our community</h1>
        <p class="left__description">
          Clarity gives you the blocks & components you need to create a truly
          professional website.
        </p>
        <div class="comments">
          <div class="comments__rating">
            <!--  -->
          </div>
          <span class="comments__feedback">
            "We love Landingfolio! Our designers were using it for their
            projects, so we already knew what kind of design they want."
          </span>
          <div class="comments__user">
            <img class="comments__user-avatar" src="/user.webp" width="45" height="45" alt="" />
            <div class="comments__user-info">
              <span class="comments__user-name">Devon Lane</span>
              <span class="comments__user-post">Co-Founder, Design.co</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="right__part">
      <h2 class="right__title">Welcome back!</h2>
      <p class="right__description">
        Clarity gives you the blocks and components you need to create a truly
        professional website.
      </p>
      <form class="form" action="">
        <label for="">Email address</label>
        <input class="form__email" type="email" />
        <label for="">Password</label>
        <input class="form__password" type="password" />
        <div class="form__remember">
          <span>Remember me</span>
          <a href="#">Forgot password?</a>
        </div>
        <button class="btn-form" type="submit">Sign in</button>
      </form>
      <div class="right__new-acc">
        <span>Don't have an account?</span>
        <a href="#">Create free account</a>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.left__part {
  width: 472px;
  height: 100%;
  display: flex;
  flex-direction: column;

  justify-content: center;
  padding: 70px;
  background-color: #2563eb;
  color: white;
  flex: 1;

  .left__title,
  .left__description,
  .comments {
    width: 472px;
  }
}
.left__content{
  display: flex;
  flex-direction: column;
  align-items: end;
}

.right__part {
  padding: 70px;
  width: 527px;
  flex: 1;

  .right__title,
  .right__description,
  .form,
  .right__new-acc {
    width: 527px;
  }
}

.left__title{
  font-size: 62px;
  line-height: 62px;
  font-weight: 700;
  margin-bottom: 32px;
}
.left__description{
  font-size: 18px;
  line-height: 27px;
  color: #CBD5E1;
  margin-bottom: 150px;
}
.comments__feedback{
  font-size: 21px;
  font-weight: 600;
}
.comments__user{
  margin-top: 30px;
  display: flex;
  align-items: center;
  gap: 15px;
  .comments__user-info{
    display: flex;
    flex-direction: column;
    gap: 5px;
    justify-content: space-between;
  }

  .comments__user-name{
    font-size: 18px;
    font-weight: 700;
    line-height: 21px;
  }
  .comments__user-post{
    font-size: 16px;
    line-height: 16px;
    font-weight: 400;
  }
}




.right__title{
  font-size: 52px;
  line-height: 52px;
  font-weight: 700;
  margin-bottom: 20px;
}
.right__description{
  color: #52525B;
  font-size: 18px;
  margin-bottom: 60px;
}
.form{
  display: flex;
  flex-direction: column;

  label{
    color: #090914;
    font-size: 18px;
    font-weight: 600;
    margin-bottom: 5px;
  }
  input{
    height: 60px;
    font-size: 20px;
    padding-left: 10px;
    border-radius: 15px;
    border: 1px solid #CBD5E1;
    margin-bottom: 10px;
  }
  input:focus{
    outline: none;
    outline-offset: none;
  }
}
.form__remember{
  display: flex;
  justify-content: space-between;
  margin-bottom: 40px;
  span{
    color: #090914;
    font-weight: 600;
    font-size: 14px;
  }
  a{
    text-decoration: none;
    color: #2563eb;
    font-weight: 500;
    font-size: 14px;
  }

}
.btn-form{
  width: 160px;
  height: 55px;
  background: #2563eb;
  color: white;
  font-size: 18px;
  font-weight: 500;
  cursor: pointer;
  border-radius: 15px;
  border: none;
  margin-bottom: 20px;
}
.right__new-acc{
  display: flex;
  gap: 5px;
  font-size: 14px;
  span{
    color: #64748B;
    
  }
  a{
    text-decoration: none;
    color: #2563eb;
    
  }
}
</style>
