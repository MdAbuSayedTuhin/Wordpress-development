# Wordpress-development
<?php 
/*=============================
This Template explain a Header
==============================*/
?>
<!DOCTYPE html>
<html lang="<?php language_attributes(); ?>" class= "no-js">
<head>
    <meta charset="<?php bloginfo('charset')?>">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" conte
    nt="width=device-width, initial-scale=1.0">
    <title><?php bloginfo("name")?><?php wp_title()?></title>
    <?php wp_head(); ?>
</head>
<body <?php body_class(); ?>>
<Header id="header_area" class ="<?php echo get_theme_mod('abu_menu_position'); ?>">
    <div class="container">
        <div class="row">
            <div class="col-md-3">
                <a href="<?php echo home_url(); ?>"><img src="<?php echo get_theme_mod('abu_logo'); ?>" alt= ""></a>
                    </div>
        <div class="col-md-9">
        <?php wp_nav_menu(array ('theme_location' => 'main_manu', 'menu_id' => 'nav') ); ?>
                </div>
                    </div>
                        </div>
                            </div>
</Header>
<?php wp_footer(); ?>
