= slideshow

Slide Show (S9) - A Free Web Alternative to PowerPoint and KeyNote in Ruby

* http://slideshow.rubyforge.org

== DESCRIPTION:

The Slide Show (S9) Ruby gem lets you create slide shows and author slides in plain text
using a wiki-style markup language that's easy-to-write and easy-to-read.
The Slide Show (S9) project also collects and welcomes themes and ships
"out-of-the-gem" with built-in support for "loss-free" gradient vector graphics themes.

== SYNOPSIS:

  Usage: slideshow [options] name
    -o, --output PATH                Output Path
    -g, --generate                   Generate Slide Show Templates
    -t, --template MANIFEST          Template Manifest
        --s5                         S5-Compatible Slide Show (same as -t s5.txt)
        --fullerscreen               FullerScreen-Compatible Slide Show (same as -t fullerscreen.txt)
    -f, --fetch URI                  Fetch Templates
    -c, --config PATH                Configuration Path (default is ~/.slideshow)
    -l, --list                       List Installed Templates
    -v, --verbose                    Show debug trace
    -h, --help                       Show this message

Examples:

  slideshow microformats
  slideshow microformats.textile
  slideshow -o slides microformats       # Output slideshow to slides folder
  slideshow --s5 microformats            # Use S5-compatible slide show templates
  slideshow --fullerscreen microformats  # Use FullerScreen-compatible slide show templates

More examles:

  slideshow -g                           # Generate slide show templates
  slideshow -g --s5                      # Generate S5 compatible slide show templates
  slideshow -g --fullerscreen            # Generate FullerScreen compatible slide show templates

  slideshow -l                           # List installed slide show templates
  slideshow -f s5blank                   # Fetch (install) S5 blank starter template from internet
  slideshow -t s5blank.txt microformats  # Use your own slide show templates (e.g. s5blank.txt)


== REQUIREMENTS:

* RedCloth (Textile Markup)
* BlueCloth (Markdown Markup)

* RDiscount (Markdown Markup) [Optional]
* Coderay (Syntax Highlighting) [Optional]
* Ultraviolet (Syntax Highlighting) [Optional]

== INSTALL:

Just install the gem:

  $ sudo gem install slideshow

== LICENSE:

The slide show scripts and templates are dedicated to the public domain. Use it as you please with no restrictions whatsoever.