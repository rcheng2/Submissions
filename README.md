For this assignment, I made a folder called Submissions. 

To change the permissions so that only the TA and the Professor can read or execute from the folder, first you use groups command to compare it to the TA and another students to find a group that only the TA and Professor have in common and not the student. 

One such group I found was eg-aff-faculty@gsuad.gsu.edu.
Then you would use chgroup to change the group of the Submissions folder.

chgroup -R eg-aff-faculty@gsuad.gsu.edu Submissions

The other way to do it is:

chown :eg-aff-faculty@gsuad.gsu.edu Submissions

To make a tar file: tar -czvf Submissions.tar.gz Submissions/

After that I copied The Hunger Games from the Professors 3320 folder into the submissions folder using cp and the absolute path
cp /home/cumoja1/The\ Hunger\ Games.txt Submissions/

After that I used :%s/Katniss/Roxane/g to replace all the characters with my name.
Next I saved the final product and quit with :wq!

The next step was renaming the file to My Hunger Games using the mv command.

