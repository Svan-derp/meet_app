<template>
  <div class="container">
    <div class="screen">
      <form class="login">
        <input type="text" class="login__input" placeholder="Email" />
        <input type="password" class="login__input" placeholder="Password" />
        <button class="button is-primary">Log In</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}

.screen {
  position: relative;
  width: 360px;
  border-radius: 16px;
  box-shadow: 0px 8px 24px var(--primary);
}

.login {
  padding: 30px;
}

.login__input {
  border: none;
  border-bottom: 2px solid #d1d1d4;
  background: none;
  padding: 10px;
  padding-left: 24px;
  font-weight: 700;
  width: 100%;
  transition: 0.2s;
}

.login__input:active,
.login__input:focus,
.login__input:hover {
  outline: none;
  border-bottom-color: #6a679e;
}
.button {
  margin-top: 40px;
  width: stretch;
}
</style>
