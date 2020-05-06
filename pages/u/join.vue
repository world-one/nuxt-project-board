<template>
  <div class="container container__height">
    <div class="box column is-one-third is-offset-one-third">
      <div class="tabs">
        <ul>
          <li class="is-active"><a>로그인</a></li>
          <li><a>회원가입</a></li>
        </ul>
      </div>
      <form action="">
        <div class="field">
          <p class="control has-icons-left has-icons-right">
            <input class="input" type="text" placeholder="아이디">
            <span class="icon is-small is-left">
              <i class="fa fa-user"></i>
            </span>
            <span class="icon is-small is-right">
              <i class="fas fa-check"></i>
            </span>
          </p>
        </div>
        <div class="field">
          <p class="control has-icons-left">
            <input class="input" type="password" placeholder="비밀번호">
            <span class="icon is-small is-left">
              <i class="fas fa-lock"></i>
            </span>
          </p>
        </div>

        <button type="submit" class="button is-fullwidth is-primary">Join</button>
      </form>

    </div>
  </div>
</template>