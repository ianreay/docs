.. _vim:
Vim
=================================================

Quick reference
--------------------------------------------------------------------------------

:ref:`Useful keyboard shortcuts <vim-shortcuts>`

Books
-------------------------------------------------

`Practical VIM <http://pragprog.com/book/dnvim/practical-vim>`_ is a very
effective book. Lots of examples and well written.

Tutorials
--------------------------------------------------------------------------------

`Easier buffer switching <http://vim.wikia.com/wiki/Easier_buffer_switching>`_
`Fix indentation <http://vim.wikia.com/wiki/Fix_indentation>`_
`VIM loading sequence and vundle <https://github.com/gmarik/vundle/issues/163>`_

Tips for learning VIM
-------------------------------------------------------------------------------

* Understand it will take time. It may take a month or two before you really get comfortable with it.
* Start with the basics.
** Copy/Paste/Delete
** Navigation
* Every day/week add a new command.
* Use REAL examples. You will learn the fastest about what works best for you by doing real work rather than just working through examples over and over again.
* Try to minimize plugins. Stock VIM can do a great deal and is transferable. Good plugins can be very powerful, but often do not transfer between work environments.

Useful aids
-------------------------------------------------------------------------------

`Text anywhere <http://www.listary.com/text-editor-anywhere>`_

* Allows you to invoke gvim from text areas such as those in a browser. Useful for using vim in web apps or wikis that otherwise would not support editing with vim.

Plugins
-------------------------------------------------

`Vundle <https://github.com/gmarik/vundle>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The `Vundle <https://github.com/gmarik/vundle>`_ plugin is pretty much
mandatory if you are doing software development with vim. While you should
strive to minimize the number of plugins you depend upon, some plugins are well
worth it, and Vundle makes loading them dead easy.

The site has a good tutorial on how to get going with it. Works well for windows.

`UltiSnips <https://github.com/SirVer/ultisnips>`_ 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
UltiSnips is a fantastic plugin. It implements textmate like snippits. You will love how much time it can save you.

Frequently people install a plugin. That plugin has some great quick completion helpers to remove the need for a great deal of typing. This is great.

Then people need to do another file format. Maybe another programming language. So they get another plugin for that language. It has a completely different set of quick completion helpers. Not so great, but still worth it.

Then people get 4 or 5 more file formats or lanaguages in play. Soon you are in plugin and quick completion hell with all of the different keystrokes one must learn to do the basics. This really does not scale well.

Enter UltiSnips. It provides a very simple way of making a platform agnostic way of entering repetitive text. Very simple to use. I strongly advise using something like it for your day to day stuff and investigate language plugins for things beyond quick completion.

Some very useful screencasts have been provided in https://github.com/SirVer/ultisnips. I strongly advise checking them out if you want a quick summary of what this plugin is capable of.   

`SessionMan <https://github.com/vim-scripts/sessionman.vim>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
SessionMan allows you to save and then later reload your editing sessions.

Really, really useful when you need to jump between different work items. For example, you can have:

* One session for editing your vim configuration with important files open and ready.
* One session for editing your current non-customer work.
* One session for each active customer project. 
* One session for editing your personal docs and todo lists.

This can really save a great deal of time over the long run especially if you switch tasks fairly frequently.

Important commands:

* SessionSaveAs <name>
* SessionSave
* SessionList

Quick tutorial:

* Open vim. Open some windows, tabs, and set some current working directories.
* Save your session. :SessionSaveAs mysession
* Close vim
* Open vim. Get a session list by typing :SessionList
* Select the mysession session and open it
* All your original windows, tabs, and environment settings should be restored

`Vim-Commentary <https://github.com/tpope/vim-commentary>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Vim-Commentary <https://github.com/tpope/vim-commentary>`_ is a really nice
plugin when you are editing code or latex files. It provides a very slick way
of commenting and uncommenting large chunks of code.

Also very useful when you are putting comments in your code. Just write
language as you normally would and the comment the paragraph.

:help commentary.txt

gcap = comment out a paragraph of code (normally a function)
gc<space> = comment out a line
gc<motion> = comment out a motion of stuff

`Python-mode <https://github.com/klen/python-mode>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
`Python-mode <https://github.com/klen/python-mode>`_ is a nearly mandatory
plugin if you are doing work with python in vim. Its main strengths are:

* `PEP8 <http://www.python.org/dev/peps/pep-0008/>`_ style enforcement
* effective python auto indenting
* pylint code checking
 
Its well worth the small amount of time required to set it up.

`Nerd tree <https://github.com/scrooloose/nerdtree>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
:help NERD_tree.txt

NERDTree is a useful file system explorer. Its greatest value comes when you are learning a new code base since it allows you to quickly gain a grasp on the directory structure of a code set.

I personally find I don't use it too much once I know the code structure, but many people swear by it.

`Easy motion <https://github.com/Lokaltog/vim-easymotion>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
:help easymotion.txt

* \\b - backward start of word
* \\w - forward start of word
* \\e - forward end of word
* \\gE - backward end of word

Easy motion can be convenient for navigating and doing spot edits in large documents. In practice though, I find I only sometimes use it since VIMs native motions are generally very powerful.

`C.VIM <https://github.com/vim-scripts/c.vim>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
:help csupport.txt

C.VIM can be very powerful if C and C++ are your primary languages. It has many templates that assist with quick editing and also contains helpers for compiling code if you use Makefile's to compile your code.

I personally don't use it much though since I find UltiSnips to be generally more powerful and flexible and I tend not to use Makefile based software projects.

`XMLEdit <https://github.com/sukima/xmledit/>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

XMLEdit has some very nice helpers for editing xml docs. That said, UltiSnips is also capable of doing many of the helpers that XMLEdit can do and has the potential to scale to complex edits much easier in common xml files you use.

I would generally recommend seeing how far UltiSnips will get you before using XMLEdit so you can keep the number of commands you need to digest minimized.

`Latex-VIM <http://vim-latex.sourceforge.net/>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

`Latex-VIM tutorial <http://vim-latex.sourceforge.net/documentation/latex-suite-quickstart/index.html>`_

Latex-VIM is like XMLEdit. A very powerful standalone plugin, but one I generally do not use in favour of UltiSnips. Its nice to have one set of consistent commands for re-usable text snippts.

That said, if you are doing lots of latex, you may appreciate Latex-VIMs integrated document make and viewers.


