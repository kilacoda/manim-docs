Running Manim projects
======================

.. note::
     I'd suggest you create a separate folder for your animations
     as a lot of files are created by manim (e.g. LaTeX files)
     which can become difficult to manage at times. It's also good
     practice to create a new folder for every project you have. The rest is upto
     you.

Create a new file called ``file1.py``, and write/paste the following code::

    from manimlib.imports import *

    class HelloWorld(Scene):
        def construct(self):
            hello_world = TextMobject("Hello World")

            self.play(Write(hello_world))
            self.wait()

No need to worry about what's going on here at the moment, as
everything will be explained in due time.

Save the file now and return to your terminal. If you've
installed the manim from ``pip``, you can use the following
statement::

[py|python|python3 -m] manim path\to\file1.py HelloWorld -pl

If you've downloaded manim from GitHub, you'll have to enter
the directory where manim is stored, and then run the same.

The ``-pl`` in the above statement tells manim to ``p`` review/
play the rendered video in your default media player, in ``l`` ow
quality (480p15).

The output is this.

.. raw:: html

    <iframe width="560" height="315" src="https://www.youtube.com/embed/Ooh8cOem4ow" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Congratulations! You've rendered your first video.

.. note::

    Shameless plug, but I've written a GUI renderer for manim
    which you can find `here <https://github.com/raghavg123/Manim-Renderer>`_.
    I've found it useful in imporving my workflow and I hope it
    does for you. Check it out!


You can try running the premade scenes in ``example_scenes.py`` 
as well, using the same steps.

