The Game: Bash Battle Arena 🎮


Level 1:The Basics
Mission: Create a directory named Arena and then inside it, create three files: warrior.txt, mage.txt, and archer.txt. List the contents of the Arena directory.

Steps:
1. mkdir Arena
2. touch warrior.txt mage.txt archer.txt
3. cd Arena
4. ls

---

Level 2: Variables and Loops
Mission: Create a script that outputs the numbers 1 to 10, one number per line.

Steps:
for (( i=1; i<=10; i++ ))
do
    echo "$i"
done

---

Level 3: Conditional Statements
Mission: Write a script that checks if a file named hero.txt exists in the Arena directory. If it does, print Hero found!; otherwise, print Hero missing!.

file = "/Arena/hero.txt"

if [[ -f "$file" ]]; then
echo "Hero found!"
else
echo "Hero missing!"
fi

<!--
-f checks file exists
-->

---

Level 4:File Manipulation
Mission: Create a script that copies all .txt files from the Arena directory to a new directory called Backup.

mkdir backup

cp Arena/*.txt backup

---

Level 5: The Boss Battle - Combining Basics

Mission: Combine what you've learned! Write a script that:
1. Creates a directory names 'Battlefield'
2. Inside Battlefield, create files named knight.txt, sorcerer.txt, and rogue.txt.
3. Check if knight.txt exists; if it does, move it to a new directory called Archive.
4. List the contents of both Battlefield and Archive.

#create Battlefield
mkdir Battlefield

#creates files 
cd Battlefield
touch knight.txt sorcerer.txt rogue.txt
cd ..

#check knight
mkdir Archive

if [[ -f "/Battlfield/knight.txt" ]]; then
echo "file moved"
else
echo "does not exist"
fi

ls Battlefield Archive


