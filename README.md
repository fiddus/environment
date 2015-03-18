# Development Environment Configuration


Here you will find how to set up you computer to better work on **Fiddus** projects.


## Bash Color Configuration

You will need terminal command line so you can turn it better for you day by day work. We have some suggestions about how you can setup your terminal. You can get help from some people who shared theirs scripts, click on their names and you can get code for a working bash color configuration. If you didn't like any of those with a little of work you can do your own.

> - [Mauricio Mercado](https://gist.github.com/maumercado/3354613)
> - [Jonathan Buchanan](https://gist.github.com/insin/1425703)
> - [Paul Gower](https://github.com/pmgower/Mac-Profile-Settings-bash/blob/master/.bash_profile)
> - [Nathaniel Landau](http://natelandau.com/my-mac-osx-bash_profile/)

1. Check if you have a .profile file

        cd
        ls -alt

2. If you do have go to step 3, if you do not have this file create and open it

        touch .profile
        vim .profile

3. Paste or create your own bash configuration

        # With 'vim' opened
        # Type 'i' for insert some text
        # Write or paste the code you like
        # Type 'Esc' and after that 'wq' and 'Enter'


## Git

You will need git to manage your code versioning

1. Download git for your operation system ([Mac](http://git-scm.com/download/mac), [Linux](http://git-scm.com/download/linux) or [Windows](http://git-scm.com/download/windows)) and install it

2. Test if you have succeeded installing it

        # See git version
        git --version

        # If every thing went well you probably get some thing like the follow
        git version 1.8.5.2 (Apple Git-48)


## Graphical Client for Git

Git is a great tool but is better to see it in a graphical client, you can choose a graphical client for you operation system

> - GitX [Mac](http://rowanj.github.io/gitx/)
> - SourceTree [Mac and Windows](http://www.sourcetreeapp.com/)
> - GitHub [Mac](https://mac.github.com/), [Windows](https://windows.github.com/)
> - GitEye [Mac, Windows and Linux](http://www.collab.net/downloads/giteye)
> - GitG [Linux](https://wiki.gnome.org/Apps/Gitg/)
> - Giggle [Linux](https://wiki.gnome.org/Apps/giggle/)

## GitHub Account

To work with your team and every one know about a project you need a GitHub account. If you do not have a GitHub account follow this steps

1. Signup a [Gravatar](https://en.gravatar.com/) account. Although this is not necessary for GitHub it will assist you managing your personal information among many sites

2. Go to [GitHub](https://github.com/) and signup

3. In your terminal [generate your SSH key](https://help.github.com/articles/generating-ssh-keys)
        # Generate a key
        ssh-keygen -t rsa -C "your_email@example.com"
        # You can press 'Enter' on all questions

4. Get `id_rsa.pub` content

        # Go to your '.ssh' folder
        cd ~/.ssh
        # Show the 'id_rsa.pub' content
        cat id_rsa.pub

5. Add that content as a new key on [GitHub SSH keys](https://github.com/settings/ssh). As name for that key you can name your computer something like 'Fiddus laptop'

6. Test if this key worked

        # Testing ssh
        ssh -T git@github.com

        # Answer 'yes' to a warning
        The authenticity of host 'github.com (207.97.227.239)' can not be established.
        RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
        Are you sure you want to continue connecting (yes/no)?
        
        # You should get a message similar to the follow
        Hi username! You have successfully authenticated, but GitHub does not provide shell access.


## Text Editor

You can use a text editor of your choice: [Sublime Text](http://www.sublimetext.com/), [NotePad++](http://notepad-plus-plus.org/), [TextMate](http://macromates.com/), [Atom](https://atom.io/)

We suggest `Sublime Text`, because its easy configuration and because it has a great community

### Sublime Configurations

1. Install Sublime Package Control. It will help you install and uninstall packages on Sublime Text. Click [here](https://sublime.wbond.net/installation) to copy the package control installer code according your Sublime Text version.

2. Open Sublime Text and go to `View > Show Console` and paste on console the content copied from step before and press `Enter`

#### Sublime packages

Now you can install packages using `Ctrl + Shift + p` start typing `install`, select `Package Control: Install Package` and find a package you want to install

Suggested packages

> - [SublimeLinter](https://github.com/SublimeLinter/SublimeLinter-for-ST2)
> - [AngularJs](https://github.com/angular-ui/AngularJS-sublime-package)
> - [CSSLint](https://github.com/austinhappel/sublime-csslint)
> - [Emmet](https://github.com/sergeche/emmet-sublime)
> - [Hayaku](https://github.com/hayaku/hayaku)
> - [HTMLBeautify](https://github.com/rareyman/HTMLBeautify)
> - [AllAutocomplete](https://github.com/alienhard/SublimeAllAutocomplete)
> - [Git](https://sublime.wbond.net/packages/Git)
> - [SideBarEnhancements](https://sublime.wbond.net/packages/SideBarEnhancements)
> - [Puppet](https://sublime.wbond.net/packages/Puppet)
> - [BracketHighlighter](https://sublime.wbond.net/packages/BracketHighlighter)


#### Suggested Sublime Text user configuration `Preferences > User Settings`

     {
       "color_scheme": "Packages/Color Scheme - Default/Monokai Bright.tmTheme",
       "bold_folder_labels": true,
       "font_size": 13.0,
       "tab_size": 4,
       "translate_tabs_to_spaces": true,
       "trim_trailing_white_space_on_save": true,
       "ensure_newline_at_eof_on_save": true,
       "higlight_line": true,
       "scroll_past_end": true
     }

