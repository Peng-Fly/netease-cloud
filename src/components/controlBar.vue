<template>
  <div class="controlBar" :style="{ display: (typeof(isShow) == 'undefined' ? 'flex' : (isShow ? 'flex' : 'none')) }">
    <div class="ctrlMusicImg">
      <img src="" alt="">
    </div>
    <div class="ctrlMusicInfo">
      <p>可惜没如果</p>
      <p>林俊杰</p>
    </div>
    <div class="ctrlBtn">
      <div class="ctrlPlay"></div>
      <div class="ctrList"></div>
    </div>
  </div>
</template>
<script>
  export default {
    props:['isShow']
  }
</script>
<style>
  .controlBar{
    width: 100%;
    height: 1rem;
    background-color: rgba(250,250,250,.9);
    position: fixed;
    bottom: 0;
    right: 0;
    padding: 0.133rem;
    box-sizing: border-box;
    display: flex;
  }
  .controlBar .ctrlMusicImg{
    height: 0.73erm;
    width: 0.73rem;
  }
  .controlBar .ctrlMusicImg img{
    width: 100%;
  }
  .controlBar .ctrlMusicInfo{
    flex: 1;
    display: flex;
    margin-left: 0.3rem;
    flex-direction: column;
    justify-content: space-around;
  }
  .controlBar .ctrlMusicInfo p:first-child{
    font-size: 0.28rem;
  }
  .controlBar .ctrMusicInfo p:last-child{
    font-size: 0.207rem;
  }
  .controlBar .ctrlBtn {
    display: flex;
    align-items: center;
  }
  .controlBar .ctrlPlay{
    height: 0.553rem;
    width: 0.553rem;
    margin-right: 0.3rem;
    background: url(./../../static/images/ctrl_play.png);
    background-size: 100%;
  }
  .controlBar .ctrList{
    height: 0.553rem;
    width: 0.553rem;
    background: url(./../../static/images/ctrl_list.png);
    background-size: contain;
  }
</style>


