# Epsilon Dasboard Widget

## 1. Installation
> Load class-epsilon-dashboard.php

> Initiate Epsilon_Dashboard class; E.g.

	if ( ! function_exists( 'plugin_name_dashboard_widget' ) ) {
		/**
		 * The helper method to run the class
		 *
		 * @return Epsilon_Dashboard
		 */
		function plugin_name_dashboard_widget() {
			$epsilon_dashboard_args = array(
				'widget_title' => esc_html__( 'Theme Listings', 'text-domain' ),
				'feed_url'	=> array( '#' )
			);
			return Epsilon_Dashboard::instance( $epsilon_dashboard_args );
		}
	}

	plugin_name_dashboard_widget();
