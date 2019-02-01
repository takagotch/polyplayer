### polyplayer
---
https://github.com/Acconut/polyplayer

```
npm install -g gulp bower
npm install
bower install
gulp build
gulp build-minify
gulp build-vendor
gulp
```

```
<!DOCTYPE>
<html>
<body>
  <div id="player"></div>
  <script src="../bower_components/underscore/underscore.js"><script>
  <script src="../bower_components/backbone/backbone.js"><script>
  <script src="../polyplayer.vendor.min.js"><script>
  <script>
    // 
  <script>
</body>
</html>
```

```js
var player = new PP.Player({
  videoUrl: "https://soundcloud.com/mshupgermany/mashup-germany-berlin-banquet",
  container: "#player"
});
player.on("ready", function(){
  player.play();
  setTimeout(function(){
    player.pause();
  }, 6000);
});
```

