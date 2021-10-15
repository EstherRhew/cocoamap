<template>
  <header>
    <div class="container">
      <h1>CoCoa Map</h1>
      <div class="btn-box">
        <button class="btn">로그인</button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
header {
  background-color: #8a8074;
  width: 100%;
  height: 3.5rem;
  /* display: flex; */
  /* align-content: center; */
  color: #e0e0e0;
}
.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
h1 {
  font-family: "Noto Sans KR", sans-serif;
  font-weight: 700;
  font-size: 1.2em;
}
.btn {
  background-color: #ffffff;
  color: #83796c;
  border: none;
  outline: none;
  font-family: "Noto Sans KR", sans-serif;
  font-weight: 700;
  font-size: 0.8em;
  border-radius: 5px;
  padding: 6px 15px;
  cursor: pointer;
}
</style>