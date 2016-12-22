# Emoji Commit Messages

My personal variant of the ever-popular emoji commit message practice.

## Motivation

Emoji help make it more clear what a given commit is trying to accomplish,
make your commit history easier to search though, and encourage you
to keep each of your changes contained to a single type of action.
This makes it easier to reason about the history of your code.

For example, instead of having one massive commit that adds a feature,
refactors an old related feature, fixes a typo, and fixes a bug,
you could split that change into four commits that each accomplish
one specific action. Not only does this make things cleaner and clearer,
but it also helps when using tools like `git bisect` to track down bugs.

## The List

| Emoji | When to use it |
|:-----:|:-------------- |
| 🎉 | initial commit |
| 🎨 | when improving UI |
| 📦 | when refactoring or improving code |
| 🐎 | when improving performance |
| ☁ | when tweaking an API |
| 📝 | when writing docs (e.g. README, code comments) |
| 🐛 | when fixing a bug |
| 💥 | when fixing a crash |
| 🚱 | when plugging memory leaks |
| 🔥 | when removing code or files |
| ✅ | when adding tests |
| 💚 | when fixing the CI build |
| ⬆ | when upgrading dependencies |
| ⬇ | when downgrading dependencies |
| 👕 | when removing linter warnings |
| ✨ | when adding a new user-facing feature |
| 🎌 | when adding an A/B test or feature flag |
| ♿ | when improving accessibility |
| ⚡ | when making a backwards-incompatible change |
| 🎀 | when making a custom change at someone's behest |
| 🔧 | when updating configs |
| 🔒 | when dealing with security |
| 🚧 | when the change is a "work in progress" (do not merge) |
| 📡 | when adding instrumentation or metrics |
| 🔊 | when adding logging |
| 🔇 | when removing logging |
| 🚀 | when doing stuff related to dev tools |
| 💎 | when bumping version for a new release |

## How to decide which emoji to use

In most cases, your change will fit into a pretty obvious emoji category. If it doesn't, you should think hard about whether you're really making a clean change. Often you can break it into two or more commits that each accomplish their own specific type of action. If that means you only change one tiny line or fix a simple typo in a commit, so be it! It should be a no-brainer that any given commit does exactly what it says it does and **only** what is says it does. No side-effects.

In general, you should use exactly one emoji per commit message. In rare cases, you should use a second emoji (e.g. when using something like :zap: to signify that whatever you just did -- :bug:, :fire:, etc. -- was a breaking change).

## How to type emoji on your computer

You could always type the raw emoji code in plain text,
but it's often easier to search through the actual icons.

On Mac OSX, you can simply use the hotkey `Ctrl + Cmd + Space`.

On Ubuntu 14+, you can use the Emojione Picker app:

```console
sudo add-apt-repository ppa:ys/emojione-picker && sudo apt-get update
sudo apt-get install emojione-picker
```

On Windows 8+, you can use the on-screen keyboard in the system tray (there must be a better way...)

And if all else fails, you can search for them at <http://emojipedia.org/>
and simply copy/paste.

## Credits

Developed along with my wonderful co-workers at [Cribspot](https://www.cribspot.com/).

Inspired in part by style guides from [slashsBin](https://github.com/slashsBin/styleguide-git-commit-message#suggested-emojis) and [atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages).
