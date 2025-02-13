# Evelution Overview

## What is Evelution?
Evelution is a Skin built by Qora Qore Telecommunities and is distributed for general use on Github by A Techno Services. This skin is designed to bring an experience that it is as close as the ones from FandomDesktop.

Feel free to use it on your wiki and make it as the default skin, if you wish. Modifications to the code must be licensed under the GPL 3.0 license.

Evelution can be called whatever you want on your Wiki. It is the second fork of MpistoSkin2, the first being MpistoServerSkin2.

## Differences of Evelution and MpistoSkin2
Evelution, despite being essentially similar to MpistoSkin2 from Q.Qore, there're several differences, to name a few:
- Evelution used to be a plain Desktop skin with official support of Screens between 705 to 1500 pixels whereas MpistoSkin2 was always a hybrid Mobile-Desktop-Desktop XL skin with support of screens between 360 to 2000 pixels. As such, no XS and XL breakpoints existed on Evelution. XL Breakpoint was added in version 3.4.0 while XS Breakpoint was added in version 3.6.0
- Evelution has 705 pixels on its small size instead of 760 pixels that MpistoSkin2 offers. Its large size offers the same size as MpistoSkin2, which is at 1280 pixels.
- Evelution used to lack a right rail that MpistoSkin2 has. However, evelution has support for Sitenotice. 4.8.0 added support for Right Rail but in a completely different style despite sharing the same classes from MpistoSkin2
- Evelution uses smaller typography on the Article compared to MpistoSkin2. Article text size for instance, is at 13 pixels.
- Evelution uses LocalStorage to store all skin-related settings (Theme Management, Article Width, Toolbar width and Sticky Nav width) so when page is reloaded, those settings are preserved. MpistoSkin2 does not rely on this and as such, all skin-related settings are reset when page is reloaded.
- Evelution used not to take care of System's native Dark Mode, unlike MpistoSkin2
- Evelution's Global Navigation consists of different items:
  - Top links include the GitHub link (Scoped to this repository), the Evelution Support Server Link and the MediaWik site link
  - The Explore Menu contains the list of links found in the footer the Vector skin has, instead of the official A Techno Links
  - Bottom Links are essentially identical, however, no wikis and flags menus exist
  - Bottom Links additionally contain the **In other Languages**, **Language Variants** and the **Notifications** links but they appear only if the page has interwiki links, the wiki's language has other versions such as Chinese  and the Echo Extension is installed respectively
  - Search in Global Navigation in Evelution is Local instead of Global compared to MpistoSkin2
  - Evelution has no user avatar support, unlike MpistoSkin2 and such an icon takes place. Also, instead of the user name being in the tooltip, the **Personal tools** message takes place
- Evelution uses icons from the Material Icons library instead of the DS Icons, and they're embedded as a font instead of an SVG compared to MpistoSkin2.
- Unlike MpistoSkin2, no Global Footer exists. However, a small article footer does exist
- In Evelution, only namespaces, views and actions reside by default on Page Header Actions. In MpistoSkoin2, Visual Appearance also redies there.
- MpistoSkin2 is a GMK skin that has many wrappers and is semi-dynamical. Evelution is however, a MediaWiki skin with reliance on Mustache and much more dynamical. Because of this, the custom appearance of Preferences Screen is unavailable on Evelutiion but the ones from core MW is at least themed.

