<template>
  <div id="display-box-1">
    <div class="display-row-content">
      <span>
        {{rowtext}}
      </span>
    </div>
    <div class="display-column-content">
      <span>
        {{ columntext }}
      </span>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'Secretdiv',
    data() {
      return {
        rowtext: '我也不想这样反反复复',
        columntext: '反正每个人最后都孤独',
      }
    }
  }
</script>
<style scoped>
#display-box-1 {
  background-color: black;
  width: 400px;
  height: 400px;
  position:relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 10vw 0 0 0;
  color: white;
}

.display-row-content {
  position: absolute;
  left: 0;
  top: 0;
  transform:rotate(0deg);
  width: 100%;
  height: 100%;
  line-height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.display-row-content span {
  transform: scale(1.5, 20.0)
}

.display-column-content {
  position: absolute;
  left: 0;
  top: 0;
  transform:rotate(-90deg);
  width: 100%;
  height: 100%;
  line-height: 100%;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.display-column-content span {
  transform: scale(1.5, 20.0)
}

</style>