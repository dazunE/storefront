# Storefront Changelog

### *2017.xx.xx* - 2.2.0
* **Fix** - Remove unnecessary button styling in WooCommerce Quick View extension.
* **Tweak** - Improved the Bookings calendar styles.
* **Dev** - Added actions; `storefront_jetpack_infinite_scroll_before`, `storefront_jetpack_infinite_scroll_after`, `storefront_jetpack_product_infinite_scroll_before` and `storefront_jetpack_product_infinite_scroll_after`.

### *2017.01.17* - 2.1.7
* **Tweak** - [WooCommerce 2.7] - Ensure all checkboxes function correctly with new markup.
* **Tweak** - [WooCommerce 2.7] - Order item meta styling.
* **Tweak** - [WooCommerce 2.7] - Don't display the stock icon when `.stock` is empty.
* **Fix** - Cross-sells layout

### *2016.11.15* - 2.1.6
* **Fix** - Close dropdowns in the nav when you tap away on touch devices.
* **Fix** - Ensure the header cart dropdown works properly on touch devices.
* **Fix** - 404 layout.
* **Fix** - Javascript error when `.site-header-cart` isn't present in the DOM.
* **Fix** - Consistent spacing in site title.
* **Dev** - Refactored `storefront_get_content_background_color()` to account for and give priority (over Storefront Designer) to Storefront Powerpack.
* **Dev** - Deprecated `is_woocommerce_activated()` and made it pluggable.
* **Dev** - Added `storefront_is_woocommerce_activated()`.

### *2016.10.24* - 2.1.5
* **Tweak** - Jetpack infinite scroll now works on product archives as well as posts.
* **Tweak** - Add styles for WooCommerce 2.7's new gallery.
* **Tweak** - Style the 'dismiss' link in WooCommerce 2.7's 'demo notice' feature.

### *2016.10.11* - 2.1.4
* **Fix** - Product/category title size in loops (WooCommerce 2.7 compatibility).
* **Fix** - Star rating selector when WooCommerce lightbox is disabled.
* **Fix** - Dropdowns can now be closed on iOS.
* **Fix** - PHP 5.2 compatibility.
* **Tweak** - Structured data sanitization and other minor adjustments.
* **Tweak** - Header cart dropdown now only scrolls if it renders beyond the current window height.
* **Tweak** - Star rating selector styling.
* **Tweak** - Widget region order. Addresses the issue of widgets being added to an unexpected region on default installs.
* **Dev** - `storefront_post_thumbnail()` is now hooked in to `storefront_post_content_before`.
* **Dev** - Added `storefront_post_content_before` and `storefront_post_content_after` actions.
* **Dev** - `storefront_post_thumbnail()` now provides a default size.
* **Dev** - Updated FontAwesome to 4.6.3.