## Differences of Evelution and FandomDesktop
Evelution, despite being as a close-off to Fandom's new FandomDesktop, there're several differences, to name a few:
- Evelution uses breakpoints to define its appearance, like Oasis but unlike FandomDesktop
- Unlike FandomDesktop where FandomMobile is the Mobile segment of FandomDesktop, Evelution has the mobile segment inside the skin. However, a more mobile optimized version with minimal formatting named Tunic is available.
- Evelution uses LocalStorage to store all skin-related settings (Theme Management, Article Width, Toolbar width and Sticky Nav width), unlike FandomDesktop which uses user preferences. As a result, those are tied to a specific browser for all users instead to a specific user for all browsers
- You have the ability to collapse the sticky nav, unlike FandomDesktop
- Toolbar appears as icon-only with tooltips and like Oasis but unlike FandomDesktop, it appears as a full-width container. It is uncustomizable as well but is loaded with many links
- Unlike FandomDesktop, no Global Footer exists. However, a small article footer does exist
- Evelution has no user avatar support, unlike FandomDesktop and such an icon takes place.
- Unlike FandomDesktop, no floating page actions exist. While server mode of Evelution gives something similar, it is completely unrelated.
- Unlike FandomDesktop, in Evelution you have double the amount of themes you can define in FandomDesktop and the light/dark mode toggle does not toggle between wiki themes but rather between Inverted Colors mode. Also, Evelution takes care of System's native dark mode, unlike FandomDesktop
- Page header on Evelution is completely different from the ones found in FandomDesktop but similar
- Global Nav is mostly unbranded, is smaller and is themed. Also, search is not opened as a modal but rather as dropdown in the global nav. In addition global nav links do not include text below the icon and instead have tooltips.
- Evelution, unlike FandomDesktop uses pure JS to control theming and theming variables can be changed with ease. All background-related options are accesed with CSS variables as well. Several attributes to the body element are put as well. Users can also force specific color scheme or use different premade visual styles.
  - Evelution is, however compatible with **ALL** Fandom theming CSS variables. However, they're aliased to existing CPE Language variables, so instead of having the behavior seen in FandomDesktop, they have essentially the same behavior from CPE Language System.

## What are the different sizes I can use?
Evelution gets powered up with six main sizes: 320 pixels for small phones, 375 pixels for medium phones, 425 pixels for large phones 705 pixels for small desktops, 1280 pixels for large desktops and 1500 pixels for extra large desktops. A middle breakpoint size also exists. Users are able to read articles in either fixed width or full width, whichever they want to use.

With the inclusion of a top Sticky Navigation and a Bottom Toolbar which both can be collapsed, things can become more fun

The local navigation on Evelution is fetched from ``MediaWiki:Sidebar``. It is placed as links on the ``.color-nav`` container on the static navigation and as submenus of another menu on the sticky navigation called ``.mpisto-sticky-header-container``

## What are the differences between the Small and Large Sizes?
The small 705 breakpoint contains the following differences from the large 1280 ones:
  - Text Size on Community and Sticky headers is smaller
  - No wordmark appears on either header
  - Less content can be seen compared to the large ones

Other than these three changes, both sizes can be used for reading articles. For medium-sized devices, a breakpoint that mixes the small breakpoint with the large ones is present and has the following gimicks:
  - Wordmark appears on either header but on the static ones, it appears smaller
  - Text sizes are a bit smaller compared to the larger ones
  - 
When customizing the skin using CSS, please make sure that when you edit the body background image, don't use the ``body`` element. Use ``.body-community-background`` instead if you want to change the background even more.

## Is there a native dark mode?
Yes. Evelution not only offers many dark themes but also an Inverted Colors Mode. This is offered in Solo theme mode (Strictly light or dark themes) and Duo theme mode (Light/Dark themes). State of Inverted Colors is reversed when system's native dark mode is active. Color invertion is powered by **Liatch** With **Liacth** phenomenon running (Based on value of Inverted colors):
  - All static background colors (Except Caret Color) are getting a partial invertion to make them play nice under this mode
  - Anchor Background Color, Static Page Border Background Color and Accent Background Color are color edited versions of the original if them won't play nice under Page Text Background Color as the role of Page Background Color
  - Community Background Image gets inverted to improve legibility of Community Header

## Can I change the themes using CSS?
Of course. It has been tested and it works. For instance, if you want to modify the 2nd theme, paste this to ``MediaWiki:Common.css``:
```css
[theme="B"][visualcolors="standard"] {
--community-background-image:url("");
--community-background-color:#e995ca;
--anchor-background-color:#058892;
--page-background-color:#ffffff;
--page-border-background-color:#ccc;
--page-text-background-color:#000000;
--accent-background-color:#18BBC5;
--sticky-header-background-color:#0000ff;
--toolbar-background-color:auto;
}
```
Per-page theming is also supported. If you want to use a different theme for the 1st theme on **Sample Test Page** article, paste this to ``MediaWiki:Common.css``:
```css
[theme="A"][visualcolors="standard"].config-rootpage-Sample_Test_Page {
--community-background-image:url("");
--community-background-color:#e995ca;
--anchor-background-color:#058892;
--page-background-color:#ffffff;
--page-border-background-color:#ccc;
--page-text-background-color:#000000;
--accent-background-color:#18BBC5;
--sticky-header-background-color:#0000ff;
--toolbar-background-color:auto;
}
```

