# To-Be-Productive

Getting you closer to reaching peak productivity levels.

![](https://tva1.sinaimg.cn/large/006tNbRwly1g9phshc0wpj31jk0pjju3.jpg)

> All the things are based on mac. So if you'r using windows, you'r welcome to send [pull request](https://github.com/azl397985856/To-Be-Productive/pulls?q=is%3Apr+is%3Aopen+sort%3Aupdated-desc) to me.

## Mac 装机指南

https://github.com/azl397985856/mac-setup

## 习惯

### 劳逸结合

我们大脑工作其实有两种模式，一种是“发散模式”，一种是“专注模式”。 两种模式适合做的事情不一样，经常休息，有助于我们在两种模式之间切换。

另外，根据“首因效应”和“近因效应”，这种经常休息的行为，实际上是有效利用了这两种效应。另外适当锻炼也可以有效改善记忆，一些研究甚至指出，坚持运动的人大脑中负责记忆的前额叶皮质区和侧头叶皮质区会比常人更大。

我的个人做法是在需要的时候“设定一个物理的番茄时钟 ⏰”。然后按照番茄工作法来强制自己不断休息，同时它也可以提醒我时间的流逝。 我们知道一天只有 1440 分钟，一个完整番茄的时间是 30 分钟，除去玩吃饭，睡觉，娱乐，我们按照 12 个小时来算，也就是 24 个番茄，因此番茄工作法从`更大的纬度告诉我时间的流逝`。

### 尽量看文字，避免看视频和听录音等

### 如果不能避免看视频和听录音， 请开启两倍速

### 在做不需要特别注意力的事情时，可以听录音和广播等

### 复习 & 练习

相信`practice makes perfect`

### 专注模式的时候，尽可能关闭一切通知

![](https://tva1.sinaimg.cn/large/006tNbRwly1g9phjo8iouj31140tctgz.jpg)

### 重要的事情不做 TODO List

### 八二法则

### 利用好清晨

### 保持好的精力

## 技巧

### 快捷键 - GUI

> 持续更新

One principle is making shortcuts consistent.

0. system shortcuts

- `ctrl + up` show all opened windows
- `ctrl + down` show all opened windows of actived app
- `cmd + m` minimize the active window
- `cmd + ,` open setting
- show/hide of all apps (Thor)
- swipe left or right with three fingers 
> you should configure desktops  first,  3 to 4 desktops is fine.For example one for chat, one for coding, one for browser.

![](https://tva1.sinaimg.cn/large/006tNbRwly1g9rgkxe6b9j30a00edt99.jpg)

1. editor(vscode)

- `ctrl + -` back to previous position

- `ctrl + tab` switch between tabs

- `ctrl + [1-9]` go to specified tab

- `cmd + b` show/hide sidebar

- `cmd + shift + f` Search Text Through All Files At Once
- `cmd + shift + t` Re-open Last Closed Tab

- `cmd + Backtick` to open the Integrated Terminal

- `option + delete` delete previous word
- `cmd + delete` delete previous line

- `cmd + x` delete the whole line

- `cmd + /` comment the line

- `ctrl + a` move to beginning of line
- `ctrl + e` move to end of line

- `option + arrow up/arrow down` move line up/down

- `cmd + arrow up /arrow down` move to beginning/end of the file

2. terminal

- `cmd + t` open a new tab
- `cmd + [` move to previous tab（splited pane）
- `cmd + ]` move to next tab (splited pane)
- `cmd + shift + [` move to previous tab
- `cmd + shifr + ]` move to next tab
- `cmd + w` close current tab
- [others](https://github.com/azl397985856/learn-shell/projects/1#card-29852506)

3. browser(google chrome)

- `cmd + t`
- `cmd + shift + t`(Open Last Closed Tab)

- `cmd + n`
- `cmd + w` (Close the Active Right Away)

- `cmd + number` (jump through tabs by tab index)

- `cmd + shift + n` (Go Incognito Mode)

- `cmd + ->`
- `cmd + <-`

- `cmd + l` focus the 'location bar'

- `cmd + option + l` open the downloads page

- `cmd + shift + delete` clear browser cache

4. google

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g9dy1kml11j30u02pkdsk.jpg)

5. github

![](https://tva1.sinaimg.cn/large/006tNbRwly1g9pkqsp2hbj30u010q4ap.jpg)

6. Spectacle

![](https://tva1.sinaimg.cn/large/006tNbRwly1g9plxgv0kkj30y80tq47b.jpg)

### alias - CLI

eg:

```bash
# common
alias cls='clear'
alias free='top -l 1 | head -n 10 | grep PhysMem'
alias nis='cnpm i --save'
alias myip='curl http://ipecho.net/plain'
alias proxy='export all_proxy=socks5://127.0.0.1:1086'
alias unproxy='unset all_proxy'
alias su="sudo"
alias bi="brew install"
alias bci="brew cask install"
alias tree="ls -R | grep ":$" | sed -e 's/:$//' -e 's/[^-][^\/]*\//--/g' -e 's/^/   /' -e 's/-/|/'"
...
```

#### git

```bash

glg	= git log --stat
gcam = git commit -a -m
gcb	= git checkout -b
gco	= git checkout
gst	= git status
gss	= git status -s
gl = git pull
gp =	git push
ggp	= git push origin $(current_branch)
gm	= git merge
gmom	= git merge origin/master
gb =	git branch
gba	= git branch -a
gbd	= git branch -d

```

for more, [check it out](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git/)

### 代码片段 - Editor

eg:

> → means 'Tab'

```
# log
clg→	console log console.log(object)
clo→	console log object with name console.log('object :', object);
ctr→	console trace console.trace(object)
cwa→	console warn console.warn
cin→	console info console.info
clt→	console table console.table
cti→	console time console.time
cte→	console timeEnd console.timeEnd
...
# import
imp→	imports entire module import fs from 'fs';
imn→	imports entire module without module name import 'animate.css'
imd→	imports only a portion of the module using destructing import {rename} from 'fs';
ime→	imports everything as alias from the module import * as localAlias from 'fs';
ima→	imports only a portion of the module as alias import { rename as localRename } from 'fs';
...
# ...

```

### 软件使用[TODO]
