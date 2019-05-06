# Start development with Windows

> ~~Sometimes~~ _One time_ you need links and how to install it !!

- [Basic Tools](#basic-tools)
- [WindowsOs](#windowsos)
    - [Hidden files](#hidden-files)
- [GIT](#git)
- [Tools to create PR](#tools-to-create-pr)
- [Vscode](#vscode)
    - [Config](#config)
    - [Launch config](#launch-config)
    - [Plugins](#plugins)
- [Note](#note)
- [ToDO](#todo)

## Basic Tools

- [GIT](https://git-scm.com/download/win)

## WindowsOs

### Hidden files

- Open a terminal and type: `defaults write com.apple.finder AppleShowAllFiles YES`
- then relaunch your finder (using ctrl + click on finder icon)

From this [website](https://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/)

## GIT

- [autocompletion](https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion) 

    - `brew install git && brew install bash-completion`
    - copy this in `~/.bash_profile`

```bash
if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi
```

- Colored branches in `~/.bash_profile`

```bash
parse_git_branch() {
    git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1="\u@\h \W\[\033[32m\]\$(parse_git_branch)\[\033[00m\] $ "
```

## Tools to create PR

- [ImageOptim](https://imageoptim.com/) to optimize **EVERY** images
- [LICEcap](https://www.cockos.com/licecap/) to record your screen before send a Pull request.

## Vscode

### Config

Some config in preference

```json
{
    "editor.renderWhitespace": "all",
    "files.insertFinalNewline": true,
    "eslint.autoFixOnSave": true,
    "files.trimFinalNewlines": true,
    "tslint.enable": true,
    "tslint.autoFixOnSave": true,
    "markdown-preview-enhanced.liveUpdate": true
}
```

### Launch config

Useful when want debug, launch: [launch.json](vscode/launch.json)

### Plugins

- Auto Close Tag `formulahendry.auto-close-tag`
- Auto Rename Tag `formulahendry.auto-rename-tag`
- Color Info `bierner.color-info`
- CSS Peek `pranaygp.vscode-css-peek`
- Debugger for Chrome `msjsdiag.debugger-for-chrome`
- Docker `PeterJausovec.vscode-docker`
- Editorconfig for Vscode `EditorConfig.editorconfig`
- ESLint `dbaeumer.vscode-eslint`
- IntelliSense for CSS class names in HTML `Zignd.html-css-class-completion`
- Path Intellisense `christian-kohler.path-intellisense`
- Sort lines `Tyriar.sort-lines`
- Stylelint `shinnn.stylelint`
- vscode-icons `robertohuertasm.vscode-icons`

## Note

> You could wipe to linux also ;)

## ToDO

- [ ] A bash script to install my stuff (why not)