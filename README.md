ELL-i Eagle Libraries
=====================

We at the ELL-i open source co-operative have decided to adopt the
SparkFun Electronics' approach to Eagle models, with the
addition of providing EagleUp models for all the components that we
have in our libraries.  In the cases where there is already an
existing SparkFun component that we use, we only provide the
corresponding EagleUp models in this repository.

For the SparkFun Eagle libraries, see
https://github.com/sparkfun/SparkFun-Eagle-Libraries

For more information about the ELL-i co-operative, see
http://www.ell-i.org

How to install the libraries
----------------------------

These instructions assume that you have
 [Eagle](http://www.cadsoftusa.com/eagle-pcb-design-software),
 [EagleUp](https://eagleup.wordpress.com)
 and [SketchUp](http://www.sketchup.com) installed.

First, use [git](http://git-scm.com) to clone both the SparkFun and
ELL-i Eagle libraries from [GitHub](https://github.com).
If you use command-line git, give the following commands at a suitable
directory:

```
  git clone https://github.com/sparkfun/SparkFun-Eagle-Libraries.git
  git clone https://github.com/Ell-i/ELL-i-Eagle-Libraries.git
```

Then add the libraries into the Eagle library path:

1. Lauch Eagle
2. Make sure you have the ``Control Panel`` window selected.
3. Select Options->Directories... from the pull-down menues.
4. Add the newly cloned libraries to the beginning of the Libraries
   path.  For example, the new Libraries could look like this:
```
  $HOME/ELL-i/SparkFun-Eagle-Libraries:$HOME/ELL-i/ELL-i-Eagle-Libraries:$EAGLEDIR/lbr:
```
   If you are a beginner, also remove "$EAGLEDIR/lbr".  That directory
   contains the Eagle default libraries, which you should not use when
   designing ELL-i boards.  (That is, unless you know what you do.)
5. Click "Ok" to close the dialog box.
6. Quit and restart Eagle to make it to pick the new default libraries.
7. Create a new schematic to set up the used libraries: Select
   File->New->Schematic
8. Open the Libraries dialog box:  Libraries->Use...

If you have installed the SparkFun and ELL-i libraries correctly, you
should now see the SparkFun and ELL-i libraries.  Depending on whether
you removed the Eagle standard libraries (as we recommend for
beginners), you may also see (or not) the Eagle standard libraries
there.

After this, when you create a new schematic, you should see (only) the
SparkFun and ELL-i component libraries.

Using and configuring EagleUp
-----------------------------

The instructions for setting up EagleUp and using SketchUp to open 3D
models are TBD.

A note about 3D file formats
----------------------------

Please note that only hobbyists (like us) use SketchUp files.
SketchUp was originally developed for architectural sketching, and it
is still used for architecture, civil engineering, and other similar
applications.  It is not very suitable for mechanical engineering.
However, we find its user interface very easy to learn compared to
most other 3D modelling packages.  That together with the EagleUp tool
and the relative plentitude of existing EagleUp-compatible 3D models
has made it our choice.

For a relatively informed discussion about the 3D models used by the
professionals, mainly IGES and STEP, you can have a look at the
discussion that ensued from
[SparkFun's decision to start using SketchUp](https://www.sparkfun.com/news/1115).
Especially the comments about
[NURBS/BREPs](https://www.sparkfun.com/news/1115#comment-51706161757b7fe258000000)
and
[3d content central](https://www.sparkfun.com/news/1115#comment-516ed006757b7f796f000000)
appear to be particularly informed.
