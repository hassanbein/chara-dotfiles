## <h1 align="center"><img align="center" src="https://video-public.canva.com/VAD8lnOL18Q/v/d889ead9ee.gif" alt="sparkling star" height="30" width="40" /> Beautiful Rice and More Configs <img align="center" src="https://video-public.canva.com/VAD8lnOL18Q/v/d889ead9ee.gif" alt="sparkling star" height="30" width="40" /></h1>
>  :star2: :star2: Built with and inspired by great designs :star2: :star2:

### Credit & Acknowledgement

I want to acknowledge these wonderful people for inspiring me to make this config. Some helped by
providing the bootstrap of some components, some by suggesting better scripting styles and others by
recommending fixes and the logic structure to how things work. Without them, this might not have been
possible.

|               Name                |               Support             |               Socials             |
|:----------------------------------|:----------------------------------|:----------------------------------|
| Sidhanth Rathod                   | His riced dwm bootstrap called [chadwm](https://github.com/siduck/chadwm) was my inspiration      |<a href="https://matrix.to/#/@siduck:matrix.org" target="blank"><img align="center" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRh0HK0vPikdoBqarhpV5gdQq9DzUc25mUowB2EawNTrP7kWhelKhYG--ZskvzpKuWJGUg&usqp=CAU" alt="Sidhanth Rathod" height="30" width="40" /></a>  <a href="https://discord.com/users/600704648038580235" target="blank"><img align="center" src="https://www.svgrepo.com/show/353655/discord-icon.svg" alt="Sidhanth Rathod" height="30" width="40" /></a>  <a href="https://t.me/siduck" target="blank"><img align="center" src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Sidhanth Rathod" height="30" width="40" /></a> <a href="https://github.com/siduck" target="blank"><img align="center" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="siduck" height="40" width="40" /></a> |
| Gyen Abubakar Sadick              | Reviewed rices and made countless great suggestions |<a href="https://twitter.com/gyenabubakar" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="Gyen Abubakar" height="30" width="40" /></a>  <a href="https://linkedin.com/in/gyenabubakar" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="gyen abubakar" height="30" width="40" /></a>  <a href="https://github.com/gyenabubakar/gyenabubakar" target="blank"><img align="center" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="gyenabubakar" height="40" width="40" /></a>  <a href="https://hashnode.com/@gyenabubakar" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/hashnode.svg" alt="gyen abubakar" height="30" width="40" /></a>|
| Alkis Georgopoulos                | Contributed greatly to the wal script for setting random wallpapers      |<a href="https://matrix.to/#/@alkis:matrix.org" target="blank"><img align="center" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRh0HK0vPikdoBqarhpV5gdQq9DzUc25mUowB2EawNTrP7kWhelKhYG--ZskvzpKuWJGUg&usqp=CAU" alt="Alkis Georgopoulos " height="30" width="40" /></a>  <a href="https://github.com/alkisg" target="blank"><img align="center" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="alkisg" height="40" width="40" /></a> |
---

### Install Guide
This script is made for Linux platform-based machines that utilize the `aptitude` package manager. Maybe some
time later, I will consider releasing support for other package managers for Linux.

> To install, simply run the folowing command:

```bash
bash <(curl -s https://raw.githubusercontent.com/CharaD7/chara-dotfiles/main/install.sh)
```

> The document and config follows the structure below:
 - Git installation verification and setup
   - Git configuration on user confirmation
 - Installing NerdFonts
 - Installing and setting up the fish terminal
 - Installing and setting up the tmux terminal
 - Installing [Sidhanth Rathod](https://github.com/siduck/bubbly)'s bubbly widget on user confirmation
 - Installing and setting up neovim and neovide
 - Installing and setting up dwm

___

## :cop: Git :cop:


https://github.com/CharaD7/chara-dotfiles/assets/9804780/7b3c9776-9740-4ae5-a686-003e383d4b22


<details>
    <summary>After user permits the setup of git aliases, user will be able to execute git several calls using shortcuts</summary>

   > - `git init` is aliased `g i`
   > - `git fetch` is aliased `g f`
   > - `git clone` is aliased `g cl`
   > - `git fetch origin +refs/pull/*/head:refs/remotes/origin/pr/*` is aliased `g pr`
   > - `git remote add origin` is aliased `g rao`
   > - `git remote set-url origin` is aliased `g rso`
   > - `git commit -m {message}` is aliased `g acm {message}`
   > - `git commit --amend -m {message}` is aliased `g aca {message}`
   > - `git checkout` is aliased `g c`
   > - `git config --get user.name` is aliased `g cn`
   > - `git config --get user.email` is aliased `g ce`
   > - `git checkout main` is aliased `g con`
   > - `git checkout -b` is aliased `g cob`
   > - `git checkout --orphan` is aliased `g co`
   > - `git branch` is aliased `g b`
   > - `git branch -r` is aliased `g br`
   > - `git branch -m` is aliased `g brn`
   > - `git branch -a` is aliased `g ba`
   > - `git branch --merged` is aliased `g bm`
   > - `git branch --no-merged` is aliased `g bn`
   > - `git diff` is aliased `g df` *Note that this is an advance git diff that uses peco, hist and awk*
   > - `git log --pretty=format:\"%Cgreen%h %Creset%cd %Cblue[%cn] %Creset%s%C(yellow)%d%C(reset)\" --graph --date=relative --decorate --al` is aliased `g hist`
   > - `git log --graph --name-status --pretty=format:\"%C(red)%h %C(reset)(%cd) %C(green)%an %Creset%s %C(yellow)%d%Creset\" --date=relative` is aliased `g llog`
   > - `git !hub browse` is aliased `g open`
   > - `git remote -v` is aliased `g r`
   > - `git remote rm origin` is aliased `g rmo`
   > - `git branch -d` is aliased `g bd`
   > - `git branch -D` is aliased `g bD`
   > - `git push` is aliased `g p`
   > - `git pull origin` is aliased `g pl`
   > - `git pull --all` is aliased `g pa`
   > - `git push origin main` is aliased `g pon`
   > - `git pull origin main` is aliased `g plon`
   > - `git push origin` is aliased `g po`
   > - `git status` is aliased `g s`
   > - `git push -f origin HEAD^:main` is aliased `g undopush`
   > - `git merge main` is aliased `g mn`
   > - `git merge` is aliased `g m`
   > - `git reset --hard HEAD@{1}` is aliased `g undomerge`
   > - `git reset --hard` is aliased `g undo`
   > - `git reset HEAD {file}` is aliased `g unstage {file}`
</details>

___

## :honey_pot: NerdFonts - [Nice ligature fonts] :honey_pot:

[NerdFonts](https://www.nerdfonts.com) is a home of great and beautiful wide range of fonts.

<details>
    <summary>To give you the best of ligature feel and look, the following fonts have been used in this setup:</summary>

   > - Caskaydia Cove NerdFont
   > - Fira Code NerdFont
   > - FiraCode iScript
   > - Hurmit NerdFont *Bonus Font that has not been used in this setup*
   > - Iosevka NerdFont
   > - Jetbrains Mono NerdFont
   > - MaterialDesignIconsDesktop Font
   > - Roboto Mono NerdFont

   These fonts can be located in the [NerdFonts directory](https://github.com/CharaD7/chara-dotfiles/tree/main/NerdFonts)
</details>

___

## :fish: Fish :fish:

https://github.com/CharaD7/chara-dotfiles/assets/9804780/324b41a7-729a-4184-8802-bbdafc792238

[Fish](https://fishshell.com) shells is one of the best shells to use as a developer if [VIM](https://vim.org) is your preferred IDE. It
has been made such that there is a mode you can switch to in order to emulate [VIM](https://vim.org) commands,
making you the developer super-productive. To learn more about scripting with fish, kindly visit the [docs](https://fishshell.com/docs/current/index.html).

<details>
    <summary>The fish config script installs a couple of packages to make your experience with fish seemless:</summary>

   > - [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish) *My fish is not lost* :smirk:
   > - [fisher](https://github.com/jorgebucaran/fisher/tree/main) - A package manager for fish
   > - [z](https://github.com/jethrokuan/z) - A directory jumper that can be installed using [fisher](https://github.com/jorgebucaran/fisher/tree/main)
   > - [powerline-config](https://powerline.readthedocs.io/en/master/installation.html#patched-fonts) - A python-based font patcher for terminals
   > - [bobthefish](https://github.com/oh-my-fish/theme-bobthefish) - A theme for the fish terminal
   > - [ghq](https://github.com/x-motemen/ghq) - A repository organizer, very handy when you work with a lot of them and can't structure it easily.
   > - [exa](https://the.exa.website/) - A mordern replacement for `ls` with rich features
   > - [peco](https://github.com/peco/peco) - A fuzzy finder plugin for fish terminal

   **NB:** Go to the [fish config's aliases](https://github.com/CharaD7/chara-dotfiles/blob/main/fish/config.fish) to see which aliases are registered for the fish shell.
   *To emulate vim movement and Visual key bindings, hit the `<Escape>` key. Hit `i` to get back into edit mode*
</details>

___

## :pager: TMUX :pager:

 ![tmux](https://github.com/CharaD7/chara-dotfiles/assets/9804780/c1eba1d3-3591-4c7b-99f4-5dc1d36b89d2)

[tmux](https://github.com/tmux/tmux/wiki) is a terminal multiplexer, allowing you to switch between several programs, detach and reattach them in
different programs, it proves to be one of the best terminals out there. to know more about it and how to easily navigate your way while using it,
go to read the [docs](https://github.com/tmux/tmux/wiki/Getting-Started). This repo's `tmuxConfig` script comes with powerline fonts and a script
to run and configure tmux to have the status bar as you see it in the above picture. To know more about the key combinations, I recommend using the
section on [key moodifiers](https://github.com/tmux/tmux/wiki/Modifier-Keys). However, the [setup](https://raw.githubusercontent.com/CharaD7/chara-dotfiles/main/.tmux.conf)
comes with predefined key bindings you may want to take a look at the [tmux conf](https://raw.githubusercontent.com/CharaD7/chara-dotfiles/main/.tmux.conf)
file.

___

## :full_moon: Neovide - [No nonsense IDE] :full_moon:

 ![neovide](https://github.com/CharaD7/chara-dotfiles/assets/9804780/a3ce5a06-e8f0-4b17-9596-f9d40dc8cc52)

https://github.com/CharaD7/chara-dotfiles/assets/9804780/7bef1b54-c233-46cb-85e9-5d1f628468f1


[Neovide](https://neovide.dev) is a no-nonsense, cross-platform graphical user interface for [Neovim](https://github.com/neovim/neovim) (an awesome IDE that
is open source and seeks to aggresively refactor [VIM](https://www.vim.org/)). Supporting a lot of very cool [features](https://neovide.dev/features.html),
it promises a wonderful future of an extensible, yet, very stable IDE for vimmers like myself. The [Neovide](https://neovide.dev) graphical user interface though
intuitive, does not work off of its own, it needs a [Neovim](https://github.com/neovim/neovim) ```init.lua``` or ```init.vim``` file to work and so you may want to
consider having that before using this beauty 😎 That said, this [nvimConfig](https://raw.githubusercontent.com/CharaD7/chara-dotfiles/main/configNvim) comes with
some features of [Neovide](https://neovide.dev) configured to make your experience using the IDE awesome ✨

<details>
    <summary>Below is a list of the features enabled and how they are used:</summary>

   > - Ligature Support *(enabled by default)*
   > - Animated Cursor - ```vim.g.neovide_cursor_animation_length = 0.13``` *(set to 0.13seconds)*
   > - Animated Cursor Particles - ```vim.g.neovide_curosr_vfx_mode =  "railgun"``` *(Leave animated particles anytime cursor jumps around)*
   > - Smooth Scrolling - *(enabled by default)*
   > - Animated Windows - *(enabled by default)*
   > - Transparency - ```vim.g.neovide_transparency = 0.8``` *(you can increase the opacity as you like it)
   > - Blurred Floating Windows - ```vim.g.neovide_floating_blur_amount_x = 4.0``` and ```vim.g.neovide_floating_blur_amount_y = 4.0```
   > - Emoji Support - *(enabled by default)*
   > - IDE Paddings - ```vim.g.neovide_padding_[direction] = 10``` *(substitute **[direction]** for **top**, **bottom**, **left** and **right**)*

   You can take a peek at the features enabled using the [permalink](https://github.com/CharaD7/chara-dotfiles/blob/2119a40ee647ae530261c916cd184424a5b7d44c/nvim/lua/chara/options.lua#L88)

   **NB:** I have enabled autosave on every edit and on focus lost by default in this config. If it is bothersome to you, come to [this block](https://github.com/CharaD7/chara-dotfiles/blob/2119a40ee647ae530261c916cd184424a5b7d44c/nvim/after/plugin/autocommands.lua#L58)
   and comment it out.
</details>

___

## :gem: DWM - [Tiling Window Manager] :gem:

[DWM](https://dwm.suckless.org/) (Dynamic Window Manager) is a window manager for X. It displays windows in several layouts such as
tiled, monocle and floating. It is more convenient to use though requires some work if you need it to look beautiful and want to
use your custom keybindings to invoke certain calls or programs. There are several [patches](https://dwm.suckless.org/patches/) available
on the [suckless](https://dwm.suckless.org) site that can be added to the config to suit user's taste.

<details>
    <summary>Included in this config is the following plugins:</summary>

   > - [picom](https://gist.github.com/AvishekPD/f70dea1449cfae856d42b771912985f9) - for managing rounded corners and opacity of windows
   > - [rofi](https://github.com/davatorium/rofi) - a window switcher, application launcher and replacement for dmenu
   > - [eww](https://elkowar.github.io/eww/) - Elkowar's Wacky Widgets for dwm
      > - bubbly - *(concept made from siduck's bubbly widget)*
      > - dashboard - *(concept made from siduck's chadwm riced dwm)*

   **NB:** You may have to reconfigure your bubbly and dashboard to work perfectly based on your display. I had to reconfigure bubbly and dashboard
   before I got them to work as my inspirations but thankfully enough, I have highlighted where the changes can be made and how to change the values
   as you would like.

   *(I really thank [Sidhanth Rathod](https://github.com/siduck) for inspiring me to come with this compillation. You are such a beautiful gem.)

   ### Picom

   The [picom](https://raw.githubusercontent.com/CharaD7/chara-dotfiles/main/picom/picom.conf) plugin will automatically be saved to your `~/.config/picom` directory, as such, any
   changes you wish to make to the window transparency, blur or corners should be done in the `~/.config/picom/picom.conf` file. You can also make changes to the animation of windows
   in the same file. Here is a highlight of what you can change in picom

   > - The [animation](https://github.com/CharaD7/chara-dotfiles/blob/41ff240d832bbd6cc25b64e57c9406be17729fc6/picom/picom.conf#L1)
   > - The [corners](https://github.com/CharaD7/chara-dotfiles/blob/41ff240d832bbd6cc25b64e57c9406be17729fc6/picom/picom.conf#L14)
   > - The [shadows](https://github.com/CharaD7/chara-dotfiles/blob/41ff240d832bbd6cc25b64e57c9406be17729fc6/picom/picom.conf#L37)
   > - The [fades](https://github.com/CharaD7/chara-dotfiles/blob/41ff240d832bbd6cc25b64e57c9406be17729fc6/picom/picom.conf#L112)
   > - The [transparency/opacity](https://github.com/CharaD7/chara-dotfiles/blob/41ff240d832bbd6cc25b64e57c9406be17729fc6/picom/picom.conf#L144)
   > - The [blur](https://github.com/CharaD7/chara-dotfiles/blob/aae40ed4f6cac8922601d6c28c0f4ca1d1b638de/picom/picom.conf#L222)
   > - General [render](https://github.com/CharaD7/chara-dotfiles/blob/aae40ed4f6cac8922601d6c28c0f4ca1d1b638de/picom/picom.conf#L285)

</details>
