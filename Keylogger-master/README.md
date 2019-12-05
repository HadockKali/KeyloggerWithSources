# A simple keylogger for Windows

## Windows
To change visibility of the window set the `#define` in line 9 to `visible` or `invisible`.

Simply compile into an .exe, and then run. Visual Studio is good for this.

- `invisible` makes the window of the logger disappear, and it also starts up hidden from view. Note that it is still visible in the task manager.
- `visible` is visible, and the window does not close when typing. Great for testing it out.

Both of these save the keystrokes to a .txt file when closed.

> Note that sometimes your compiler may through up errors. If it does, keep compiling - the program still works. As always, please create an issue if you have a problem.


### Uninstall
`$ sudo make uninstall`

Will uninstall the program, but not the logs.

---


### How to run it?

To run it just type `keylogger` and it'll run:
```
keylogger --log-file keylogger.log 
RECORD extension version 1.13
```

The keylogger is now running! It will log your strokes to the file you
specified. Stop it by hitting the cancel key (grave or \`, if not set with
`--cancel-key`. That's the one under escape on a standard keyboard.)

You can make it run on startup:

`$ sudo make startup`

---
#### Uses

Some uses of a keylogger are:

- Business Administration: Monitor what employees are doing.
- School/Institutions: Track keystrokes and log banned words in a file.
- Personal Control and File Backup: Make sure no one is using your computer when you are away.
- Parental Control: Track what your children are doing.
- Self analysis

---
