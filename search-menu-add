add_filter( 'wp_nav_menu_items', 'wptangtoc_menu_extras_tim_kiem', 10, 2 );
/**
tim kiem tren menu
 */
function wptangtoc_menu_extras_tim_kiem( $menu, $args ) {

	//* thay doi 'primary' hoac 'secondary' tuy menu ban su dung navigation menu
	if ( 'secondary' !== $args->theme_location )
		return $menu;

	ob_start();
	get_search_form();
	$search = ob_get_clean();
	$menu  .= '<li class="right search menu-item">' . $search . '</li>';
	return $menu;

}
