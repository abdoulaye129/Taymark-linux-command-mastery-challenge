# Day 2: Creating, Copying, Moving, Deleting
Phase 1 - File Navigation & Filesystem Mastery | Day 2 of 30
## Commands covered today
See commands.md for the full list of 10 commands. I wrote each one in my own words and explained when I would use it.

## What I practiced
The drill asked me to build a nested folder structure in one command (practice/2026/april), create three empty files inside it, copy the whole folder to a backup location, rename one of the files, and then safely remove any empty directories left behind. It forced me to use `mkdir -p, touch, cp -r, mv, and rmdir` in the right order.

## What surprised me
I tried `rmdir` on a folder that still had files, and it refused to delete it. That is actually a good safety net. I used `rm -r` to remove the copied folder with everything inside, but I had to be careful not to delete the original.

## Evidence
Screenshot or terminal copy of the drill in evidence/.

## Related
Previous day: Day 1: Where Am I? Basic Orientation

Next day: Day 3: Reading & Inspecting Files
