---
layout: default
title: Art playground
---

<div class="canvas">
    <div class="circle">
        <div class="dog">
            <div class="eyes"></div>
            <div class="hands"></div>
            <div class="left-hand"></div>
            <div class="right-hand"></div>
            <div class="legs"></div>
        </div>
    </div>
</div>

<style>
* {
  margin: 0;
  padding: 0;
}

.canvas {
  background: darkgray;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.circle {
  width: 70vmin;
  height: 70vmin;
  background: transparent;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.dog {
  position: relative;
  border: 0.5vmin solid black;
  width: 30vmin;
  height: 30vmin;
  border-top-left-radius: 100px;
  border-top-right-radius: 100px;
  border-bottom: 0;
  box-sizing: border-box;
  background: transparent;
}

.legs {
  display: flex;
  width: 30vmin;
}

.legs div {
  width: 7.5vmin;
  height: 6vmin;
  border: 0.5vmin solid black;
  border-bottom-left-radius: 100px;
  border-bottom-right-radius: 100px;
  border-top: 0;
  background: transparent;
}

.eyes {
  position: absolute;
  width: 5vmin;
  height: 5vmin;
  background: #000;
  border-radius: 50%;
  top: 13vmin;
  left: 5vmin;
  box-shadow: 14vmin 0;
}

.eyes:before{
  content: "";
  position: absolute;
  background: white;
  width: 2.5vmin;
  height: 2.5vmin;
  border-radius: 50%;
  left: 2vmin;
  box-shadow: 14vmin 0 white;
}

.mouth {
  position: absolute;
  width: 4vmin;
  height: 2vmin;
  border: 0.7vmin solid black;
  border-bottom-left-radius: 100px;
  border-bottom-right-radius: 100px;
  border-top: 0;
  top: 16vmin;
  left: 12vmin;
}

.left-hand, .right-hand {
  position: absolute;
  width: 4vmin;
  height: 4vmin;
  border: 0.5vmin solid black;
  border-bottom-left-radius: 100px;
  border-bottom-right-radius: 100px;
  border-top: 0;
}

.left-hand {
  top: 22vmin;
  left: 6vmin;
  transform: rotate(-45deg)
}

.right-hand{
  top: 22vmin;
  left: 18vmin;
  transform: rotate(45deg)
}
</style>