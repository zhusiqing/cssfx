<template>
  <div class="spinner">
    <div class="ball-scale-multiple">
      <div></div>
      <div></div>
      <div></div>
    </div>
  </div>
</template>

<style scoped>
.spinner {
  flex: 0 1 auto;
  flex-direction: column;
  flex-grow: 1;
  flex-shrink: 0;
  flex-basis: 25%;
  max-width: 25%;
  align-items: center;
  justify-content: center;
}

.ball-scale-multiple {
  position: relative;
  -webkit-transform: translateY(-30px);
  transform: translateY(-30px);
}

.ball-scale-multiple > div {
  background-color: #ffffff;
  border-radius: 100%;
}

.ball-scale-multiple > div:nth-child(2) {
  -webkit-animation-delay: -0.4s;
  animation-delay: -0.4s;
}

.ball-scale-multiple > div:nth-child(3) {
  -webkit-animation-delay: -0.2s;
  animation-delay: -0.2s;
}

.ball-scale-multiple > div {
  position: absolute;
  left: -30px;
  top: 0;
  opacity: 0;
  margin: 0;
  width: 60px;
  height: 60px;
  -webkit-animation: ball-scale-multiple 1s 0s linear infinite;
  animation: ball-scale-multiple 1s 0s linear infinite;
}
@keyframes ball-scale-multiple {
  0% {
    -webkit-transform: scale(0);
    transform: scale(0);
    opacity: 0;
  }

  5% {
    opacity: 1;
  }

  100% {
    -webkit-transform: scale(1);
    transform: scale(1);
    opacity: 0;
  }
}
</style>
