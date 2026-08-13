# Task
Create a nested folder structure `practice/2026/april` in one command, create three empty files inside it, copy the folder to a backup location, rename one file, then safely delete only the empty directories left behind.
# Step 1: Create nested folder structure
mkdir -p practice/2026/april

# Step 2: Create three empty files inside it
touch practice/2026/april/file1.txt
touch practice/2026/april/file2.txt
touch practice/2026/april/file3.txt

# Step 3: Copy folder to backup location
cp -r practice practice_backup

# Step 4: Rename one file
mv practice/2026/april/file2.txt practice/2026/april/renamed.txt

# Step 5: Delete empty directories left behind
