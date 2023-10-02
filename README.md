<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for <a href="https://github.com/spicetify/spicetify-cli">Spicetify</a>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
    <a href="https://github.com/catppuccin/spicetify/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/spicetify?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/spicetify/issues"><img src="https://img.shields.io/github/issues/catppuccin/spicetify?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/spicetify/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/spicetify?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

![Spicetify Theme Preview](assets/preview.webp)

## Previews

<details>
<summary>🌻 Latte</summary>
<img src="assets/catppuccin-latte.webp"/>
</details>
<details>
<summary>🪴 Frappé</summary>
<img src="assets/catppuccin-frappe.webp"/>
</details>
<details>
<summary>🌺 Macchiato</summary>
<img src="assets/catppuccin-macchiato.webp"/>
</details>
<details>
<summary>🌿 Mocha</summary>
<img src="assets/catppuccin-mocha.webp"/>
</details>

## Usage

1. Follow the installation instructions for [Spicetify](https://spicetify.app/docs/getting-started) to setup Spicetify
   * Note: The installation instructions for linux have you setting `/opt/spotify` and `/opt/spotify/Apps/*` permissions to `777`. This is not good practice and should be avoided. If you want, you can set the group ownership for these paths to one that your user is apart of (i.e. `users`), or you can create a new group and add it as a secondary group to your user. After that you can use the following command to give access to the group:
      ```
      GROUP=<group_name>
      sudo chgrp $GROUP /opt/spotify
      sudo chgrp -R $GROUP /opt/spotify/Apps
      sudo chmod 775 /opt/spotify
      sudo chmod 775 -R /opt/spotify/Apps
      ```

2. Clone/Download the repository, and place the `catppuccin` folder (containing `user.css`, `theme.js`, `color.ini`, and `assets`) in the `Spicetify/Themes` directory:
      ```
      cp -r catppuccin ~/.config/spicetify/Themes/
      
      **For Windows users:**
      cp catppuccin "$(spicetify -c | Split-Path)\Themes\" -Recurse
      ```

3. Set theme and color scheme. Supported color schemes: `frappe`, `latte`, `macchiato`, `mocha`.:
   ```
   spicetify config current_theme catppuccin
   spicetify config color_scheme frappe
   spicetify config inject_css 1 inject_theme_js 1 replace_colors 1 overwrite_assets 1
   spicetify apply
   ```
4. To set an accent color, head over to Spotify's settings page and there will be a dropdown at the top.
<img src="assets/accents.webp"/>

## 📜 License

Catppuccin is released under the MIT license, which grants the following permissions:

-   Commercial use
-   Distribution
-   Modification
-   Private use

For more convoluted language, see the [LICENSE](https://github.com/catppuccin/catppuccin/blob/main/LICENSE).

## 💝 Thanks to

Creator:
- [davidbgonz](https://github.com/davidbgonz)

Maintainers:
- (Style) - [OlaoluwaM](https://github.com/OlaoluwaM)
- (Style) - [ghostx31](https://github.com/ghostx31)
- (Style/Extension) - [OhItsTom](https://github.com/ohitstom)

## 🌟 Community
Unofficial Catppuccin themes for Spicetify!

<details>
<summary><a href="https://github.com/Comfy-Themes/Spicetify/tree/main/Comfy#collection">Comfy</a></summary>
<img src="https://github.com/Comfy-Themes/Spicetify/raw/main/images/color-schemes/gif/catppuccin/mocha.gif"/>
</details>

<details>
<summary><a href="https://github.com/Aurn1ox/dots/tree/main/.config/spicetify/Themes/Ziro">Ziro</a></summary>
<img src="https://raw.githubusercontent.com/Aurn1ox/dots/main/assets/spotify-preview.png"/>
</details>

<p align="center"><img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" /></p>
<p align="center">Copyright &copy; 2022-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
<p align="center"><a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a></p>
