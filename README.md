# yahoomediaplayer
A version of the yahoo media / web player that can be embedded to play media, in particular mp3 files.


## Basic Usage

### 1 Add the yahoomedia folder in this repository to your sites relevant js folder 

### 2 Add the following to pages that have mp3 files on your site

```javascript
<script >
var YMPParams = { autoplay:false,volume:1, assetsroot: '{{ site.url }}/assets/js/yahoomedia', defaultalbumart:"{{ site.url }}/images/victorian_carol_singers_silouette_32.png" };
</script>

<script  src="{{ site.url }}/assets/js/yahoomedia/music-player.min.js"></script>
```

Note that you should change the assetroot to where the js file is located.

### 3 Update the branding

Change the branding-dark-theme.png in the yahoomedia/img folder to one relevant to your site.

Change the defaultalbumart in the script to an image/ logo relevant to your site.

### 4 Add a href tags to your mp3 files on your site, for example

```html
<a href="{{ site.url }}/audio/joy to the world.mp3">Joy to the World</a>
<br>
<a href="{{ site.url }}/audio/jingle bells.mp3">Jingle Bells</a>
<br>
<a href="{{ site.url }}/audio/silent night short.mp3">Silent Night</a>
<br>
<a href="{{ site.url }}/audio/deck the halls.mp3">Deck the Halls</a>
```

### 5 Any mp3 audio on your site will now have play icons and a useful sidebar...

See an example at http://www.victoriancarolsingershire.uk/.

![yahoo media player bar](https://github.com/hyweljohnllewellyn/yahoomediaplayer/blob/master/yahoomediascreenshot.png)
