## 💪 Hands-On Exercises

### Exercise 1: Getting Started

### Challenge - 1
![exe1](image.png)
 
![alt text](image-2.png)

### Challenge - 2
![alt text](image-3.png)

![alt text](image-1.png)

### Challenge - 3
![alt text](image-4.png)

![alt text](image-5.png)

### Challenge - 4
![alt text](image-6.png)

![alt text](image-7.png)

### Linux is C000000000000l
![alt text](image-8.png)


### Exercise 2: 2. File System & Navigation

### Challenge - 1
![alt text](image-9.png)

### solution
ubuntu@ip-172-31-33-31:/home$  mkdir -p projects/devops/practice

Explanation:
- mkdir – creates directories.
- -p – creates parent directories if they don't exist.
- projects/devops/practice – nested directory path.

![alt text](image-10.png)

#### Challenge - 2
![alt text](image-11.png)

### solution

touch file1.txt file2.txt file3.txt

ubuntu@ip-172-31-33-31:~/projects/devops/practice$ touch a.txt b.txt c.txt
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ ls
a.txt  b.txt  c.txt
ubuntu@ip-172-31-33-31:~/

#### Challenge - 3

![alt text](image-12.png)

### solution
cp *.txt wildcard/

Command	Purpose
cp	Copies files; originals remain
mv	Moves files; originals disappear from the source
*.txt	Matches all .txt files

![alt text](image-13.png)

#### Challenge - 4

![alt text](image-14.png)

### solution 

# Copy
cp source.txt destination.txt          # Copy file
cp -r sourcedir/ destdir/              # Copy directory recursively

# Move/Rename
mv oldname.txt newname.txt             # Rename
mv file.txt /path/to/destination/      # Move

# Delete
rm filename.txt                        # Delete file
rm -r directory/                       # Delete directory recursively
rm -rf directory/                      # Force delete (no confirmation)
rm -i file.txt                         # Interactive (ask before delete)

ubuntu@ip-172-31-33-31:~/projects/devops/practice/wildcard$ ls
a.txt  b.txt  c.txt
ubuntu@ip-172-31-33-31:~/projects/devops/practice/wildcard$ cd ..
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ mv b.txt notes.txt
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ ls
a.txt  c.txt  notes.txt  wildcard
ubuntu@ip-172-31-33-31:~/projects/devops/practice$


#### Challenge - 5

![alt text](image-15.png)

### solution 


ubuntu@ip-172-31-33-31:~/projects/devops/practice$ echo $PWD
/home/ubuntu/projects/devops/practice
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ ^C

#### Challenge - 6

![alt text](image-16.png)

### solution 


ubuntu@ip-172-31-33-31:~/projects/devops/practice$ ls
a.txt  c.txt  notes.txt  wildcard
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ rm -r wildcard
ubuntu@ip-172-31-33-31:~/projects/devops/practice$ ls
a.txt  c.txt  notes.txt
ubuntu@ip-172-31-33-31:~/projects/devops/practice$




## 🎯 Summary

### Key Commands Learned

| **Category** | **Commands** |
|--------------|--------------|
| Navigation | `pwd`, `ls`, `cd`, `tree` |
| Files | `touch`, `cat`, `cp`, `mv`, `rm` |
| Permissions | `chmod`, `chown` |
| Search | `grep`, `find` |
| Network | `curl`, `ping`, `netstat` |
| Process | `ps`, `top`, `kill` |
| Scripting | Variables, loops, conditionals |

### Best Practices

1. ✅ Always use **tab completion** to avoid typos
2. ✅ Use `man command` to read manual pages
3. ✅ Test destructive commands (`rm -rf`) in safe environments
4. ✅ Use version control (Git) for scripts
5. ✅ Add comments to your scripts

---

## 📖 Further Resources

- [Linux Journey](https://linuxjourney.com/)
- [Bash Scripting Tutorial](https://linuxconfig.org/bash-scripting-tutorial)
- [ExplainShell](https://explainshell.com/) - Explains shell commands
- [Bash Guide for Beginners](https://tldp.org/LDP/Bash-Beginners-Guide/html/)

---

**Next**: [Git Hands-On →](./03-git-hands-on.md)
