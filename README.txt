# Picture-Resizer.PHP
<?php
/*
image.php
*/
    header("Content-type: image/jpeg");
    $imgPath = 'image.jpg';
    $image = imagecreatefromjpeg($imgPath);
    $color = imagecolorallocate($image, 255, 255, 255);
    $string = "image used";
    $fontSize = 3;
    $x = 115;
    $y = 185;
    imagestring($image, $fontSize, $x, $y, $color);
    imagejpeg($image);
?>
