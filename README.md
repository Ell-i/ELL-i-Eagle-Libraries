ELL-i-Eagle-Libraries
=====================

We at the ELL-i open source co-operative have decided to adopt the
SpartFun Electronics' Eagle approach to Eagle models, with the
addition of providing EagleUp models for all the components that we
have in our libraries.  In the cases where there is already an
existing SparkFun component that we use, we only provide the
corresponding EagleUp models in this repository.

For the SparkFun Eagle libraries, see
https://github.com/sparkfun/SparkFun-Eagle-Libraries

For more information about the ELL-i co-operative, see
http://www.ell-i.org

How to install
--------------

These instructions assume that you have Eagle and SketchUp installed.

First, use git to clone both the SparkFun and ELL-i Eagle libraries.
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
6. Create a new schematic to set up the used libraries: Select
   File->New->Schematic
7. Open the Libraries dialog box:  Libraries->Use...
8. Navigate to the SparkFun libraries folder
9. Select all SparkFun-*.lbr files
10. Click Open.
11. Repeat the previous steps for the ELL-i libraries.

After this, when you create a new schematic, you should see (only) the
SparkFun and ELL-i components.

The instructions for EagleUp and SketchUp usage are TBD.
