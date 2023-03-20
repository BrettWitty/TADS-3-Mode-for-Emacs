❗ **This repo has been taken up by https://github.com/alexispurslane/tads3-mode and this version will be archived** ❗

-----

This TADS 3 emacs mode was modified by Brett Witty <brettwitty@brettwitty.net> from Stephen Granade's tads2-mode.el. The  only real changes was a modified regexp to deal with object definitions so that tads-next-object and tads-prev-object work nicer. It also helps with indenting TADS 3-style object code.

Problems:
- MANY!
- Multiline C-style comments like:
```
   /* This
      is
      a comment */
```
still have font-lock problems. Multiline font-locking is known to
be difficult.
- In such comments, an apostrophe (') will try to match with
something nonsense later on.
- You cannot move to sub-objects via tads-next-object.

It is VERY strongly recommended that swapq-fill.el is used in
conjunction with this mode, to assist in single quote filling.
