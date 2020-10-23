<?php
$key = ''; //Sua chave

$base_url = 'https://maps.googleapis.com/maps/api/directions/xml?sensor=false&key='.$key; 

$from = '-13.066770,-55.916290';
$to = '-12.538478,-55.725403';
$xml = simplexml_load_file($base_url."&origin=".$from."&destination=".$to); 

$distance = (string)$xml->route->leg->distance->text; 
$duration = (string)$xml->route->leg->duration->text;

print_r('<b>Distance:</b> '.$distance);
echo '<br />';
print_r('<b>Duration:</b> '.$duration);
?>
