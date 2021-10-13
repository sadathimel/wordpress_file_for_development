# wordpress_file_for_development
নিচের কোডটি ,আমরা যখন CSS ফাইল্কে  enqueue করার দরকার হবে এই ফিলেটি  CSS ফোল্ডারে  নিয়ে terminal গিয়ে রান করলে,ফাইল  গুলা একসাথে  দিয়ে  দিবে ।
# !/usr/bin/env php
https://github.com/sadathimel/wordpress_file_for_development/blob/main/enq-css.php

নিচের কোডটি ,আমরা যখন Js ফাইল্কে  enqueue করার দরকার হবে এই ফিলেটি  Js ফোল্ডারে  নিয়ে terminal গিয়ে রান করলে,ফাইল  গুলা একসাথে  দিয়ে  দিবে ।

https://github.com/sadathimel/wordpress_file_for_development/blob/main/enq-js.php
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


যারা ওয়ার্ডপ্রেস নিয়ে কাজ করেন তবুও ওয়ার্ডপ্রেসের উপর কনফিডেন্স লেভেল অনেক বেশি না। তাদেরকে কয়েকটা ওয়ার্ডপ্রেসের ফাইলের নাম দিব নিছে, সেই গুলো থেকে প্রতিদিন কিছু কিছু ফাংশন চেক করতে হবে আর দেখলেই বুঝতে পারবেন সব গুলো ফাংশন কত কাজের। আপনি হয়ত অনেক ইউজফুল ফাংশন আছে যা জানতেনই না। আর আবার অনেক ফাংশন ইউজ করতেন তা কোথায় আছে সেটাও জানতেন না। এই সব কিছু ক্লিয়ার হয়ে যাবে। যত বেশি দেখবেন তত বেশি ওয়ার্ডপ্রেসের উপর আপনার কর্তুত্ত্ব বাড়বে। নাহলে বছরের পর বছর কাজ করবেন, কিন্তু কিছু কমন ফাংশন ছাড়া আপনি কিছুই পারবেন না। 
এখন নিছে লিস্ট দিচ্ছি। এটাকে একটা সিলেবাস বা গাইড হিসাবে নিবেন। হাজার হাজার ফাইল আছে ওয়ার্ডপ্রেসে, সব ফাইল আপনার দেখা লাগবে না। ওয়ার্ডপ্রেস অনেক ফাইল নিজের কাজে ইউজ করে। আপনি যা ইউজ করবেন প্রায় প্রতিদিন আপনার কাছে তা এই ফাইল গুলতে পাবেন। মাত্র ২৫টার মত ফাইল যদি আপনি ভালো মত নিজের আয়ত্বে আনতে পারেন, তাহলে আপনি যেকোন যায়গায় অন্যদের থেকে এগিয়ে থাকবেন একটু হলেও, কাজ করে মজা পাবেন, আর যেকোন ইন্টার্ভিউতে গেলে অনেক সময় যে ইন্টার্ভিউ নিচ্ছে সেও লজ্জায় পড়ে যাবে আপনার জ্ঞান দেখে। আর চাকরি পাওয়া তো কোণ ব্যাপারই না। তাই ১ মাস লাগুক আর ৬ মাস লাগুক এই ফাইলগুলো খুব ভালোভাবে দেখুন আর বুঝুন, নেটে সার্চ করে ইউজকেইস দেখুন। যেকোণ ভালো থিম খুললেই এই সব ফাংশনের কাজ পাবেন। ��

# general-template.php
# link-template.php
# author-template.php
# option.php
# post.php
# post-template.php
# post.thumbnail-template.php
# query.php
# taxonomy.php
# category.php
# category-template.php
# comment.php
# comment-template.php
# media.php
# formatting.php
# pluggable.php
# plugin.php
# user.php
# functions.php
# functions.wp-scripts.php
# functions.wp-styles.php
# block-editor.php
# blocks.php
# http.php  ( For advanced user)
# template-loader.php ( For advanced user)

আর WP_Query ক্লাসটা হল প্লাগিন ডেভেলপারদের জন্য সব থেকে গুরুতপুর্ন একটা ক্লাস। এটা নিয়ে ওয়ার্ডপ্রেসের অনেক বেশি লম্বা ডকুমেন্টেশন আছে। এই ক্লাসের ব্যবহার অবশ্যই পানির মত ক্লিয়ার থাকতে হবে। তবে এটা পরে শিখলে চলবে যারা বিগিনার তাদেরকে বলছি।
