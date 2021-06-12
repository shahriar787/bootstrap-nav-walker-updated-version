<h4>WP Bootstrap Nav Walker</h4>


<pre>
<h3>If you are using a bootstrap version 4 or less then you need<br/>to download it from below link</h3> 
</pre>
<code>https://github.com/wp-bootstrap/wp-bootstrap-navwalker</code>

<pre>
<h3>If you are using a bootstrap version 4 or less then you need to download it from</h3> 

<h2>I'm not the original author of this plugin. </h3>
I just added some code because it doesn't work the latest version of bootstrap. 

<h1>This file will work on the bootstrap updated version.</h1>
</pre>

<h3>How To Install</h3>
<hr>
<pre>
/**
 * Register Custom Navigation Walker
 */
require_once get_template_directory() . '/class-wp-bootstrap-navwalker.php';
</pre>

<h4>Bootstrap Version 4.0 to 5.0 <h4>
  <div class="highlight highlight-text-html-php position-relative">
 <pre>
  <nav class="wpc-main-menu navbar navbar-expand-md navbar-light" role="navigation">
      <!-- Brand and toggle get grouped for better mobile display -->
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"> <span class="navbar-toggler-icon"></span>
       </button>
      <a class="navbar-brand" href="#">Navbar</a>
          wp_nav_menu( array(
              'theme_location'    => 'mart_primary_menu',
              'depth'             => 2,
              'container'         => 'div',
              'container_class'   => 'collapse navbar-collapse',
              'container_id'      => 'navbarSupportedContent',
              'menu_class'        => 'nav navbar-nav',
              'fallback_cb'       => 'WP_Bootstrap_Navwalker::fallback',
              'walker'            => new WP_Bootstrap_Navwalker(),
          ) );
  </pre>
  </div>
