Shell Basics Tasks. From 0 - 18 are scripts and must start with a Shebang. After a script is created using vi or emacs, we give the system permission to read the script by writing chmod 755 FileName, afterwards write chmod u+x FileName. We do this just before writing git add , committing and pushing.

0 - pwd     this is used to print the absolute path name of the working directory

1 - ls      this is used to list directory content

2 - cd      this is used to change directory

3 - ls -l   this is used to list the directory content in long form

4 - ls -la  this is used to list directory content in long form, including hidden files

5 - ls -la  this is used to list files (including hidden files in a long format) in a directory.

6 - mkdir /tmp/my_first_directory   this is used to creat the my_first_directory dir inside tmp directory

7 - mv /tmp/betty /tmp/my_first_directory/betty   this is used to mvoe betty which is inside tmp dir into my_first_directory dir which is also inside the tmp dir

8 - rm /tmp/my_first_directory/betty    this is used to remove the file betty from the my_first_directory dir

9 - rm -r /tmp/my_first_directory     this used to remove the my_first_directory dir which is inside tmp dir

10 - cd -     this is used to change the working directory to the previous directory

11 - ls -la . .. /boot    this is used to list all files in the current directory and the parent of the working dir and the /boot dir in long format

12 - file /tmp/iamafile   this is used to print the type of file named iamafile

13 - ln -s /bin/ls __ls__     this is used to create a symbolic link called __ls__ inside /bin/ls

14 - cp *.html ../            This is used to copy all html files from the current working directory to the parent working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory

15 - mv [A-Z]* /tmp/u         this is used to move all files that begin with an uppercase letter to the directory /tmp/u

16 - rm *~                    this is used to delete all files in the current working directory that ends with the character ~

17 - mkdir {welcome/, welcome/to/, welcome_/to/school}  this is used to create multiple directories

18 - ls -map    this is used to list all the files and directories of the current directory, separated by commas. The directory names should end with a slash, files and directories starting with a dot should be listed, etc.

19 - 0 string SCHOOL School data
!:mime School ( this is not a script so it won't star with a Shebang. It's a simple magic file).




