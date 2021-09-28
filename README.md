# wordpress_file_for_development
নিচের কোডটি ,আমরা যখন CSS ফাইল্কে  enqueue করার দরকার হবে এই ফিলেটি  CSS ফোল্ডারে  নিয়ে terminal গিয়ে রান করলে,ফাইল  গুলা একসাথে  দিয়ে  দিবে ।
# !/usr/bin/env php
https://github.com/sadathimel/wordpress_file_for_development/blob/main/enq-css.php

# Action Hook

add_action('after_setup_theme','function');

add_action('wp_enqueue_scripts','function');

add_action('wp_header','function');

add_action('wp_footer','function');

add_action('widgets_init','function');

# Filter Hook 
apply_filters( 'the_content', string $content ); 

apply_filters( 'the_title', string $title, int $id ); 

apply_filters( 'wp_title', string $title, string $sep, string $seplocation );

apply_filters( 'author_link', string $link, int $author_id, string $author_nicename );   