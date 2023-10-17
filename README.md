# Introduction

This is a tool I first wrote for use with `mutt`, back in the late 1990s.
What follows is the original description.

# Original description


This filter is designed for use with mutt's auto_view facility. The idea
behind the script is that it will attempt to guess the true content of an
octet-stream MIME attatchment and format for easy text-oriented viewing.

To use `mutt.octet.filter` I have the following entry in my
`~/.mutt/mailcap` (my local mutt-only mailcap file):

```
application/octet-stream; mutt.octet.filter %s; copiousoutput
```

All that is then needed is to add a line like:

```
auto_view application/octet-stream
```

to your `~/.muttrc` (use your filename of choice) file and everything should
work just fine. The script isn't perfect and I'm sure there are lots of
things that could be added to it. Think of it as a "it works for me" script
and hack away at it to make it do exactly what you want it to do.

[//]: # (README.md ends here)
