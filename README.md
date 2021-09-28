# wordpress_file_for_development
# নিচের কোডটি ,আমরা যখন CSS ফাইল্কে  enqueue করার দরকার হবে এই ফিলেটি  CSS ফোল্ডারে  নিয়ে terminal গিয়ে রান করলে,ফাইল  গুলা একসাথে  দিয়ে  দিবে ।
# !/usr/bin/env php
<?php
foreach(glob("*.css") as $css){
    echo "wp_enqueue_style( 'wptheme-{$css}', get_template_directory_uri().'/css/{$css}',null,'1.0');\n";
}