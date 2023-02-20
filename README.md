# Lorenglry
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    body {
	font: 15px Arial, Sans-serif;
}

.gallery {
	display: inline-block;
	text-align: center;
	margin: 10px auto;
	clear: both;
	padding: 0;
	padding: 10px;
	background-color: #ccc;
	border-radius: 5px;
}

.gallery img { /* thumbnails */
	width: 100px;
  height: 75px;
}





</style>
<body>
    <h1>Loren's Gallary</h1>

<div class="gallery">
	<a href="https://avatars.githubusercontent.com/u/112076184?v=4"><img src="https://avatars.githubusercontent.com/u/112076184?v=4" alt="Chrysanthemum: nice flower."></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Desert.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Desert.jpg" alt="Desert mountains"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Hydrangeas.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Hydrangeas.jpg" width="100" height="75" alt="Hydrangeas, called 'Hortensia' in Dutch"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Jellyfish.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Jellyfish.jpg" title="Jellyfish"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Koala.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Koala.jpg" alt="Koala"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Lighthouse.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Lighthouse.jpg" alt="Lighthouse"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Penguins.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Penguins.jpg" alt="Penguins"></a>
	<a href="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/Tulips.jpg"><img src="https://home.et.utwente.nl/slootenvanf/div/fancybox_images/tn/Tulips.jpg" alt="Yellow tulips"></a>
</div>



    
</body>
<script>
    $(document).ready(function() {
  // add all to same gallery
  $(".gallery a").attr("data-fancybox","mygallery");
  // assign captions and title from alt-attributes of images:
  $(".gallery a").each(function(){
    $(this).attr("data-caption", $(this).find("img").attr("alt"));
    $(this).attr("title", $(this).find("img").attr("alt"));
  });
  // start fancybox:
	$(".gallery a").fancybox();
});

</script>
</html>
