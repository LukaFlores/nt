<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>


<!-- PROJECT LOGO -->

<div>
  <h2 align="center">Dotfiles (README not up to date)</h2>
  
  <p align="center"> 
    My life inside the terminal 💻 
  </p>
    <br />
  <p align="center"> 
    <img src="/resources/images/workspace.png" alt="Logo" width="700" height="450">
    <br />
    <img src="/resources/images/lazygit.png" alt="logo" width="700" height="450">
    <br />
  </p>

  <p align="center">
    <br />
    <a href="https://github.com/lukaflores/dotfiles/issues">Report Bug</a>
    ·
    <a href="https://github.com/lukaflores/dotfiles/issues">Request Feature</a>
  </p>
</div>


<!-- ABOUT THE PROJECT -->
## About The Project

Dotfiles are highly personalized to the individual. I encourage anyone who is starting the process of creating dotfiles to find inspiration in the others whilst starting from scratch. 

Note: Before installing, please look through the code and understand. It will alter prexisting configurations.


<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

You need to have [XCode](https://developer.apple.com/downloads/index.action?=xcode) or, at the very minimum, the [XCode Command Line Tools](https://developer.apple.com/downloads/index.action?=command%20line%20tools), which are available as a much smaller download.

The easiest way to install the XCode Command Line Tools in OSX 10.9+ is to open up a terminal, type 
  ```sh
    xcode-select --install
  ``` 

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/lukaflores/dotfiles.git
   ```
2. Move Repository to `~/code` 
   ```sh
    mv dotfiles ~/code 
   ```
3. Use install script (Don't provide a parameter to see options) 
   ```sh
   ./install.sh all
   ```
   

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage

### Tmux

To start a tmux session you can use the script: In Terminal `tm`
  or 
Use my Workspace template: In Terminal `tmuxinator ide`

#### Keybindings
Tmux Bind: `ctrl a`

In order to use following commands it must be prefaced by Tmux Bind
e.g `ctrl a + g`

- Open Lazy Git: `Tmux Bind + g`
- Move between Panes: `Tmux Bind + (h,j,k,l)` 
- Open Calcurse: `Tmux Bind + j`

### Nvim
The follwing commands are inside nvim, which can be enter through `vim .`

Initially you should install vim plugins with `:PlugInstall<cr>` inside vim
or 
In terminal with `vimu`

- Open File Drawer : `,k`
- Find Word Buffer : `,fg`
- Find File Buffer : `,ff` 
- Find File (FZF) : `,t`
- Find Recent File : `,fo`


### Latex

- Compile Latex File: `\ll`
- Open PDF viewer (Skim): `\lv`
- Open Error Buffer: `\le`

### Markdown

- Open Markdown Server: `,m `


<p align="right">(<a href="#readme-top">back to top</a>)</p>

### FreshRss

``
docker run -d --restart unless-stopped --log-opt max-size=10m -p 9090:80 -e TZ=America/Los_Angeles -e 'CRON_MIN=1,31' -v freshrss_data:/var/www/FreshRSS/data -v freshrss_extensions:/var/www/FreshRSS/extensions --name freshrss freshrss/freshrss
``




<!-- CONTACT -->
## Contact

Luka Flores - [@LukaFlores12](https://twitter.com/LukaFlores12)


<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* Inspiration [Niki Nisi Dotfiles](https://github.com/nicknisi/dotfiles)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
