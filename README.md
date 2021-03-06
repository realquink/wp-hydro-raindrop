# Hydro Raindrop WordPress plugin 

![Hydro Logo](https://i.imgur.com/slcCepB.png)

Welcome to the Hydro Raindrop WordPress plugin repository on GitHub.

The `WP Hydro Raindrop` plugin provides Hydro Raindrop Multi Factor Authentication to your WordPress site.

## Installation

Download from wordpress.org (soon available).

## Manual installation

- Download and install fresh copy of WordPress (optional)
- Make sure you have installed composer (https://getcomposer.org/)
- `cd wp-content/plugins` (from root of your WordPress installation)
- `git clone git@github.com:adrenth/wp-hydro-raindrop.git`
- `cd wp-hydro-raindrop`
- `composer install`

The last step will install the required dependencies for the plugin.

And finally login with an admin account to your WordPress site and activate the plugin.

## Usage instructions

1. Login to your WordPress site as administrator.
2. Go to `Plugins` and search for the `WP Hydro Raindrop` plugin. Click `Activate` to activate the plugin.

If you don't have a **Hydrogen Developer Account**, go to [www.hydrogenplatform.com](https://www.hydrogenplatform.com) to register an account.

1. Under `Settings` navigate to the `Hydro Raindrop MFA` section and input your Application information to enable Hydro Raindrop MFA to your WordPress site. 
2. Under `Edit My Profile`, enter your HydroID in the `Hydro Raindrop MFA` section.
3. Follow the verification procedure to activate MFA for your account.

Site Editors / Authors / etc. can enable the Hydro Raindrop MFA from their profile page.

## Requirements

* **SSL MUST be enabled for MFA to work.**
* PHP 7.0 or higher is required.

## Customization

### Custom MFA page

* Login as a Site Editor
* Create a page (programmatically)
* Use the following shortcodes on this page (required!):
    - `[hydro_raindrop_mfa_form_open]`: renders the form opening element.
    - `[hydro_raindrop_mfa_form_close]`: renders closing element with the wp_nonce field.
    - `[hydro_raindrop_mfa_digits]`: renders 6 digits which should be entered into the Hydro app.
    - `[hydro_raindrop_mfa_button_authorize]`: renders the "Authorize" button; customize the look of the button using CSS class `hydro-raindrop-mfa-button-authorize`.
    - `[hydro_raindrop_mfa_button_cancel]`: renders the "Cancel" button; customize the look of the button using CSS class `hydro-raindrop-mfa-button-cancel`.
* Under `Setting` navigate to the `Hydro Raindro MFA` section and select the page you created.

## Documentation

https://www.hydrogenplatform.com/developers

## Issues

https://github.com/adrenth/wp-hydro-raindrop/issues

## Support

https://github.com/adrenth/wp-hydro-raindrop/issues

## Contributing to Hydro Raindrop WordPress plugin

Please make sure to obey the WP code styling by using PHP Code Sniffer with WordPress rules loaded into your IDE.
If you want to address an issue/bug, please create an issue first.
