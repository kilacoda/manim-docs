Scenes
======

Scenes are what can be considered the `canvases` for your animations. All scenes
are derived from the ``Scene`` class, which in itself is derived from the 
``Container`` class.

Here's a quick rundown of how manim processes videos:

1. Get classes deriving from ``Scene``.
2. Execute the ``digest_config`` function to associate parameters for the scene.
3. Execute the scene's ``construct`` function and render whatever's in it.

Let's take a look at the pre-defined scenes in manim. (Yes you can create your
own as well!)

Scene
-----

.. autoclass:: manimlib.scene.scene.Scene
    :members:

Graph Scene
-----------

.. autoclass:: manimlib.scene.graph_scene.GraphScene
    :members:

3-D Scene
---------

.. autoclass:: manimlib.scene.three_d_scene.ThreeDScene
    :members:



