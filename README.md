# Emoji commit messages

My variant of the ever-popular emoji commit messages.

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

| Text | Image | Shortcode | When to use it |
|:----:|:-----:|:--------- |:-------------- |
| `🎉` | :tada: | `:tada:` | initial commit |
| `✨` | :sparkles: | `:sparkles:` | when adding a new user-facing feature |
| `🎨` | :art: | `:art:` | when improving UI |
| `📦` | :package: | `:package:` | when refactoring or improving code |
| `🐎` | :racehorse: | `:racehorse:` | when improving performance |
| `🔒` | :lock: | `:lock:` | when improving security |
| `🔧` | :wrench: | `:wrench:` | when updating configs |
| `♿` | :wheelchair: | `:wheelchair:` | when improving accessibility |
| `🚀` | :rocket: | `:rocket:` | when improving dev tools |
| `📝` | :pencil: | `:pencil:` | when writing docs (e.g. README, code comments) |
| `💎` | :gem: | `:gem:` | when cutting a new release / version bump |
| `🐛` | :bug: | `:bug:` | when fixing a bug |
| `💥` | :boom: | `:boom:` | when fixing a crash |
| `🚱` | :non-potable_water: | `:non-potable_water:` | when fixing a memory leak |
| `🔥` | :fire: | `:fire:` | when removing code or files |
| `✅` | :white_check_mark: | `:white_check_mark:` | when adding new tests |
| `💚` | :green_heart: | `:green_heart:` | when fixing the CI build |
| `👕` | :shirt: | `:shirt:` | when fixing linter warnings |
| `📡` | :satellite: | `:satellite:` | when adding instrumentation or metrics |
| `🔊` | :loud_sound: | `:loud_sound:` | when adding logging |
| `🔇` | :mute: | `:mute:` | when removing logging |
| `⬆` | :arrow_up: | `:arrow_up:` | when upgrading dependencies |
| `⬇` | :arrow_down: | `:arrow_down:` | when downgrading dependencies |
| `🎌` | :crossed_flags: | `:crossed_flags:` | when adding an A/B test or feature flag* |
| `⚡` | :zap: | `:zap:` | when making a backwards-incompatible change* |
| `🚧` | :construction: | `:construction:` | when the change is a work in progress (do not merge)* |

\* Asterisk means these emoji are often combined with another, primary emoji.

## How to decide which emoji to use

In most cases, your change will fit into a pretty obvious emoji category. If it doesn't, you should think hard about whether or not you're making a clean change.

Often you can break up changes into two or more commits that each accomplish their own specific type of action. If that means you only change one tiny line or fix a simple typo in a commit, so be it! It should be a no-brainer that any given commit does exactly what it says it does -- and **only** what is says it does. No side-effects.

In general, you should use exactly one emoji per commit message. In rare cases, you should use a second emoji (e.g. when using something like :zap: to signify that whatever you just did -- :bug:, :fire:, etc. -- was a breaking change).

Emoji will also depend on your client/user. A back-end API might use :sparkles: when adding new API endpoints, and the front-end app might use :sparkles: when using those endpoints to display new content.

## How to type emoji on your computer

I find it faster to type the raw emoji shortcode with colons (GitHub and GitLab both recognize this), but sometimes it's easier to search through the actual icons, especially as you're starting out.

- On Mac OSX, you can open the built-in emoji picker with the hotkey `Ctrl + Cmd + Space`

- On Ubuntu 14+, you can use the Emojione Picker app:

    ```console
    sudo add-apt-repository ppa:ys/emojione-picker && sudo apt update
    sudo apt install emojione-picker
    ```

- On Windows 8+, you can use the on-screen keyboard in the system tray (there must be a better way...)

If all else fails, you can search for an emoji at <http://emojipedia.org/>
and simply copy/paste.

## Real examples

The following is a brief list of open-source projects currently using these emoji:

- https://github.com/cooperka/emoji-commit-messages (of course)

- https://github.com/cooperka/react-native-immutable-list-view

- https://github.com/cooperka/react-native-snackbar

- https://github.com/cooperka/bash-git-utils

- https://github.com/cribspot/emoji-utils

## Credits

Developed along with my co-workers at [Cribspot](https://www.cribspot.com/). Inspired in part by style guides from [slashsBin](https://github.com/slashsBin/styleguide-git-commit-message#suggested-emojis) and [atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages).
