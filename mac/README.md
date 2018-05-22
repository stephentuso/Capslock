# CapsLock (Mac)

 > *This fork allows for normal use of alt/command with navigation on Mac (navigate by word/line)*

* CapsLock Enhancement (mac) is based on Project [`Karabiner-Elements`](https://pqrs.org/osx/karabiner/)

* Current release of karabiner works on following macOS:

  * macOS High Sierra (10.13)
  * macOS Sierra (10.12)
  * macOS EI Capitan (10.11)

* For older OS X user, refers to [old](../mac-old) `karabiner` XML-Format configuration script.

  ​


## Install (mac)

1. Download [Karabiner-Elements](https://pqrs.org/osx/karabiner/) and Install

2. Copy URL to your browser to import configuration script.

```bash
karabiner://karabiner/assets/complex_modifications/import?url=https://raw.githubusercontent.com/stephentuso/Capslock/master/mac/caps_lock.json
```

3. Open Karabiner, Tab "ComplexModification", Button "Add Item", and enable entries you like.

4. Default conf file path is `$HOME/.config/karabiner/assets/complex_modifications`. Modify it if you like.


* Or you can just download and put json conf file in conf directory manually：

  `$HOME/.config/karabiner/assets/complex_modifications`


* See [Karabiner-Elements Sample Scripts](https://github.com/pqrs-org/KE-complex_modifications) for instructions:
  * Open `karabiner-elements`
  * Select tab `Complex Modification`
  * Click `Add item` at bottom
  * Enable function you like.

  ​


## Usage

![keyboard](keyboard.png)

### Basic

`✱` Hyper actually maps to `⌃⌥⇧⌘` (all right modifiers) , It works well with additional left modifiers. And compatible with most application. Hold CapsLock to enable `Hyper` funcationality while press it will emit an `Escape`.

| Origin    | Maps to    | Comment                    |
| --------- | ---------- | -------------------------- |
| `⇪` Press | `⎋` Escape | Single press to escape     |
| `⇪` Hold  | `✱`  Hyper | Enable Hyper Functionality |



### Navigation

* Hold  `✱` Hyper to enable navigators


| Origin | Maps to        | Comment                  |
| ------ | -------------- | ------------------------ |
| `H`    | `←` LeftArrow  | cursor left              |
| `J`    | `↓` DownArrow  | cursor down              |
| `K`    | `↑` UpArrow    | cursor up                |
| `L`    | `→` RightArrow | cursor right             |
| `U`    | `⇞` PageUp     | cursor page up           |
| `I`    | `↖` Home       | cursor to line(doc) head |
| `O`    | `↘`  End       | cursor to line(doc) end  |
| `P`    | `⇟` PageDn     | cursor page down         |



### Deletion

| Origin    | Maps to                            | Comment             |
| --------- | ---------------------------------- | ------------------- |
| `N`       | `⌥⌫`  Option + ForwardDelete       | Delete a word ahead |
| `M`       | `⌫` ForwardDelete                  | Delete a char ahead |
| `,`       | `⌦` Delete                         | Delete a char after |
| `.`       | `⌥⌦` Option + Delete               | Delete a word after |
| `⌘M`,`⌘N` | `⌘⌥⌫` Command+Option+ForwardDelete | Delete to line head |



### Window Control

| Origin           | Maps to                 | Comment                                  |
| ---------------- | ----------------------- | ---------------------------------------- |
| `⇥` Tab          | `⌘⇥` Command+Tab        | Switch Window                            |
| `⌘⇥` Command+Tab | `⌘⇧⇥` Command+Shift+Tab | Switch Window Reversely                  |
| `Q`              | `⌘Q`                    | Close Window                             |
| `W`              | `⌘W`                    | Close Tab                                |
| `E`              | Open Safari             | Open Web Browser                         |
| `⌘E`             | Open Finder             | Open File Browser                        |
| `A`              | `⌃⌥⇧⌘A`                 | Leaves to [Moom](https://manytricks.com/moom/), ※a window resize app |
| `⌘A`             | `⌃↑`  Ctrl+UpArrow      | OSX Expose All                           |
| `S`              | `⌃⇥`  Ctrl+Tab          | Switch Tab                               |
| `⌘S`             | `⌃⇧⇥` Ctrl+Shift+Tab    | Swtich Tab Reversely                     |
| `⌘D`             | `F11`                   | Show Desktop                             |



### Bash Control

* Common bash utils: EOF, SIGINT, SIGTSTP, VIM/Tmux Prefix

| Origin | Maps to     | Comment                                  |
| ------ | ----------- | ---------------------------------------- |
| `Z`    | `⌃Z` Ctrl+Z | SIGTSTP                                  |
| `X`    | `⌃R`        | IDE Run                                  |
| `C`    | `⌃C`        | SIGINT                                   |
| `V`    | `⌃V`        | Vim Prefix                               |
| `B`    | `⌃B`        | [Tmux](http://tmux.github.io) Default Prefix |
| `D`    | `⌃D`        | EOF                                      |



#### Applications

* Maybe you'd like overwrite these with your own favorite apps.

| Origin | Maps to                 | Comment                                  |
| ------ | ----------------------- | ---------------------------------------- |
| `R`    | Open iTerm2             | Great terminal for osx (`Run`)           |
| `⌘R`   | Open Preview            | Switch to opened picture, pdf, etc...    |
| `T`    | Open Visual Studio Code | Text Editor: Visual Studio Code          |
| `⌘T`   | Open Typora             | Text Editor: Typora , a great WYSIWYG md editor |
| `Y`    | Open Siri               |                                          |
| `F`    | Open Dash               | Find API Document                        |
| `⌘F`   | Open Dictionary         | Find words                               |
| `G`    | Open Intellij IDEA      | Open IDE                                 |
| `⌘G`   | Open Chrome             | Google Chrome                            |



### Functional

* Use F1,…F12 as standard functional keys, while hold hyper to turn them back.

| Origin            | Maps to              | Comment                          |
| ----------------- | -------------------- | -------------------------------- |
| `F1`              | `BrightnessDown`     |                                  |
| `F2`              | `BrightnessUp`       |                                  |
| `F3`              | `ExposeAll`          |                                  |
| `F4`              | `LaunchPad`          |                                  |
| `F5`              | `KeyboardLightDown`  |                                  |
| `F6`              | `KeyboardLightUp`    |                                  |
| `F7`              | `MusicPrev`          |                                  |
| `F8`              | `MusicPlay`          |                                  |
| `F9`              | `MusicNext`          |                                  |
| `F10`             | `Mute`               |                                  |
| `F11`             | `VolumeDown`         |                                  |
| `F12`             | `VolumeUp`           |                                  |
| `F13` PrintScreen | `MusicPrev`          |                                  |
| `F14` ScrollLock  | `MusicNext`          |                                  |
| `F15` Pause       | `Mute`               |                                  |
| `Insert`          | `⌥BrightnessUp`      | Fine grained brightness up       |
| `Delete`          | `⌥BrightnessDown`    | Fine grained brightness down     |
| `Home`            | `⌥KeyboardLightUp`   | Fine grained keyboard light up   |
| `End`             | `⌥KeyboardLightDown` | Fine grained keyboard light down |
| `PgUp`            | `⌥VolumeUp`          | Fine grained volume up           |
| `PgDn`            | `⌥VolumeDown`        | Fine grained volume down         |



### Shifter

* A more convient shift for most case

| Origin             | Maps to | Comment                  |
| ------------------ | ------- | ------------------------ |
| `1`                | `!`     | Exclamation              |
| `2`                | `@`     | At                       |
| `3`                | `#`     | Sharp                    |
| `4`                | `$`     | Dollar                   |
| `5`                | `%`     | Percent                  |
| `6`                | `^`     | Caret                    |
| `7`                | `&`     | Ampersand                |
| `8`                | `*`     | Star                     |
| `9`                | `(`     | Left Round Bracket       |
| `0`                | `)`     | Right Round Bracket      |
| `-` Minus          | `_`     | Hyphen                   |
| `=` Equal          | `+`     | Plus                     |
| `[` Left Bracket   | `(`     | Left Round Bracket `⇧9`  |
| `]`  Right Bracket | `)`     | Right Round Bracket `⇧0` |
| `\` Back Slash     | `|`     | Bar                      |
| `;` Semicolon      | `:`     | Colon                    |
| `'` Single Quote   | `"`     | DoubleQuote              |



### Misc

| Origin                 | Maps to             | Comment                                  |
| ---------------------- | ------------------- | ---------------------------------------- |
| `⎋` Escape             | `⇪`  CapsLock       | Bug: Difficult to turn capslock off after emit |
| `~` BackQuote          | `⌃⇧⌘4`              | macOS Area Screenshot to Clipboard       |
| `⌘~` Command+BackQuote | `⌃⇧4`               | macOS Area Screenshot to Desktop File    |
| `⌫` Backspace          | `⌘⌫`                | macOS Delete File                        |
| `↩`  Return            | `=`                 | Return to Equal Sign                     |
| `/` Slash              | `⌘/` Command+Slash  | Comment/Uncomment in many IDE            |
| `␢` Spacebar           | `⌃␢`  Ctrl+Spacebar | Switch Input Source                      |

