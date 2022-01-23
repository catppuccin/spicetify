<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for Spicetify
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
    <a href="https://github.com/davidbgonz/spicetify/stargazers"><img src="https://img.shields.io/github/stars/davidbgonz/spicetify?colorA=1e1e28&colorB=c9cbff&style=for-the-badge&logo=starship style=for-the-badge"></a>
    <a href="https://github.com/davidbgonz/spicetify/issues"><img src="https://img.shields.io/github/issues/davidbgonz/spicetify?colorA=1e1e28&colorB=f7be95&style=for-the-badge"></a>
    <a href="https://github.com/davidbgonz/spicetify/contributors"><img src="https://img.shields.io/github/contributors/davidbgonz/spicetify?colorA=1e1e28&colorB=b1e1a6&style=for-the-badge"></a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/dev/assets/misc/sample.png"/>
</p>

## Usage

1. Follow the installation instructions for [Spicetify](https://spicetify.app/docs/getting-started/installation)
   * Note: The installation instructions for linux have you setting `/opt/spotify` and `/opt/spotify/Apps/*` permissions to `777`. This is not good practice and should be avoided. If you want, you can set the group ownership for these paths to one that your user is apart of (i.e. `users`), or you can create a new group and add your user to is as a secondary group. After that you can use the following command to give access to the group:
      ```
      GROUP=<group_name>
      sudo chgrp $GROUP /opt/spotify
      sudo chgrp -R $GROUP /opt/spotify/Apps
      sudo chmod 775 /opt/spotify
      sudo chmod 775 -R /opt/spotify/Apps
      ```
2. Follow the [basic usage](https://spicetify.app/docs/getting-started/basic-usage) to setup spicetify
3. Either clone this repo `git clone https://github.com/davidbgonz/spicetify.git ~/.config/spicetify/Themes/catppuccin` or copy over the `color.ini` and `user.css` files manually to a directory named `catppuccin` in the Spicetify theme directory. This is usually located in `~/.config/spicetify/Themes`
4. Update the following lines in `config-xpui.ini`:
    ```
    color_scheme            = lavender
    current_theme           = catppuccin
    ```
    Supported color schemes: `rosewater`, `flamingo`, `mauve`, `pink`, `maroon`, `red`, `peach`, `yellow`, `green`, `teal`, `blue`, `sky`, `lavender`
5. Run `spicetify apply` if Spotify is not open or `spicetify apply` to apply the theme and restart Spotify.


## 💝 Thanks to

- [Human](https://github.com/catppuccin)