## Testing your themes against color contrast
When checking your themes, you must be in Duo theme mode without inverted colors on as Liatch (Such as Duo theme mode with Inverted Colors enabled) will modify the theme to avoid any color contrast issue

## Theming Variables
This section lists all static Theming Variables and where they're used:

### ``--community-background-image`` (Accepts: ``<image>``)
This is used as the background image of the body container. When the opposite version of that theme is being running, this will appear inverted. An empty value results in no background being shown.

### ``--community-background-image-opacity`` (Accepts: ``<percentage>``)
This is used as the opacity of the body background image. 0% makes it invisible, 50% makes translucent and 100% makes it visible.

### ``--community-background-color`` (Accepts: ``<color>``)
This is used as the background color of the body container and the gradient overlay shown on header backgrounds. This is also used on  ``is-headline`` buttons.

### ``--community-header-text-color`` (Accepts: ``<color> | auto``)
This is used as the foreground color of the Community Header. When set to ``auto``, it autopicks the computed foreground community color.

### ``--community-background-mode`` (Accepts: ``standard | full``)
When set to ``standard``, community background spans to the header area only. When set to ``full``, communnity background spans to the whole screen.

### ``--community-background-horizontal-alignment`` (Accepts: ``left | center | right``)
Sets the horizontal alignment of the background image. Accepts all standard properties ``background-position-x`` supports.

### ``--community-background-vertical-alignment`` (Accepts: ``top | center | bottom``)
Sets the vertical alignment of the background image. Accepts all standard properties ``background-position-y`` supports.

### ``--community-background-size`` (Accepts: ``cover | contain | stretched | full``)
When set to ``cover``, it makes the background image display on the whole screen, clipping some parts of it. When set to ``contain``, it behaves like cover except that no clipping happens in which it can reveal the community background color. When set to ``stretched``, it behaves like contain except that the background image will be stretched to remove any bg color revealance. When set to ``full``, it dispalys the background image as it is (Without changing its size).

### ``--community-background-no-horizontal-tiling`` (Accepts: ``<boolean>``)
When set to ``true``, it removes background tiling on the horizontal axis

### ``--community-background-no-vertical-tiling`` (Accepts: ``<boolean>``)
When set to ``true``, it removes background tiling on the vertical axis

### ``--anchor-background-color`` (Accepts: ``<color>``)
This is used as the color of the links, checkboxes and range inputs. This is also used on  ``is-alternate`` and secondary OOUI buttons.

### ``--page-background-color`` (Accepts: ``<color>``)
This is used as the background color of the page container, rail modules and many more containers.

### ``--page-border-background-color`` (Accepts: ``<color> | auto``)
This is used as the border color of the page container, rail modules and many more containers.  When set to ``auto``, it autopicks a color based on page background color.
 This is also used on  ``is-borderline`` buttons.

### ``--page-text-background-color`` (Accepts: ``<color> | auto``)
This is used as the border color of the page container, rail modules and many more containers.  When set to ``auto``, it autopicks either the light or dark text background color, whichever works best on the set page background color.
 This is also used on  ``is-colorline`` buttons.

### ``--accent-background-color`` (Accepts: ``<color>``)
This is used as the color of the buttons, selected text in Contrast and Classic visual styles, primary OOUI buttons and hovered and focused input styles without extra class

### ``--sticky-header-background-color`` (Accepts: ``<color>``)
This is used as the color of the sticky header navigation and since 11.17.6 as the color of the toolbox. This is also used on  ``is-titleline`` buttons.


### ``--toolbar-background-color`` (Accepts: ``<color> | auto``, until 11.17.5)
This was used as the color of the toolbox.  When set to ``auto``, it autopicked a color based on page, accent and sticky header background colors. This was also used on  ``is-intitleline`` buttons.

### ``--caret-color`` (Accepts: ``<color> | auto``)
This is used as the color of the insertation caret.  When set to ``auto``, it autopicks the text color of the editable element.


