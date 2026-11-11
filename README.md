# typeclip

Types your clipboard out as keystrokes after a few seconds. For pages with a broken paste, like teams.cloud.microsoft.

## Install

Needs bash, xclip, xdotool and dmenu on X11. Notifications go through `notify-send` when it's there.

```sh
cp typeclip ~/.local/bin/
```

## Usage

Copy the text, run `typeclip` from dmenu, then click into the field. It types after 3 seconds.

```sh
typeclip      # wait 3 seconds
typeclip 5    # wait 5 seconds
```

Set `TYPECLIP_DELAY` to change the default. Newlines are typed as Return, so a multi-line text lands the way it was copied, which can submit a chat message early. In Teams, use Shift+Enter yourself if that matters.

## Notes

Typing is about 80 characters a second, so a long text takes a moment. Don't touch the keyboard until it's done.
