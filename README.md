# EdgyArc-fr

Because Arc and Edge look pretty af but FOSS FTW

![Screen Shot 2024-05-04 at 11 44 39 PM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/6f0879fa-f08b-4e36-91dd-29e321f81193)

### This branch only supports Firefox v137+. For older versions, please see the [v136 branch](https://github.com/Loskir/EdgyArc-fr/tree/v136).

## Features

- Based on [Edge-frfox](https://github.com/bmFtZQ/edge-frfox)
- Sidebar Modifications
  - Auto-collapse sidebar into just icons
  - Auto-hide sidebar
  - Toggle sidebar show/collapse _(using [UserChrome Toggle](https://addons.mozilla.org/firefox/addon/userchrome-toggle/))_
- `macOS only` Translucent windows
- Custom Sidebery theme
- Auto-hide native top tabs when Sidebery or TST is active

## Differences compared to artsyfriedchicken/EdgyArc-fr

- The code is formatted with prettier (easier to maintain and contribute)
- The color scheme from edge-frfox is disabled by default (can be enabled with `af.edgyarc.edge-styles`)
- The shadow around the content is disabled making it more consistent
- Various fixes (centered url, rounded corners, margins)
- New option `af.edgyarc.separate-extended-urlbar`
- New option `uc.tweak.hide-tabs-bar.always` that permanently hides native tabs
- Proper translucency support for Sidebery (introduced in FF 130.0)
- Noise texture background tweak
- `af.edgyarc.autohide-sidebar-slide`
- Support for Firefox v137+

## Usage

### Step 1 - Installation

<details>
  <summary> 🔵 Install recommended addons </summary>

- [Sidebery](https://addons.mozilla.org/firefox/addon/sidebery/)
- [UserChrome Toggle](https://addons.mozilla.org/firefox/addon/userchrome-toggle/) `Required for sidebar autohide`
- Optional Addons:
  - [Adaptive Tab Bar Color](https://addons.mozilla.org/en-GB/firefox/addon/adaptive-tab-bar-colour/)
    `[OR]`
  - [Firefox Color](https://addons.mozilla.org/en-US/firefox/addon/firefox-color/)

</details>

<details>
  <summary> 🔵 Install and Configure Base theme </summary>
  
  - Clone or download the repository to your local machine.
  - Copy the contents of the `chrome` folder into your Firefox profile's `chrome` folder.
  - Go to `about:config` and set these properties to `true`

    `toolkit.legacyUserProfileCustomizations.stylesheets`

    `svg.context-properties.content.enabled`

    `layout.css.color-mix.enabled`

    `layout.css.light-dark.enabled`

    `layout.css.has-selector.enabled`

    `widget.macos.titlebar-blend-mode.behind-window` [Required for translucency on macos]

    `browser.tabs.allow_transparent_browser` [Required for translucency on macos]

- Set these properties to `true` as well

  `uc.tweak.hide-tabs-bar`

  `uc.tweak.rounded-corners`

</details>

### Step 2 Configure EdgyArc

<details>
<summary>Although the theme can be used as is, you can customize some aspects of it</summary>

| Feature Description                                                                                                                                                                        | Screenshot                                                                                                                                      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Translucent Effects** `macos Only` <br> `af.edgyarc.macos-translucent`                                                                                                                   | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/dd122094-0545-4145-9733-ef9776b40a6b">                             |
| **More Translucent** <br> `af.edgyarc.macos-more-translucent`                                                                                                                              |                                                                                                                                                 |
| **🔵 UI Tweaks**                                                                                                                                                                           |                                                                                                                                                 |
| **Always hide native tabs** <br> `uc.tweak.hide-tabs-bar.always` <br>                                                                                                                      | ![uc.tweak.hide-tabs-bar.always](https://github.com/user-attachments/assets/4b528bf3-b920-4bd2-8c35-3701210cae14)                               |
| **Separate extended URL bar** <br> `af.edgyarc.separate-extended-urlbar` <br> ❗ Does not work well with `af.edgyarc.thin-navbar`                                                          | ![af.edgyarc.separate-extended-urlbar](https://github.com/user-attachments/assets/6cc3cd72-2459-4a9c-95ef-93285c57b4fe)                         |
| **Noise texture background** <br> `af.edgyarc.noise-texture`                                                                                                                               | ![af.edgyarc.noise-texture](https://github.com/user-attachments/assets/1dc41944-4dcf-480a-9f12-f424169adf12)                                    |
| **Thin Navigation Bar** <br> `af.edgyarc.thin-navbar`                                                                                                                                      | ![Screen Shot 2024-05-04 at 11 52 25 PM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/0b030f04-c10d-48a2-8462-b61c52e4f8de) |
| **Minimal Navigation Bar**<br> `af.edgyarc.minimal-navbar`                                                                                                                                 | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/1e56cc7c-1b54-4602-b825-b68000f6f92c">                             |
| **Greyscale webextensions icons** <br> `uc.tweak.af.greyscale-webext-icons`                                                                                                                | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/7e3c4b3d-43ae-4a5e-bdbb-f067105ee346">                             |
| **Centered URL** <br>`af.edgyarc.centered-url`                                                                                                                                             | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/aa9a89cb-320f-434c-b66d-8b474bfbdc0a">                             |
| **🔵 Sidebar Tweaks**<br> ⚠️ Note: Requires [UserChrome Toggle](https://addons.mozilla.org/firefox/addon/userchrome-toggle/) to <br>make use of auto-collapse/auto-hide                    |                                                                                                                                                 |
| **Enable Sidebery Theme** <br> `af.sidebery.edgyarc-theme`                                                                                                                                 | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/504574e5-609b-4192-b061-fc29caea7c48">                             |
| **Sliding hidden sidebar**<br> `af.edgyarc.autohide-sidebar-slide`                                                                                                                         | <video src="https://github.com/user-attachments/assets/a68b3416-4708-44b6-a410-ae2db6c041ef">                                                   |
| **Minimal Sidebery when Collapsed**<br> `af.sidebery.minimal-collapsed`                                                                                                                    | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/84ccb725-3ca9-4332-82a7-b9dc17909d5b">                             |
| **Edge-like Sidebar** <br> `af.edgyarc.edge-sidebar`                                                                                                                                       | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/7216bcd1-ac58-4264-ba83-61db7f342db0">                             |
| **Show Sidebar Header** <br> `af.edgyarc.show-sidebar-header`                                                                                                                              | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/e72e9f59-e49d-4f79-ad9b-fc12b3f56bcc">                             |
| **Auto-Hide Sidebar**<br> `af.edgyarc.autohide-sidebar`<br> **_Note: Requires [UserChrome Toggle](https://addons.mozilla.org/firefox/addon/userchrome-toggle/) to work_**                  | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/cfa7a899-6bb1-4058-be12-9e95a10cd981">                             |
| **Sidebar Always Collapsed** <br> `af.edgyarc.sidebar-always-collapsed` <br> **_Note: Requires [UserChrome Toggle](https://addons.mozilla.org/firefox/addon/userchrome-toggle/) to work_** | <video src="https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/06c9c876-43d4-490f-a766-0d2b6f4de2f8">                             |
| **Wider Expanded Sidebar on Hover** <br> `uc.tweak.af.sidebar-width-350`                                                                                                                   |                                                                                                                                                 |
| **Sidebery Horizontal Navbar <br> on Top Tab List** <br> `af.sidebery.nav-on-top`                                                                                                          |                                                                                                                                                 |
| **Disable Dynamic Width Pinned Tabs**<br>`af.sidebery.static-pinned-tab-width`                                                                                                             |                                                                                                                                                 |

</details>

### Step 3 - Import Sidebery configs

Import the following into sidebery (`Sideberry Settings` > `Help` > `Import Addon Data`)

- `sidebery-settings.json` Contains settings for the addon that **will** overwrite your own settings. you dont _have_ to use this if you dont want to.
  **IF** you are not using `sidebery-settings.json` please make sure you have the following settings configured in Sidebery Settings

- General
  - Use Native Scroll Bars
    - Use thin Scroll Bars
- Context Menu
  - Render Icons
- Navigation Bar
  - Layout : `Horizontal`
  - Show Navigation Bar in one line: `Off` [OR `On` is you want a smaller more compact nav bar(beta11 and up)]
- Tabs
  - Tab Colorization
    - Colorize tabs: `Off`
    - Colorize Branches: `On`
- Appearance
  - Theme: `Proton`
  - Density: `Relaxed`
  - Color Scheme: `Firefox`

### Step 4 - Set up Adaptive Tab Bar Color settings

![Screen Shot 2024-05-04 at 11 18 47 PM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/2edfd163-5dc7-45fb-b8d4-53c83e278683)

## Known Bugs

- `windows` Translucency / blur does not work on windows
- `linux` Translucency / blur does not work out of the box

## Screenshots

![Screen Shot 2024-05-05 at 12 22 49 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/0f006a8a-a5d9-48a8-8a9e-7726a2fd0248)

![Screen Shot 2024-05-05 at 12 24 52 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/2597a88e-1d85-498c-9181-831296bdbf6d)

![Screen Shot 2024-05-05 at 12 41 02 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/d9f67cb2-8020-4a67-b7a6-c42157d28d28)

![Screen Shot 2024-05-05 at 12 40 44 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/df0b4223-6c5e-45ee-b193-b1e6979f0a68)

![Screen Shot 2024-05-05 at 12 39 48 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/f038c4a9-96cc-42b2-a583-91ab79c409f3)

![Screen Shot 2024-05-05 at 12 40 04 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/24fe7ec9-ed08-4c90-9271-44dfa3f3a53e)

![Screen Shot 2024-05-05 at 12 43 55 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/2c0b280b-3b17-4b16-839a-cb240eb63396)

![Screen Shot 2024-05-05 at 12 43 55 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/68f76e78-0af4-492d-8af1-a049e310eb25)

![Screen Shot 2024-05-05 at 12 42 38 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/6e487a81-7390-4fa7-b9f4-41ea5d36f0b5)

![Screen Shot 2024-05-05 at 12 43 02 AM](https://github.com/artsyfriedchicken/EdgyArc-fr/assets/100123017/8c37f4d8-5a2d-4b95-a847-5ac3810abaeb)

## Changelog

- v1.0.0-b10
  - Support for FF126 [for FF125 and lower, please continue using v1.0.0-b9]
  - Rewrote a large chunk of the code
  - Included copy of [Edge-frfox](https://github.com/bmFtZQ/edge-frfox) (v 24.4.18) for fewer version compatibility issues
- v1.0.0-b9
  - New
    - Added Thin navbar variant `uc.tweak.af.thin-navbar`
  - Fixed
    - Sidebery CSS (default background for pinned tabs)
    - Titlebar Controls positioning
- v1.0.0-b8

  - Fixed
    - findbar background colour when using firefox color/adaptive tab bar color addons
    - tab notification deck translucency `macOS`
    - toolbar height
    - padding in urlbar+reload button combo
    - Positioned window controls `Windows 10/11`
    - private window indicator `Windows 10/11`
  - Tweaks
    - uc.tweak.af.no-dimming makes sidebar have 100% opacity.
      Prequisite : translucency must be disabled using uc.tweak.af.not-translucent #14
    - tweaked margins and paddings `Windows 10/11`

- v1.0.0-b7
  - Cleaned up code
  - Fixed sidebery css bug - dragging tabs would indicate incorrect drop location
  - fixed sidebery css bug - pinned tabs misaligned
  - Added feature - Show a styled sidebar header
    `uc.tweak.af.show-sidebar-header` > `true`
  - Added feature - Turn all web extension icons greyscale when not hovered
    `uc.tweak.af.greyscale-webext-icons` > `true`
  - Css tweak - Toolbar background images now fade away at the bottom so it doesnt look jarring
  - Css fix - show custom private window badge when tabbar is hidden
  - Css fix - fixed margins and paddings of buttons inside the urlbar
  - bug fix - extension dropdown sheets inside the urlbar now show properly when urlbar is not hovered
- v1.0.0-b6
  - cleaned up code
  - bugfixes
  - updated sidebery styles
- v1.0.0-b5

  - Rewritten most of the code for translucency in macos
  - Added new preference uc.tweak.af.hidden-sidebar to fully hide sidebar when autohde is turned on in Userchrome Toggle
  - Added new preferenceuc.tweak.af.translucent-enable to control translucency [mac only]
  - Added new preference uc.tweak.af.translucent-enable to enable arc-like translucent sidebar
  - Tweaked sidebery css

- v1.0.0-b4
  - Supports Adaptive Tab Bar Color in translucent windows enabled!
- v1.0.0-b3
  - restyled horizontal navigation bar to make it look less crappy
  - coloured tabs only show colour behind favicon, and not the whole row
  - expand tab group icon now more visible
- v1.0.0-b2
  - added translucency support on macos
  - changed hover opacities and transitions on navigator-toolbox
  - fixed search bar placement in sidebery css
  - fixed 1px bug in sidebery css
- v1.0.0-b1
- initial release

## Issues and Contributions

If you encounter any issues or have suggestions for improvement, please [open an issue](https://github.com/Loskir/EdgyArc-fr/issues). Contributions are always welcome!

## License

This project is licensed under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
