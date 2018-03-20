<template>
    <Page class="page">
        <ActionBar class="action-bar" title="Hello world">
        <NavigationButton text="Go Back" android.systemIcon="ic_menu_back" @tap="$router.push('/home')"/>
        </ActionBar>

        <StackLayout backgroundColor="#3c495e">
            <Label text="first" height="70" backgroundColor="#43b883"/>
            <Label text="second" height="70" backgroundColor="#289062"/>
            <Label text="third" height="70" backgroundColor="#1c6b48"/>
        </StackLayout>
        <div class="music-cards">
            <img src="https://usatsneakhype.files.wordpress.com/2015/04/emceez-ansari-4.jpg?w=1000" alt="" />
            <div class="play-btn color4">
                <img src="https://cdn4.iconfinder.com/data/icons/ionicons/512/icon-play-128.png" alt="" />
            </div>
            <div class="disc color4">
                <div class="music-title">Wiz Khalifa</div>
            </div>
        </div>
    </Page>
</template>

<script>
  export default {
    data () {
      return {
        
      };
    },
  };
</script>

<style scoped>
    .music-cards {
        width: 178px;
        height: 180px;
        display: inline-block;
        position: relative;
        float: left;
        padding: 1px;
        }
    .music-cards img {
        width: 100%;
        opacity: 1;
    }
 .music-cards .play-btn {
  display: inline-block;
  width: 40px;
  height: 40px;
  position: absolute;
  bottom: 17px;
  right: 10px;
  z-index: 2;
  border-radius: 50%;
  box-shadow: 0px 0px 10px 1px rgba(0, 0, 0, 0.3);
  cursor: pointer;
  transform: scale(1, 1);
  transition: 0.5s ease;
}
 .music-cards .play-btn img {
  width: 20px;
  padding: 11px;
  opacity: 0.4;
}
.music-cards .play-btn:hover {
  transform: scale(1.1, 1.1);
}
 .music-cards .play-btn:hover img {
  opacity: 0.6;
}
.music-cards .play-btn.color1 {
  background: #F6A197;
}
.music-cards .play-btn.color2 {
  background: #FDA052;
}
.music-cards .play-btn.color3 {
  background: #F6B2C7;
}
.music-cards .play-btn.color4 {
  background: #476471;
}
.music-cards .play-btn.color5 {
  background: #61BF93;
}
.music-cards .play-btn.color6 {
  background: #E26263;
}
.music-cards .disc {
  position: absolute;
  bottom: 0px;
  height: 35px;
  left: 0;
  right: 0;
  color: #fff;
  font-size: 12px;
  text-align: left;
  margin: 1px;
}
.music-cards .disc .music-title {
  margin: 10px;
}
.music-cards .disc.color1 {
  background: #F6A197;
}
.music-cards .disc.color2 {
  background: #FDA052;
}
 .music-cards .disc.color3 {
  background: #F6B2C7;
}
 .music-cards .disc.color4 {
  background: #476471;
}
.music-cards .disc.color5 {
  background: #61BF93;
}
.music-cards .disc.color6 {
  background: #E26263;
}

</style>
