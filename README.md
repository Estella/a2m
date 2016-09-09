# a2m

Convert ansi art to mirc art.

![screenshot](https://github.com/tat3r/a2m/blob/master/screenshot.png?raw=true)

For reference screenshot is iTerm2 with Menlo font ssh'd to a linux
machine attached to a tmux session running irssi.

## Installation

run make and copy a2m wherever you want.

## Usage

run a2m -h for a list of options

## Troubleshooting

### IRC Client

IRCCloud doesn't work very well.  It's monospaced font is *Iconsolata*, served
up by Google Web Fonts, which doesn't draw the block characters correctly
(see below).

### Terminal

Don't use reverse video, just make foreground white on black background, but
not bright white, there should be two different whites, bright white and
grayish white, 16 unique colors in all, as shown below:

Color | Regular | Bold
------|---------|-----
Black   | #000000 (0, 0, 0)       | #555555 (85, 85, 85)
Red     | #aa0000 (170, 0, 0)     | #ff5555 (255, 85, 85)
Green   | #00aa00 (0, 170, 0)     | #55ff55 (85, 255, 85)
Yellow  | #aa5500 (170, 85, 0)    | #ffff55 (255, 255, 85)
Blue    | #0000aa (0, 0, 170)     | #5555ff (85, 85, 255)
Magenta | #aa00aa (170, 0, 170)   | #ff55ff (255, 85, 255)
Cyan    | #00aaaa (0, 170, 170 )  | #55ffff (85, 255, 255)
White   | #aaaaaa (170, 170, 170) | #ffffff (255, 255, 255)

### Font

Try *Andale Mono* or *Menlo* for Mac.  *Deja Vu Sans* for Linux.
Someone tell me what works good for Windows.

If the font you use is missing some of the block drawing unicode
characters its going to borrow them from another font, which
will probably having a different width than the original font.
