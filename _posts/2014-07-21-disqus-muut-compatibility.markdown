---
published: true
title: Disqus & Muut Compatibility
layout: post
tags: [coding, disqus, muut, wordpress]
categories: [Coding]
permalink: disqus-muut-compatibility
---
**Disqus & Muut** can work together in Wordpress. Simply *place this code at the bottom of your theme's functions.php file*.

    // Make sure that Disqus commenting can be used even on a site that uses Muut for other things.
    function my_remove_muut_comments_template_filter() {
    if (class_exists('Muut') && class_exists('Muut_Initializer')) {
    remove_filter( 'comments_template', array( Muut_Initializer::instance(), 'initTemplateLoader' ) );
    }
    }
    add_action( 'init', 'my_remove_muut_comments_template_filter' );

This code was provided by Paul Hughes from Muut and will be available on the next release of the WP plugin.