<script setup>
const role = "restoran";
</script>
<template>
  <div class="login-bg">
    <img src="\Frame.png" alt="" class="frame" />
    <div class="login-wrapper">
      <form action="">
        <div class="align-center">
          <p class="title">Kamu nanya mau makan apa?</p>
          <label> Pilih makananmu di{{ role }}</label>
        </div>
      </form>
    </div>
    <div v-if="role == 'restoran'" class="login-wrapper info">
      <div class="info-item">
        <h4 class="info-title">Restoran</h4>
        <div class="value">Restoran A</div>
      </div>
      <div class="info-item">
        <h4 class="info-title">Order bulan ini</h4>
        <div class="value">Ayam bakar</div>
      </div>
      <div class="info-item">
        <h4 class="info-title">Order Terakhir</h4>
        <div class="value">Ayam Geprek</div>
      </div>
      <div class="info-item">
        <h4 class="info-title">Order aktif</h4>
        <div class="value">Ayam goreng</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.login-wrapper {
  margin-left: auto;
  margin-right: auto;
}
.title {
  border-radius: 10px;
  background-color: #FCEED5;
  padding: 10px;
  color: #070046;
  font-size: 15px;
}
.frame {
  height: 200px;
  width: 200px;
  left: 30px;
  top: 30px;
  position: absolute;
}
.login-bg {
  position: relative;
  flex-direction: column;
}
.login-wrapper.info {
  width: 97%;
  display: flex;
  margin-left: 30px;
  margin-right: 30px;
  padding: 30px;
  margin-top: 50px;
}
.info-item {
  background-color: #FCEED5;
  padding: 20px;
  color: #070046;
  text-align: center;
  border-radius: 10px;
  width: 23%;
  margin-right: auto;
  min-height: 200px;
  display: flex;
  flex-direction: column;
  margin-left: auto;
}
.info-item .value {
  font-size: 30px;
  font-size: 700;
  margin-top: auto;
  margin-bottom: auto;
}
.info-title {
  padding: 5px;
  width: 100%;
  background-color: #FCEED5;
  border-radius: 5px;
}
</style>
