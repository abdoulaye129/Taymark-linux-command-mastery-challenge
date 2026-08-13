# Commands Covered
`mkdir` creates a new folder. You give it a name, and it makes that folder right where you are.

`mkdir -p `creates a whole path of folders at once. For example, `mkdir -p practice/2026/april` builds all three levels even if none of them exist yet.

`touch` makes a new empty file. If the file already exists, it just updates the timestamp without changing the content.

`cp` copies a file from one place to another. You need to give it the source and the destination.
`cp -r` copies a folder and everything inside it. The `-r` stands for recursive, which means it goes into the folder and copies all sub‑folders and files.

`mv` moves a file or folder to a new location. You can also use it to rename things by moving them to the same folder with a new name.

`rm` removes a file. Be careful with this one; once it is gone, it is gone.

`rm -r` removes a folder and everything inside it. That is how you delete a whole directory with its contents.

`rm -rf` forcefully removes a folder without asking for confirmation. The `-f` stands for force. It is dangerous because it does not warn you.

`rmdir` removes an empty folder. If the folder has any files or sub‑folders, it fails. That makes it safer than rm -r when you only want to clean up empty directories
