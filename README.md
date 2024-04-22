# Gym-Git-Exercise-Solutions
Git &amp; GitHub Bundle Exercises
<!-- These are changes so far in my exercise1 project:
*changes to the project by doing the following to the existing file(added a file, edited two of them) -->

<!-- for the  -->

```bash
hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 0727649 this is the first commit on exercise1

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ touch about.html

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add --all

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 0727649 this is the first commit on exercise1

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ touch team.html

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add --all

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 0727649 this is the first commit on exercise1

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop about.html
error: about.html is not a valid reference

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{<about>}
bash: about: No such file or directory

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{<about.html>}
bash: about.html: No such file or directory

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{<about.html>}
bash: about.html: No such file or directory

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 0727649 this is the first commit on exercise1
stash@{1}: WIP on dev: 0727649 this is the first commit on exercise1
stash@{2}: WIP on dev: 0727649 this is the first commit on exercise1

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (3e1863ec18f3809f881f0953e9f87c0c4b183f12)

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git add --all

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "the second commit after using stash and retrive by stash pop"
[dev 51a27d2] the second commit after using stash and retrive by stash pop
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

hopem@Tesy MINGW64 ~/OneDrive/Desktop/Gym-Git-Exercise-Solutions (dev)
$
```