### ``--custom-secondary-font`` (Accepts: ``<family-name>``)
This is used as the extra secondary font to be used other than the stock ones. When set to an empty quoted string, no special extra font is used.

### ``--border-radius`` (Accepts: ``<length>``)
This is used to control the rounded corners of all supported elements. 0px removes the rounded corners entirely. Values between 0 to 15px are generally favored.


### ``--logo-filter`` (Accepts: ``<filter-function>``)
This is used as the base filter of the logo.

### ``--logo-filter-hover`` (Accepts: ``<filter-function>``)
This is used as the base filter of the logo when hovering on it. When set to empty, it fallbacks to the base logo filter.

### ``--logo-filter-duration`` (Accepts: ``<time>``)
This is used as the time needed to transition from the base filter to the hover filter and vice versa. 0ms removes the transition. Values between 0ms to 1000ms are generally favored.

### ``--logo-filter-delay`` (Accepts: ``<time>``)
This is used as the time needed to start the transition from the base filter to the hover filter and vice versa. 0ms removes the delay. Values between 0ms to 1000ms are generally favored.

## Configuring Evelution
Evelution, being a Mustache-powered MW skin, does support a few configurations, standard and non-standard, to name a few:

### Logo (Since 1.0.0)
Evelution uses ``$wgLogo`` to fetch the logo. If ``$wgLogos[icon]`` exists, then that setting will be used to fetch the logo. If none of them are found, no logo is shown. Note that any size works, and it can also be an SVG image in addition to a PNG ones. This logo appears on Desktop and Sticky community headers on the Large Size onwards

### Wordmark (Since 5.3.0)
By default, Evelution writes the sitename next to the wordmark. If you want to use your own mark instead of the default text ones, set the ``$wgLogos[wordmark]`` property on LocalSettings.php. Note that the wordmark set must be at most 40px in height for best results and it will appear monochrome so as it can adapt any text color. This wordmark appears on all places the default text-mark would appear otherwise so.

### ``$wgEvelutionLeftPersonalLinks`` (Since 4.3.0)
Defaults to false. When set to true, it allows you to align the toolbar links to the left.

### ``$wgEvelutionDisableColorManagement`` (Since 4.3.0)
Defaults to false meaning you have color management, When set to true, it hardcodes the color scheme used on Evelution to be similar to the ones used in Vector. This setting is useful for wikis that can't adapt to the many color schemes Evelution gives.

### ``$wgEvelutionForceOneHeader`` (Since 4.3.0)
Defaults to false. When set to true, it removes the Desktop Community Header and leaves the Desktop sticky header the only ones for Desktops. This setting does not affect Mobile Devices. This setting is useful for wikis who want a solo header layout. Sticky header is still able to be collapsed.

### ``$wgEvelutionDisableRightRail`` (Since 5.0.0)
Defaults to false meaning that a right rail will be shown where appropriate. When set to true, no right rail will appear. If the wiki heavily relies on layouts that might break with the Right Rail on, this setting is very useful to be turned on.

### ``$wgEvelutionServerMode`` (Since 5.1.0)
Defaults to false aka Home Mode. When set to true aka Server Mode, it changes the layout to be more server/development wikis-friendly: 
- No Desktop Local Navigation
- Addition of Left actions link before the content (Which has the local navigation menus)
- Smaller page header title
- Full width Small Breakpoint size 
- No right rail on Help and Project Namespaces

### ``$wgEvelutionCustomFont`` (Since 5.3.0)
Defaults to an empty string meaning Didact Gothic will be used. When set to another value, that font will be used instead

### ``$wgEvelutionIconStyle`` (Since 5.5.0, until 6.1.0)
Defaulted to outlined. When set to either filled, rounded, shart or two-tone, it changed the icon display to a style other than outlined. Values outside the allowed ones would result in outlined icons. It did not affected OOUI and Inline SVGs but did affected Material Icons inserted on articles.

### ``$wgEvelutionIconWireframe`` (Since 6.2.0, until 8.0.0)
Defaulted to true aka outlined Icons. When set to false, icons would display filled aka without any wireframe

### ``$wgEvelutionStickyRail`` (Since 8.1.0)
Defaults to true aka right rail will be sticky. When set to false, right rail will not be sticky. In order for sticky behavior of right rail to appear, browser window size must be at least 960x600.
