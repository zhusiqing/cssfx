<template>
  <div class="snake-spinner">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
  </div>
</template>

<style scoped>
.snake-spinner {
  width: 100px;
  height: 20px;
  position: relative;
}
.snake-spinner span {
  position: absolute;
  width: 20px;
  height: 20px;
  background-color: #3cefff;
  opacity: 0.5;
  border-radius: 20px;
  animation: snake 1s infinite ease-in-out;
}
.snake-spinner span:nth-child(1) {
  left: 0px;
  animation-delay: 0s;
}
.snake-spinner span:nth-child(2) {
  left: 20px;
  animation-delay: 0.2s;
}
.snake-spinner span:nth-child(3) {
  left: 40px;
  animation-delay: 0.4s;
}
.snake-spinner span:nth-child(4) {
  left: 60px;
  animation-delay: 0.6s;
}
.snake-spinner span:nth-child(5) {
  left: 80px;
  animation-delay: 0.8s;
}
@keyframes snake {
  0% {
    opacity: 0.3;
    transform: translateY(0px);
    box-shadow: 0px 0px 3px rgba(0, 0, 0, 0.1);
  }
  50% {
    opacity: 1;
    transform: translateY(-10px);
    background-color: #fc2f70;
    box-shadow: 0px 20px 3px rgba(0, 0, 0, 0.05);
  }
  100% {
    opacity: 0.3;
    transform: translateY(0px);
    box-shadow: 0px 0px 3px rgba(0, 0, 0, 0.1);
  }
}
</style>
