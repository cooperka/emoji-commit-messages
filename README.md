# Emoji commit messages

A fun paradigm to encourage cleaner commits.

## Motivation

Images (including emoji) help clarify what a given commit accomplishes,
make your commit history easier to scan though, and encourage you
to limit each of your changes to a single type of action.
This makes it easier to reason about the history of your code.

For example, instead of having one massive commit that adds a feature,
refactors an old related feature, fixes a typo, and fixes a bug,
you could split that change into four commits that each accomplish
one specific thing. Not only does this make things cleaner and clearer,
but it also helps when using tools like `git bisect` to track down bugs,
as well as when reverting individual changes.

## The list

| Text | Image | GFM shortcode | Windows 10 picker name | When to use it |
|:--:|:-----:|:--------- |:-------------- |:-------------- |
| `🎉` | :tada: | `:tada:` | `party popper` | initial commit |
| `✨` | :sparkles: | `:sparkles:` | `sparkles` | when adding a new user-facing feature |
| `🎨` | :art: | `:art:` | `artist palette` | when improving UI |
| `📦` | :package: | `:package:` | `package` | when refactoring or improving code |
| `🐎` | :racehorse: | `:racehorse:` | `horse` | when improving performance |
| `🔒` | :lock: | `:lock:` | `locked` | when improving security |
| `🔧` | :wrench: | `:wrench:` | `wrench` | when updating configs |
| `♿` | :wheelchair: | `:wheelchair:` | `wheelchair symbol` |  when improving accessibility |
| `🚀` | :rocket: | `:rocket:` | `rocket` | when improving dev tools |
| `📝` | :pencil: | `:pencil:` | `pencil` | when writing docs (e.g. README, code comments) |
| `💎` | :gem: | `:gem:` | `gem stone` | when cutting a new release / version bump |
| `🐛` | :bug: | `:bug:` | `bug` | when fixing a bug |
| `💥` | :boom: | `:boom:` | `collision` | when fixing a crash |
| `🚱` | :non-potable_water: | `:non-potable_water:` | `non-potable water` | when fixing a memory leak |
| `🔥` | :fire: | `:fire:` | `fire` | when removing code or files |
| `✅` | :white_check_mark: | `:white_check_mark:` | `check mark button` | when adding new tests |
| `💚` | :green_heart: | `:green_heart:` | `green heart` | when fixing the CI build |
| `👕` | :shirt: | `:shirt:` | `t-shirt` | when fixing linter warnings |
| `📡` | :satellite: | `:satellite:` | `satellite antenna` | when adding instrumentation or metrics |
| `🔊` | :loud_sound: | `:loud_sound:` | `speaker high volume` | when adding logging |
| `🔇` | :mute: | `:mute:` | `muted speaker` | when removing logging |
| `⬆` | :arrow_up: | `:arrow_up:` | `up arrow` | when upgrading dependencies |
| `⬇` | :arrow_down: | `:arrow_down:` | `down arrow` | when downgrading dependencies |
| `🎌` | :crossed_flags: | `:crossed_flags:` | `crossed flags` | when adding an A/B test or feature flag* |
| `⚡` | :zap: | `:zap:` | `high voltage` | when making a backwards-incompatible change* |
| `🚧` | :construction: | `:construction:` | `construction` | when the change is a work in progress (do not merge)* |

GFM shortcodes mainly work with **G**itHub **F**lavored **M**arkdown, but may work in other markdown renderers too.

\* Asterisk means these emoji are often combined with another, primary emoji.

## How to decide which emoji to use

In most cases, your change will fit into a pretty obvious emoji category. If it doesn't, you should think hard about whether or not you're making a clean change.

Often you can break up changes into two or more commits that each accomplish their own specific type of action. If that means you only change one tiny line or fix a simple typo in a commit, so be it! It should be a no-brainer that any given commit does exactly what it says it does — and **only** what is says it does. No side-effects.

In general, you should use exactly one emoji per commit message. In rare cases, you should use a second emoji (e.g. when using something like :zap: to signify that whatever you just did — :bug:, :fire:, etc. — was a breaking change).

Emoji will also depend on your client/user. A back-end API might use :sparkles: when adding new API endpoints, and the front-end app might use :sparkles: when using those endpoints to display new content.

## How to type emoji on your computer

I find it faster to type the raw emoji shortcode with colons (GitHub and GitLab both recognize this), but sometimes it's easier to search through the actual icons, especially as you're starting out.

- On Mac OS X, you can open the built-in emoji picker with the hotkey <kbd>Ctrl</kbd> + <kbd>Cmd</kbd> + <kbd>Space</kbd>.

- On Ubuntu 14+, you can use the Emojione Picker app:

    ```console
    sudo add-apt-repository ppa:ys/emojione-picker && sudo apt update
    sudo apt install emojione-picker
    ```

- On Windows 10 update 1709, pressing <kbd>Win</kbd>+<kbd>.</kbd> while having keyboard focus in a text field in any program will bring up the built-in emoji picker, similarly to Mac OS. The table above includes names which work specifically in this emoji picker, but the GFM shortcodes work too. Some of the Windows-specific ones can be easier to remember, though.

  On lower versions of Windows, starting with Windows 8, you can use the on-screen keyboard in the system tray. Alternatively, you can use [BabelMap] which is a Unicode character picker for even lower versions of Windows. It also might be more convenient than the Windows 8 on-screen keyboard.

If all else fails, you can search for an emoji at <http://emojipedia.org/> and simply copy/paste.

## Real examples

The following is a brief list of open-source projects currently using these emoji:

- https://github.com/cooperka/emoji-commit-messages (of course)

- https://github.com/cooperka/react-native-immutable-list-view

- https://github.com/cooperka/react-native-snackbar

- https://github.com/cooperka/bash-git-utils

- https://github.com/cribspot/emoji-utils

## Credits

Developed along with my co-workers at [Cribspot](https://www.cribspot.com/). Inspired in part by style guides from [slashsBin](https://github.com/slashsBin/styleguide-git-commit-message#suggested-emojis) and [atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages).

[BabelMap]: https://www.babelstone.co.uk/Software/BabelMap.html
