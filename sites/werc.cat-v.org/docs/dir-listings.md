Autogenerated Directory Listings
================================

If a directory has no `index.md`, `index.html` or `index.txt` and has no other
*main handler* set up by a [werc app](/apps/), the default directory listing
handler is used.

The default directory handler simply displays the path to the directory, and a
list of links to all files and dirs located at this path.


Header and footer
-----------------

If a `_header.md` or `_footer.md` files are found in the directory, their
contents will be displayed in the corresponding sections before and after
the directory contents.


Tuning the item's order
------------------------

You can set the `dir_listing_ls_opts` config variable in the dir's corresponding _werc/config to change the way items will be ordered.

For example to list items in reverse chronological order simply add:

    dir_listing_ls_opts=( -t )

The options taken are [the standard Plan 9 ls(1) flags](http://man.cat-v.org/plan_9/1/ls).
