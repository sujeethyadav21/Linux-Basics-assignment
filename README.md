# Linux-Basics-assignment.

1. Creating and Renaming Files/Directories
Create a directory named test_dir using mkdir.
Inside test_dir, create an empty file called example.txt.
Rename example.txt to renamed_example.txt using mv
Summary:
mkdir test_dir && cd test_dir
touch example.txt
mv example.txt renamed_example.txt

# Create the directory
mkdir test_dir

# Move into the directory
cd test_dir

# Create the file
touch example.txt

# Rename the file
mv example.txt renamed_example.txt

2. Viewing File Contents
Use cat to display the contents of /etc/passwd.
Display only the first 5 lines of /etc/passwd using head.
Display only the last 5 lines of /etc/passwd using tail.
summary:
cat /etc/passwd
head -n 5 /etc/passwd
tail -n 5 /etc/passwd

# Displays the full content of a file
cat [file]

# Shows the first x lines of a file
head -n [x] [file]

# Shows the last x lines of a file
tail -n [x] [file]

3.Searching for Patterns
Use grep to find all lines containing the word "root" in /etc/passwd.
summary:
grep "root" /etc/passwd

grep: The engine that performs the search.

"root": The Pattern. It looks for this specific sequence of letters.

/etc/passwd: The Source. This tells the command where to look.

4. Zipping and Unzipping
Compress the test_dir directory into a file named test_dir.zip using zip.
Unzip test_dir.zip into a new directory named unzipped_dir.
summary:
zip -r test_dir.zip test_dir
unzip test_dir.zip -d unzipped_dir

# Compresses a folder and all its contents (Recursive)
zip	-r

# Extracts a zip file into a specific destination directory
unzip	-d

5. Downloading Files
Use wget to download a file from a URL (e.g., https://example.com/sample.txt).
summary:
wget https://example.com/sample.txt

wget: Short for "World Wide Web Get". It is designed for downloading files over the internet using protocols like HTTP, HTTPS, and FTP.

The URL: This is the direct web address of the file you want to download

6. Changing Permissions
Create a file named secure.txt and change its permissions to read-only for everyone using chmod.
summary:
touch secure.txt
chmod 444 secure.txt
ls -l secure.txt

# Create the File
touch secure.txt

# Change Permissions to Read-Only
chmod 444 secure.txt

# How to Verify the Change
ls -l secure.txt

7. Working with Environment Variables
Use export to set a new environment variable called MY_VAR with the value "Hello, Linux!".
summary:
export MY_VAR="Hello, Linux!"
echo $MY_VAR
Output should be: Hello, Linux!

export: This command tells the shell to make the variable available to all child processes and commands run from that terminal session. Without export, the variable might only stay local to the specific shell you are in.

MY_VAR: This is the name of your variable. By convention, Linux environment variables are written in ALL_CAPS.

="Hello, Linux!": This is the value you are assigning to the name.
