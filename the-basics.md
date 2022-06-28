1. Create a folder called git-basic
>mkdir git-basic

2. cd into the git-basic folder
>cd git-basic

3. Create a file called first.txt
>touch first.txt

4. Initialize an empty git repository
>git config --global user.name "anisaauralita"
>git config --global user.email anisaauralita20@gmail.com
>git init .

5. Add first.txt to the staging area
>touch first.txt

6. Commit with the message "adding first.txt"
>git add first.txt
>git commit -m "add first.txt"

7. Check out your commit with git log
>git log

8. Create another file called second.txt
>touch second.txt

9. Add second.txt to the staging area
>git add second.txt

10. Commit with the message "adding second.txt"
>git commit -m "add second.txt"

11. Remove the first.txt file
>git rm first.txt

12. Add this change to the staging area
>git add .

13. Commit with the message "removing first.txt"
>git commit -m "removing first.txt"

14. Check out your commits using git log
>git log