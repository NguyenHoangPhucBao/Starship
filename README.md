# **Custom your Terminal with Starship 🚀** #
This project makes your Termimal looks prettier 🤩🤩🤩

## ***Requirements📃*** ##
• Nerd Fonts : [NerdFonts](https://www.nerdfonts.com/ "NerdFonts")

##  ***Installation🔧*** ##
<details>
<summary>Windows</summary>

Scoop
```bash
    scoop install starhip
```

Winget
```bash
    winget install --id Starship.Starship
```
</details>

<details>
<summary>MacOs and Linux</summary>

Curl
```sh
    curl -sS https://starship.rs/install.sh | sh
```
</details>

## ***Configure Starship🔩*** ##
To get started configuring Starship, create the following file : ` ~/.config/starship/starship.toml `

```bash
    mkdir -p ~/.config/starship && touch ~/.config/starship/starship.toml 
```

All the configuration for Starship is done in this TOML file

## ***Setup to use Starship⚙️*** ##
(Becaue I use Powershell so I just config for Powershell 😁)
Run `$PROFILE` on your terminal to find location of the ps1 folder

Add the following to the end of the Powershell config:
```powershell
    Invoke-Expression (&starship init powershell)
```

### 📌 Config File Location ###
You can change default configuration file location with `STARSHIP_CONFIG` environment variable:

*put in your `$PROFILE`*
```powershell
    $ENV:STARSHIP_CONFIG = "path to your starship.toml file"
```
### 📌 Logging ###
*put this in you `$PROFILE`*
```powershell
    $ENV:STARSHIP_CACHE = "$HOME\AppData\Local\Temp"
```

## ***Documentation📖*** ##
🚀Starship Configuration : [here](https://starship.rs/config/) 

