# Fedora 36 Setup for Manim

Steps required to install Manim via `pip3`

## Guides Used

1. [Manim Docs](https://manim.readthedocs.io/en/latest/installation/linux.html)
   - This is for Ubuntu and I may come back to double check 
2. [3b1b/manim Wiki](https://github.com/3b1b/manim/wiki/Install-on-Linux-Fedora-29)
   - An old guide for Fedora 29!
3. ...

## Steps

1. `dnf` packages

    ```sh
    $ sudo dnf install python-devel
    # Need python dev tools for some pip packages

    $ sudo dnf install sox sox-devel cairo cairo-devel
    # As Docs but different names for Fedora - <1MB
    #   cairo was already installed for me

    $ sudo dnf install ffmpeg-free
    # Free version of ffmpeg - 27MB

    $ sudo dnf install texlive
    # Latex the full bhoona - 424MB

    $ sudo dnf libglvnd-glx libglvnd-opengl libglvnd-devel
    # NOTE: Not sure about this. mesa{-devel} already present or depedency

    ```

2. `pip` packages

    ```sh
    $ pip install wheel
    # WARNING
    #   The script wheel is installed in '/home/shahzad/.local/bin' which is not on PATH.

    $ pip install manimgl
    #
    # Does quite a bit of stuff

    ```

3. 
