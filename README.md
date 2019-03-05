# toolbox-creative-website-guide
### TBx Color Values (SASS)
```sass
/*TBx Color Values SASS*/
$white: #fff;
$black: #000;
$tbc-dark-green: #485452;
$tbc-darkest-green: #1a2422;
$tbc-light-green: #aebca3;
$tbc-light-green-hover: #6f8674;
$tbc-orange: #ff6c00;
$tbc-orange-hover: #da5c00;
$tbc-orange-link-only: #fd8831;
$tbc-beige: #f7f2ed;
$tbc-beige-bg: #f9f1eb;
$tbc-beige-bg-alt: #f7f2ed;
$tbc-dark-beige: #ddd1c4;
$tbc-light-blue: #999fd1;
$tbc-light-blue-hover: #75789a;
$tbc-gold: #ea9c0b;
$tbc-gold-hover: #cc7c18;
$tbc-brown: #b49ea1;
$tbc-brown-hover: #786a6d;
$tbc-light-brown: #d8cec7;
$tbc-red: #e63f42;
$tbc-red-hover: #a32d30;
$tbc-medium-gray: #777776;
$tbc-purple: #875578;
$tbc-purple-hover: #603e57;
$tbc-bright-purple: #cf7eb7;

/*Client Color Values*/
$tbc-brendle-green: #aebe37;
$tbc-brendle-teal: #8cbac4;
$tbc-brendle-blue: #327789;
$tbc-lcs-red: #a41128;
$tbc-a2a-yellow: #eea526;
$tbc-a2a-green: #007239;
$tbc-lulzbot-dark-green: #7b8a20;
$tbc-lulzbot-light-green: #bcd231;
$tbc-prieto-orange: #e47c26;
$tbc-solidscape-bright-blue: #1da1f2;
$tbc-food-bank-green: #8dc63f;
$tbc-food-bank-purple: #621c42;
$tbc-changing-minds-teal: #69c9ce;
$tbc-housing-catalyst-teal: #00677f;
````
### TBx Color Styles
```css
/*Add these classes to any text site-wide to change it's color*/
.white

.tbc-dark-green

.tbc-light-green

.tbc-orange

.tbc-red

.tbc-beige

.tbc-light-blue

.tbc-gold

.tbc-brown

.tbc-purple

.tbc-brendle-green

.tbc-a2a-yellow

.tbc-lcs-red

.tbc-lulzbot-dark-green

.tbc-lulzbot-light-green

.tbc-solidscape-bright-blue

.tbc-prieto-orange

.tbc-food-bank-green

.tbc-changing-minds-teal

.tbc-bright-purple

.tbc-housing-catalyst-teal
```

Color style usage:
```html
<p class="tbc-brown">This text will be brown.</p>
```

### Reveal Classes
If you would like to have a section “reveal“, we have three built in classes that allow you to reveal from the bottom, reveal from the left, or reveal from the right. Simply append the following class to any page element as needed.

```css
.reveal-standard <!--Reveal from bottom-->
.reveal-left <!--Reveal from left to right-->
.reveal-right <!--Reveal from right to left-->
```
```html
<!--Use case-->
<div class="container reveal-standard">
  <p>This is some content inside a container that will reveal from the bottom up.</p>
</div>
```

>_NOTE:_Due to JS conflicts, reveal classes SHOULD NOT be used on the homepage of the site.

### Creating a new Search & Filter Form
1. Go to Search & Filter in the Wordpress backend.
2. Duplicate the form you'd like to match. Make note of the form id you duplicate from.
3. Change the form name and modify any settings as needed. In most cases, you'll need to update the Tags, Categories & Taxonomies tab and potentially the Posts tab to make sure you're including and excluding the appropriate post information.
4. Using SFTP, log on to the Toolbox Server and go to: `wp-content > themes > Avada-Child-Theme > search-filter`
5. Right click on the file that matches the form ID you duplicated from and duplicate the file.
6. Rename the file with the form ID of your new form. This will ensure that your new form's display style will match the existing style.
7. You can embed the form in the page without a search form using the Results Shortcode. To include a Search Form, inlcude the Search Form shortcode immediately above the Results Shortcode.

8. You're all set!

### Project Industry and Service Links
The links below can be added to any <a> tag to link a hyperlink to a specific filter on the Projects page.
  ```
  <!--INDUSTRY Filters-->
/projects/?_sft_category=do-gooders
/projects/?_sft_category=threed-printing
/projects/?_sft_category=agtech
/projects/?_sft_category=clean-tech

<!--SERVICE Filters-->
/projects/?_sft_post_tag=ad-design
/projects/?_sft_post_tag=animation
/projects/?_sft_post_tag=logo-design
/projects/?_sft_post_tag=awareness-campaign
/projects/?_sft_post_tag=branding
/projects/?_sft_post_tag=digital-ads
/projects/?_sft_post_tag=ecommerce
/projects/?_sft_post_tag=print-design
/projects/?_sft_post_tag=website-design
  ```
Example use case:
```html
<a href="/projects/?_sft_category=do-gooders">This will link to a list of all Do Gooders projects</a>
<a href="/projects/?_sft_post_tag=logo-design">This will link to a list of all projects that have been tagged with a Logo Design tag</a>
```