### *2016.09.26* - 2.1.3
* **Fix** - Dropdowns in the main navigation when tabbing through links.
* **Fix** - Hide empty labels when using the Advanced Product Labels extension.
* **Tweak** - Updated MasterCard logo. Kudos [@nishitlangaliya](https://github.com/nishitlangaliya).

### *2016.09.08* - 2.1.2
* **Fix** - Fatal errors in the Customizer when using older versions of WordPress.
* **Tweak** - blockUI styling on checkout.
* **Dev** - Tweaked how Customizer defaults are set so that checkboxes will work.

### *2016.09.02* - 2.1.1
* **Fix** - Changed some customizer settings transport from postMessage to refresh for live preview of changes.
* **Fix** - Secondary navigation dropdown styling.
* **Dev** - Restructured the way objects are initiated. Objects are now initiated into an accessible global $storefront for access to hooks. Kudos [@jtsternberg](https://github.com/jtsternberg).

### *2016.08.24* - 2.1.0
* **New** - Lots of SEO enhancements. Kudos [@opportus](https://github.com/opportus).
* **New** - Selective refresh on site title, tag line, logo and widgets.
* **New** - Integration with [Advanced Product Labels](https://woocommerce.com/products/woocommerce-advanced-product-labels/) extension.
* **New** - Integration with [WooCommerce Mix and Match](https://woocommerce.com/products/woocommerce-mix-and-match-products/) extension.
* **New** - Integration with [WooCommerce Quick View](https://woocommerce.com/products/woocommerce-quick-view/) extension.
* **Fix** - Product thumbnail size on cart page.
* **Fix** - Sticky order review position on RTL stores. Kudos [@farookibrahim](https://github.com/farookibrahim)
* **Dev** - Restructured scss; removed components/typography and added main styles to `assets/sass/base/_base.scss`. Layout styles then added to `assets/sass/base/_layout.scss`. Moved WooCommerce extension integration styles to `assets/sass/woocommerce/extensions/`.

### *2016.07.26* - 2.0.7
* **Fix** - Compatibility with PHP 5.2.
* **Fix** - Further structured data sanitization.
* **Dev** - Added .editorconfig.

### *2016.07.22* - 2.0.6
* **Fix** - Added missing laser card icon.
* **Fix** - Additional menu displayed on handheld when a menu isn't assigned to the 'primary' location.
* **Fix** - Structured data sanitization.
* **Fix** - Photography extension layout on handheld devices.
* **Tweak** - Product Bundles integration tweaks.
* **Tweak** - Updated all docs links to point to docs.woocommerce.com.
* **Dev** - Made `storefront_primary_navigation_wrapper()` and `storefront_primary_navigation_wrapper_close()` pluggable.

### *2016.07.05* - 2.0.5
* **Fix** - Saved payment method styling.
* **Fix** - Card expiry date layout in checkout.
* **Fix** - Product loop links in widgets are no longer underlined.
* **Tweak** - Secondary nav wrapper no longer present is no menu is assigned. Kudos [@titanic-fanatic](https://github.com/titanic-fanatic).

### *2016.06.14* - 2.0.4
* **Fix** - Credit card input label styling.
* **Fix** - `$content_width` declaration.
* **Fix** - Mobile menu when using an empty menu in the primary menu location.
* **Tweak** - Minor style fixes / improvements for various WooCommerce extensions.
* **Tweak** - Account / Cart links in the handheld nav bar will only appear if the pages are set in WooCommerce.
* **Tweak** - Footer padding on handheld devices.
* **Tweak** - `pre` background color to ensure legibility when displayed in messages.
* **Dev** - Deprecate `storefront_html_tag_schema()`.

### *2016.06.02* - 2.0.3
* **Fix** - Fatal error when using Storefront without WooCommerce.

### *2016.06.01* - 2.0.2
* **Fix** - Correct CSS property applied to the header if no background image is present.
* **Fix** - Sticky order review + Checkout Add-ons compatibility.
* **Fix** - Active link color when using the Custom Menu widget in the sidebar.
* **Fix** - Store notice no longer hidden by the handheld nav bar.
* **Fix** - Some errors in structured data. Kudos [@opportus](https://github.com/opportus).
* **Dev** - Added `storefront_sticky_order_review` filter.
* **Dev** - Added `storefront_structured_data` filter for structured data customisation.

### *2016.05.12* - 2.0.1
* **Fix** - Horizontal scroll bar on Safari.
* **Fix** - Ensure the menu toggle background color updates correctly in the preview.
* **Fix** - Positioning of cart icon in header cart link.
* **Fix** - Missing Customizer settings after updating to 2.0.0.
* **Tweak** - Blog pagination hover effect.
* **Tweak** - Apply the 'alt' button style to the checkout button in the cart widget.
* **Dev** - Apply Customizer setting defaults on `customize_register` to account for child themes filtering `storefront_setting_default_values`.
* **Dev** - Fix typo in the `storefront_homepage_after_best_selling_products` action name.

### *2016.05.06* - 2.0.0
* **New** - Extensive improvements to the responsive design.
* **New** - Design refresh including full typography revamp.
* **New** - Refactored all underlying code and re-organised / minified assets.
* **New** - Added 'Best Sellers' product section to the Homepage.
* **New** - oEmbed styling to match Storefront aesthetic.
* **New** - The welcome screen now dynamically pulls in new products.
* **New** - Added `storefront_header_styles()` for the header image/styles along with the `storefront_header_styles` filter to customise the treatment of header styles.
* **New** - Support for the Custom Logo theme feature (requires WordPress 4.5).
* **New** - Styled 'Average Rating' widget.
* **New** - Styled WooCommerce 2.6 tabbed account section.
* **Tweak** - All template functions are now pluggable.
* **Tweak** - The 'menu' button is now styled automatically based on header settings in the Customizer.
* **Tweak** - Customizer settings are now all assigned to a single theme mod on theme switch and Customizer save to improve performance.
* **Tweak** - Humanised homepage product section titles.
* **Tweak** - Redesigned blog post meta section.
* **Tweak** - Comments / Reviews design.
* **Fix** - Inadequate left/right content margin at certain screen sizes.
* **Fix** - z-index on demo store notice.
* **Fix** - Checkout add-ons integration.
* **Fix** - Display of portrait logos on handheld devices.
* **Dev** - Deprecated `storefront_categorized_blog()`.
* **Dev** - Deprecated `storefront_sanitize_hex_color()`.
* **Dev** - Deprecated `storefront_sanitize_layout()`.

### *2016.01.18* - 1.6.1
* **Tweak** - Jetpack integration updates.
* **Tweak** - Styling for WooCommerce 2.5's terms positioning on the checkout.
* **Tweak** - Styling for WooCommerce 2.5's totals inc tax on the cart.
* **Tweak** - Removed the bottom border on the cart / checkout pages.
* **Tweak** - Renamed 'Header' widget region to 'Below Header'.
* **Fix** - WooCommerce active filters widget now styled.
* **Fix** - Image gallery layouts.
* **Fix** - Sticky order review feature now accounts for any size of payment box to avoid cutting off the Place Order button.

### *2016.01.05* - 1.6.0
* **New** - [Storefront Mega Menus](https://woocommerce.com/products/storefront-mega-menus/) integration.
* **New** - Integration with [Ship to Multiple Addresses](https://woocommerce.com/products/shipping-multiple-addresses/) extension.
* **New** - Sticky order review on checkout.
* **New** - Automatic credit card type detection in compatible payment gateways.
* **Tweak** - Styled the in stock/out of stock message. Props @nishitlangaliya.
* **Tweak** - Added new function `storefront_star_rating_script`. Outputs JavaScript for the new star rating input while we wait for WooCommerce 2.5 to be released.
* **Tweak** - Contrast on hovered links in the primary navigation.
* **Tweak** - If no widgets are present in the sidebar a full width layout will be applied to all pages.
* **Tweak** - Updated integration with the Variation Swatches extension.
* **Tweak** - Featured images on posts / pages are now centered.
* **Fix** - Table alignment on desktop.
* **Dev** - Added some new hooks to the homepage template tags; `storefront_homepage_after_product_categories_title`, `storefront_homepage_after_recent_products_title`, `storefront_homepage_after_featured_products_title`, `storefront_homepage_after_popular_products_title`, `storefront_homepage_after_on_sale_products_title`
* **Dev** - Styling for 6 column product layouts.
* **Dev** - Updates FontAwesome to version 4.5.0.

### *2015.11.03* - 1.5.3
* **Fix** - Storefront will now automatically load a child themes stylesheet.
* **Fix** - CSS Syntax error in Customizer output.
* **Tweak** - WooCommerce responsive table styles.

### *2015.10.30* - 1.5.2
* **Fix** - Duplicate menu display when not using a handheld menu and switching between desktop/handheld orientations.
* **Tweak** - Adjusts how CSS is enqueued for child theme compatibility with RTL.
* **Tweak** - Better display of prices in WooCommerce product widgets.
* **Tweak** - Improved caption display.
* **Tweak** - Re-organised welcome screen.
* **Tweak** - Adjusted Product Bundles integration to include support for the WooCommerce Product Bundles - Tabular Layout extension.
* **Tweak** - Styled the variation reset link.
* **Tweak** - Start rating input now more intuitive.
* **Tweak** - Added styles for WooCommerce password strength meter.
* **Tweak** - Arrange the login/registration forms on the account page into two columns.
* **Tweak** - Support for the most recent class applied to the site logo added by Jetpack.
* **Dev** - `storefront_display_comments` is now hooked into `storefront_single_post_after` with priority 20 (was 10).
* **Localisation** - All translations are now managed on [WordPress.org](https://translate.wordpress.org/projects/wp-themes/storefront)
* **Localisation** - Product names can no longer be translated.

### *2015.09.10* - 1.5.1
* **Fix** - Occasional text wrapping on product sorting dropdown.
* **Fix** - Double taps no longer required to click buttons in iOS browsers.
* **Fix** - Fixed the landing page layout in WordPress 4.3+
* **Fix** - Header cart now compatible with Currency Converter extension.
* **Tweak** - Embedded objects (videos etc) width will no longer exceed the width of their containing element.
* **Tweak** - Improved the ligibility of the active swatch when using the Variation Swatches extension.
* **Dev** - Improved how RTL stylesheets are enqueued.
* **Dev** - The default layout is now  filterable via `storefront_default_layout`.

### *2015.08.11* - 1.5.0
* **New** - rtl support.
* **New** - Integration with WooCommerce Deposits.
* **New** - Pages now display featured images above the page title.
* **New** - Revamped 404 page helpfulness to include product search, popular products and product ctegories.
* **New** - Integration with WooCommerce Bundles extension.
* **New** - Scrolling header cart.
* **Fix** - Welcome screen now only visible to admins.
* **Fix** - Horizontal scroll bar in Safari at small sizes.
* **Fix** - Pay for order screen layout when using full width page template on my account.
* **Fix** - Fixed display of disabled `option`s in Firefox.
* **Dev** - Added `storefront_sanitize_checkbox()` sanitization function.
* **Dev** - Added `Storefront_Custom_Radio_Image_Control` class for creating radio image controls in the Customizer.
* **Dev** - Added `storefront_post_thumbnail()`.
* **Dev** - Renamed `do_shortcode_func()` to `storefront_do_shortcode()`.
* **Dev** - Updated Composite Products integration for compatibility with 3.2.
* **Dev** - Updated normalize.css to 3.0.3.
* **Tweak** - Menu button spacing on handheld.
* **Tweak** - Button display in cart widgets.
* **Tweak** - The 'Configure Menus' button in the welcome screen now points to the Customizer.

### *2015.06.10* - 1.4.6
* **Fix** - `font-family` delcaration on `select`s.
* **Tweak** - Escaping function used on homepage section titles.
* **Tweak** - Remove all instances of `do_shortcode()` to improve performance.
* **Tweak** - Reduced link focus outline from 2px to 1px.
* **Dev** - `$storefront_version` global when using a child theme.

### *2015.05.14* - 1.4.5
* **Fix** - Use the correct escaping function in `storefront_product_categories()`.
* **Fix** - Pagination when only showing product categories / subcategories on archives.
* **Tweak** - Logo prompt in Header section in Customizer.
* **Tweak** - Only output description paragraph in header if one is set.
* **Tweak** - Updated header image dimension recommendation.
* **Tweak** - Dismissible notices.
* **Tweak** - Debug notices in WooCommerce message. Props @WPprodigy.
* **Dev** - Bump npm susy to 2.2.3.
* **Dev** - Made `Layout_Picker_Storefront_Control` class pluggable. Props @niravmehta
* **Dev** - Added order and orderby parameters to homepage featured products template tag.
* **Dev** - Added before/after hooks inside homepage product sections.

### *2015.04.23* - 1.4.4
* **Fix** - Post author styles applied to incorrect child comments. Props @ibndawood.
* **Fix** - Third level dropdowns (and beyond) are now revealed in the correct situation.
* **Fix** - Header margin on homepage template when WooCommerce isn't activated.
* **Fix** - Dropdowns on touch devices.
* **Fix** - Pagination hidden correctly when only displaying categories / subcategories.
* **Tweak** - Output WooCommerce messages on all appropriate pages.
* **Tweak** - Revamped 'Enhance' section of welcome screen.
* **Localisation** - Translation files are now included.

### *2015.04.08* - 1.4.3
* **Fix** - Star rating display in Safari.
* **Tweak** - Cart dropdown appears on focus.
* **Tweak** - Payment form layout/styling when paying from My Account.
* **Tweak** - Improvements to the product archive sorting / pagination layout and styling.
* **Tweak** - Layered nav list item styling.
* **Tweak** - Product meta styling.
* **Tweak** - Heading and Star Rating size on product loops.
* **Dev** - Updated node-sass and grunt-sass dependency versions.

### *2015.03.24* - 1.4.2
* **Fix** - Navigation not displaying if no menu is assigned to primary location.

### *2015.03.24* - 1.4.1
* **Fix** - Remove unnecessary `!important` declaration on star rating color.
* **Fix** - Star rating display in IE11.
* **Fix** - Site header margin when using shop page as homepage.
* **Fix** - Navigation on handheld devices when no menu is set.
* **Tweak** - Layout selector graphics.
* **Tweak** - Accessibility improvements in post meta.
* **Tweak** - Products widget styling.
* **Tweak** - Widget headings are now `h3`s.
* **Tweak** - Skip links are now a function (`storefront_skip_links()`) hooked into `storefront_header`.
* **Tweak** - Header widget region markup only displays when widgets are assigned.
* **Tweak** - `:focus` styles.
* **Dev** - Replaced `paginate_links()` with `the_posts_pagination()`.
* **Dev** - Replaced `previous_post_link()` and `next_post_link()` with `the_post_navigation()`.
* **Dev** - HTML5 widget support.
* **Dev** - Fixed typo in classname: `storefront-feautred-products` is now `storefront-featured-products`.
* **Dev** - Updated node-bourbon
* **Dev** - Replaced instances of `box-sizing` mixin with standard css.

### *2015.03.09* - 1.4.0
* **New** - Added a 'Handheld' menu location.
* **New** - Many accessibility improvements.
* **Fix** - Header margin when WooCommerce isn't activated.
* **Fix** - Subscription payment form layout.
* **Tweak** - Pagination now clears content.
* **Tweak** - Header cart now displays sub total.
* **Dev** - Removed npm-debug.log.

### *2015.02.20* - 1.3.1
* **Fix** - Header margin when using static page or latest posts for homepage.
* **Fix** - Related products total / columns.
* **Tweak** - Product Reviews Pro submission form.
* **Tweak** - Review form input alignment.
* **Tweak** - Improved integration with WooCommerce Photography extension.
* **Dev** - Added `storefront_related_products_args` filter.

### *2015.02.10* - 1.3.0
* **New** - Support for WooCommerce 2.3 features like responsive tables.
* **Fix** - Margin on site title / logo.
* **Fix** - Tweaked some css selectors in the checkout to improve compatiblity with Amazon Payments Advanced gateway.
* **Fix** - Layout selector in Firefox.
* **Fix** - `storefront_menu_toggle_text` filter. Props [jesinwp](https://github.com/jesinwp).
* **Tweak** - Product Reviews Pro integration.
* **Tweak** - Select width in WooCommerce forms.
* **Tweak** - Composite Products integration improvements.
* **Tweak** - Removed header widget region bottom margin.
* **Tweak** - Increased size of photos displayed in the WooCommerce Photography extension.
* **Tweak** - Page / term description width.
* **Tweak** - Hide 'What is WooCommerce' section on welcome screen when it's already installed.
* **Tweak** - Widget region order in dashboard.
* **Tweak** - Add the correct page content hook in the inline docs ( template-homepage.php ).
* **Tweak** - `mark` styling.
* **Dev** - Added `storefront_sanitize_choices()`.
* **Dev** - Tweaked the divider Customizer control to allow text/title.
* **Dev** - Updated FontAwesome to version 4.3.0.
* **Dev** - Libsass / node susy for faster compiling. Please do a fresh `npm install` when working with this version.

### *2015.01.22* - 1.2.5
* **Fix** - Review form input alignment.
* **Tweak** - Widget region order in dashboard.
* **Tweak** - Post archive pagination is now numbered.
* **Tweak** - Styling for current post / product category in widgets.
* **Tweak** - Added an informational section to the Customizer.
* **Tweak** - Link color in the sidebar.
* **Tweak** - Padding in the header.
* **Tweak** - Breadcrumb position.
* **Dev** - `storefront_header_cart()` is now pluggable.
* **Dev** - Make use of WordPress 4.1 functions `the_archive_title()` and `the_archive_description()`.

### *2015.01.15* - 1.2.4
* **Fix** - First level threaded comment layout.
* **Tweak** - Improved font size on handheld devices.
* **Tweak** - Wishlist table design.
* **Dev** - Reorganised sass files.
* **Dev** - Added some handy class names to homepage product sections.
* **Dev** - Added `storefront_menu_toggle_text` filter.
* **Dev** - Updated how WooCommerce styles are dequeued.

### *2015.01.07* - 1.2.3
* **Fix** - Button border in WooCommerce messages when using the Storefront Designer extension.
* **Tweak** - Stock icon.
* **Dev** - Grid system now powered by Susy.

### *2015.01.05* - 1.2.2
* **Fix** - Hidden publish date on single post.
* **Fix** - Order details color.
* **Tweak** - Header widget z-index for when used with Parallax Hero.
* **Tweak** - Nested `ul`s in widgets.
* **Tweak** - Product category widget styling.
* **Tweak** - Make use of WordPress 4.1's `title-tag` theme feature. (Requires WordPress 4.1).
* **Tweak** - Welcome screen tweaks for WordPress 4.1.
* **Tweak** - Slightly reduced button/input size.
* **Dev** - Made `storefront_product_search()` pluggable.

### *2014.12.09* - 1.2.1
* **Fix** - Blog post category and tag link output.
* **Fix** - Cart link in handheld orientation.
* **Tweak** - Improved payment form display when using a dark background colour.
* **Tweak** - Blog author rich snippet.
* **Dev** - Added `storefront_single_post_posted_on_html` filter.
* **Dev** - Replaced reset.css with normalize.css.

### *2014.12.02* - 1.2.0
* **New** - Integration with Product Reviews Pro extension.
* **New** - Integration with Smart Coupons extension.
* **Fix** - Layout picker images when using a child theme.
* **Fix** - Header link color now properly applied to site title.
* **Fix** - Included styling for `.form-row-wide`.
* **Dev** - Added `storefront_copyright_text` filter.
* **Dev** - Tweaked how Storefront determines whether Customizer logic should be loaded.
* **Dev** - Added `storefront_after_footer` action.
* **Dev** - Customizer CSS now correctly appended to appropriate stylesheets.
* **Tweak** - Improved star rating input display for handheld devices.
* **Tweak** - Several minor code optimisations (thanks https://scrutinizer-ci.com).

### *2014.11.24* - 1.1.1
* **Fix** - Title tag now displays correctly.
* **Localisation** - Tweaked how translation files are loaded.

### *2014.11.21* - 1.1.0
* **New** - Integration with AJAX Layered Navigation extension.
* **New** - Integration with Variation Swatches and Photos extension.
* **New** - Integration with Composite Products extension.
* **New** - Integration with WooCommerce Photography extension.
* **New** - Integration with Jetpacks `site-logo` feature.
* **Tweak** - Create account checkbox styling at checkout.
* **Tweak** - Added support for WordPress 4.1s `title-tag` theme feature.
* **Tweak** - Softened default text color slightly.
* **Tweak** - Styling for valid/invalid inputs.
* **Tweak** - Price filter slider styling.
* **Tweak** - Default settings for display options.
* **Tweak** - Added custom layout picker control.
* **Tweak** - Removed unused animation styles.
* **Tweak** - Default customizer settings added.

### *2014.10.15* - 1.0.3
* **Fix** - Comment date link color.
* **Fix** - Comment reply link color.
* **Tweak** - Sanitize layout setting.
* **Tweak** - No redirect to welcome screen on activation.

### *2014.10.12* - 1.0.2
* **Fix** - Upsell display on cart when using full width template.
* **Fix** - Smiley display.
* **Fix** - Date font size in post meta.
* **Fix** - Remove the breadcrumb separator to resolve markup errors.
* **Fix** - Returning to the welcome screen from the Customizer.
* **Tweak** - Clearfixed product galleries.
* **Tweak** - Adjusted the add to cart form design on product details pages.
* **Tweak** - Set a default border color on buttons for extensions to utilise.
* **Tweak** - Adjusted the max-height of images in the payment method list items.
* **Tweak** - Secondary navigation alignment in header.
* **Tweak** - Sale marker display is more universally friendly and customisable.
* **Tweak** - Moved the header controls in to the header image section.
* **Tweak** - Removed header widget border.
* **Tweak** - `.site-main` margin.
* **Dev** - Added `storefront_product_thumbnail_columns` filter.
* **Dev** - Added `Gruntfile.js` and `package.json`.

### *2014.09.14* - 1.0.1
* **Tweak** - Improved vertical spacing in the site header on mobile sized devices.
* **Tweak** - Updated some links & content in the welcome screen.
* **Tweak** - Improved comment/review respond form layout.
* **Fix** - Header text color live preview in cart dropdown.

### *2014.09.05* - 1.0.0
* Initial release