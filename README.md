# Custom Keyboard Shortcuts for Gnome Evolution Mail Client

If currently running, quit Evolution before making changes. Even after quitting the application, Eolution processes continue to run in the background. The following command-line may be used to list and kill the Evolution processes:

`user@linux:~$ kill $(ps aux | grep '[e]volution' | awk '{print $2}')`

Review and update the `accels` file to `$HOME/.config/evolution/accels` and start Evolution again.

The following articles provide more information:

- [Where Does Evolution Save Its Data and Configuration Files on Linux?](https://www.systutorials.com/240792/evolution-save-data-configure-files-linux/)

- [Custom keyboard shortcuts for Evolution in GNOME](https://major.io/2015/11/27/custom-keyboard-shortcuts-for-evolution-in-gnome/)

These commonly used keyboard shortcuts will be enabled/changed:

```
(gtk_accel_path "<Actions>/new-item/mail-message-new" "<Primary>n")
(gtk_accel_path "<Actions>/mail/mail-flag-for-followup" "asterisk")
(gtk_accel_path "<Actions>/mail-convert-any/mail-convert-to-task" "<Shift>t")
(gtk_accel_path "<Actions>/mail/mail-delete" "numbersign")

(gtk_accel_path "<Actions>/shell/search-quick" "slash")

(gtk_accel_path "<Actions>/mail/mail-threads-expand-all" "semicolon")
(gtk_accel_path "<Actions>/mail/mail-threads-collapse-all" "colon")

(gtk_accel_path "<Actions>/mail/mail-next" "j")
(gtk_accel_path "<Actions>/mail/mail-previous" "k")
(gtk_accel_path "<Actions>/mail/mail-next-thread" "n")
(gtk_accel_path "<Actions>/mail/mail-previous-thread" "p")

(gtk_accel_path "<Actions>/core-editor/style-list-number" "<Primary><Shift>7")
(gtk_accel_path "<Actions>/core-editor/style-list-bullet" "<Primary><Shift>8")
```
