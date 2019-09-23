#####1. First Name, Last Name

    Raximjon Komiljonov
    
#####2. Contact Info (add several ways to contact you)
    
    Email: komiljonovrahimjon@gmail.com
    Tel:   +998 94 6099500
    Tel:   +998 97 7195419
    
#####3. Summary (your goal, wishes, reveal what is important for you, what do you want and why. Some kind of self-presentation. In case of lack of experience  Junior Developer sells his/her potential, his/her passion and ability to learn fast. You shouldn't think that everybody is going to teach you when you come to the workplace . Rather being a Junior means always learning new things from everywhere etc.).
    
    Goal: To be one of the best programmers.
    
    Wish: I want to help humanity by developing useful applications.
   
    Important: My family. My life. Quality of work.
    
    Want: I want to be brilliant programmer because I want to get more best feelings from that kind of actions.
    
    Self-presentation: So 1.82cm height boy with good behavior.
    
    Ability: I can learn fast if I have free time for this.

#####4. Skills (e.g. programming languages, frameworks, methodologies, version control, tools etc.)

    PHP, Javascript, HTML, CSS
    Bootstrap, WordPress, Joomla, Laravel
    BEM, MVC
    Git, Bitbucket, Github
    Adobe PhotoShop, AI, Online metrix(GPSI, GM, Pingdom)
    English, Korean
    
#####5. Code examples (LATEST)

```php
    /* 1. CONSTANTS */
    define('THEMEROOT', get_stylesheet_directory_uri());
    define('CSS', THEMEROOT . '/css');
    define('JS', THEMEROOT . '/js');
    define('IMG', THEMEROOT . '/images');
    
    /* 2. ACF options page */
    if (function_exists('acf_add_options_page')) {
        acf_add_options_page();
    }
    if (function_exists('acf_set_options_page_menu')) {
        acf_set_options_page_menu('PTA Theme');
    }
    
    /* 3. Menus */
    register_nav_menus(array(
        'headermenu' => 'Header Menu',
        'footermenu' => 'Footer Menu',
    ));
    
    /* 4. Styles and scripts */
    function theme_scripts()
    {
        wp_enqueue_style('main', CSS . '/main.css');
        wp_enqueue_style('add', CSS . '/add.css');
        wp_enqueue_style('add-rax', CSS . '/add-rax.css');
        wp_enqueue_style('new-css', CSS . '/new.css');
    
        wp_enqueue_script('libs', JS . '/libs.min.js', array('jquery'), null, true);
        wp_enqueue_script('main', JS . '/main.js', array('jquery'), null, true);
        wp_enqueue_script('profile', JS . '/profile.js', array('jquery'), null, true);
        wp_enqueue_script('new-js', JS . '/new.js', array('jquery'), null, true);
        if ( is_page_template('page-myFAQs.php') ) {
            wp_enqueue_script( 'faqs-script', JS.'/faqs.js', array( 'jquery' ), null, true );
        }
        wp_localize_script(
            "new-js",
            "reviews_filter",
            array(
                "ajax_url"      =>  admin_url("admin-ajax.php"),
                'security'      =>  wp_create_nonce('reviews-filter-nonce')
            )
        );
    
        wp_localize_script(
            "profile",
            "profile_obj",
            array(
                "ajax_url"      =>  admin_url("admin-ajax.php"),
                'security'      =>  wp_create_nonce('profile-save-security-nonce')
            )
        );
    }
    add_action('wp_enqueue_scripts', 'theme_scripts');
```
    
#####6. Experience (for a Junior Dev it means all kinds of experience: coding tests, projects from courses, freelance projects - wherever they had the opportunity to demonstrate skills they have. Also it would be awesome if you add links to source code)
    
    Alex-ITS from 6th february of 2014 till 2nd september of 2015
    Upwork ~
    NGS from 24 february of 2016
#####7. Education (including courses, seminars, lectures, online learning)

    Tashkent University of Information Techonologies (completed)
    Udemy - The Complete JavaScript Course 2018 from Jonas Schmedtmann
#####8. English (elaborate on what kind of practice you had, if any, how long it lasted and so on)
    
    Pre-intermediate