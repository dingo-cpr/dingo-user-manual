Dingo User Manual
==================

This repository contains the LaTeX source code for building the end user product
documentation for [Dingo](http://www.clearpathrobotics.com/dingo/). If you are
an end user, please download the official and released version of the manual from
the [Clearpath Robotics Resources Page](http://www.clearpathrobotics.com/dingo-user-manual/).


Build
-----


To build Dingo's user manual:

    git clone --recurse-submodules https://github.com/dingo-cpr/dingo-user-manual.git
    cd dingo-user-manual
    xelatex dingo.tex

The output is written to `dingo.pdf`. The `xelatex` command must be invoked twice
to generate the complete manual including table of contents and correct watermarks.


Setting it up
-------------

The manual may be built on any platform supported by TeXWorks or TeXLive.

On a **Mac**, download and install [MacTex Basic](http://mirror.ctan.org/systems/mac/mactex/mactex-basic.pkg).

On **Ubuntu**, run:

    sudo apt-get install texlive-xetex

Install some additional texlive packages:

    sudo tlmgr install everypage background titlesec microtype upquote \
                       enumitem tcolorbox environ trimspaces siunitx

On **Fedora/RHEL/CentOS**, run:
sudo yum install texlive-xetex texlive-everypage texlive-background texlive-titlesec texlive-microtype texlive-upquote texlive-enumitem texlive-tcolorbox texlive-environ texlive-trimspaces texlive-siunitx

On **Windows**:
- Install TeXworks.
- Install Source Tree, or your preferred Windows Git client.
- Install DINPro, Consolas typefaces.
- Use Sourcetree to clone this repo locally, then open `dingo.tex` in TeXworks.
- In Texworks, in the drop down menu beside the green arrow, switch to XeLaTeX + MakeIndex + BibTex
- Click the green start arrow


Typefaces
---------
To build the official manual, the following fonts will need to be installed:

- [DINPro](https://www.fontshop.com/families/ff-din/buy)
- [Consolas](http://www.fontpalace.com/font-download/Consolas/)


License
-------

Redistribution and use in source and binary forms, with or without modification, is
not permitted without the express permission of Clearpath Robotics.
