<template>
  <div class="box">
    <div class="right-tick"></div>
  </div>
</template>

<style scoped>
.box {
  width: 3.5em;
  height: 3.5em;
  position: relative;
}
.right-tick {
  width: 3em;
  height: 1.5em;
  position: absolute;
  left: 50%;
  top: 50%;
  margin: auto;
  transform: translate(-50%, -100%) rotate(-45deg);
  overflow: hidden;
}
.right-tick::before,
.right-tick::after {
  content: '';
  position: absolute;
  background-color: #3cefff;
  border-radius: 2px;
}
.right-tick::before {
  width: 2px;
  height: 1.5em;
  left: 0;
  animation: tickLeft 0.5s linear 3s 1 both;
}
.right-tick:after {
  width: 3em;
  height: 2px;
  bottom: 0;
  animation: tickRight 0.5s linear 3.5s 1 both;
}
@-webkit-keyframes tickLeft {
  0% {
    top: -100%;
  }
  100% {
    top: 0%;
  }
}
@-webkit-keyframes tickRight {
  0% {
    left: -100%;
  }
  100% {
    left: 0%;
  }
}
</style>
