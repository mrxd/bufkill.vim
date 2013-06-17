Up to date mirror of John Orr's bufkill - http://www.vim.org/scripts/script.php?script_id=1147

Basic Usage:
When you want to unload/delete/wipe a buffer, use:
  :bun/:bd/:bw to close the window as well (vim command), or
  :BUN/:BD/:BW to leave the window(s) intact (this script).
To move backwards and forwards through the chronological
list of buffers accessed, use :BB and :BF, respectively.
Mappings are also defined.

Detailed Description:
This is a script to
a) unload, delete or wipe a buffer without closing the window (or windows)
    it was displayed in
b) in its place, display the buffer most recently used in each window
    it was displayed in.  This selection is taken from the full list of
    buffers ever displayed in each respective window (since vim was started)
c) allow one level of undo in case you kill a buffer then change your mind
d) allow various customizations via option variables

Since the script maintains a list of buffer access order for each window,
commands are also provided to move backwards and forwards between
the buffers in this order, similar to going backwards and forwards in a
web browser.

The inspiration for this script came from
a) my own frustration with vim's lack of this functionality
b) the description of the emacs kill-buffer command in vimtip #622
   (this script basically duplicates this command I believe,
   not sure about the undo functionality)
c) comments and many mails from Keith Roberts when the issue was
   raised in the vim@vim.org mailing list.
