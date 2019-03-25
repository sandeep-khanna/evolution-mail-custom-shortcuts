# Custom Keyboard Shortcuts for Gnome Evolution Mail Client

If currently running, quit Evolution before making changes. Even after quitting the application, Eolution processes continue to run in the background. The following command-line may be used to list and kill the Evolution processes:

`user@linux:~$ ps aux | grep evolution | awk '{print $2}'`

Review and update the `accels` file to $HOME/.config/evolution/accels` and start Evolution again (Check more at [this post](https://www.systutorials.com/240792/evolution-save-data-configure-files-linux/)).

These commonly used keyboard shortcuts will be enabled/changed:

```
(gtk_accel_path "<Actions>/new-item/mail-message-new" "<Primary>n")
(gtk_accel_path "<Actions>/mail/mail-flag-for-followup" "asterisk")
(gtk_accel_path "<Actions>/mail/format-bulleted-list" "<Primary><Shift>8")
(gtk_accel_path "<Actions>/mail/mail-previous-thread" "p")
(gtk_accel_path "<Actions>/mail/format-numbered-list" "<Primary><Shift>7")
(gtk_accel_path "<Actions>/mail/mail-next" "j")
(gtk_accel_path "<Actions>/mail-convert-any/mail-convert-to-task" "<Shift>t")
(gtk_accel_path "<Actions>/mail/mail-threads-expand-all" "semicolon")
(gtk_accel_path "<Actions>/mail/mail-threads-collapse-all" "colon")
(gtk_accel_path "<Actions>/mail/mail-next-thread" "n")
(gtk_accel_path "<Actions>/mail/mail-previous" "k")
(gtk_accel_path "<Actions>/core-editor/style-list-number" "<Primary><Shift>7")
(gtk_accel_path "<Actions>/core-editor/style-list-bullet" "<Primary><Shift>8")
```