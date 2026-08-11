# Task
Open a terminal, print your working directory, then navigate to /var/log using an absolute path, back to your home directory using ~, and finally return to /var/log using cd -. List its contents in long, human-readable format.
# Step 1: Check where I am right now
pwd
# Output: /home/student

# Step 2: Go to /var/log using the full path from root
cd /var/log

# Step 3: Confirm I made it
pwd
# Output: /var/log

# Step 4: Go back home using the shortcut
cd ~

# Step 5: Make sure I am home
pwd
# Output: /home/student

# Step 6: Go back to /var/log using the "go back" shortcut
cd -

# Step 7: Show what is in /var/log with all the details and readable file sizes
ls -lh
