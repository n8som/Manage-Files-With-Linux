# Manage-Files-With-Linux

<h2>Activity overview</h2>

In this lab activity, I’ll use Linux commands to modify a directory structure and the files it contains.

I’ll also use the nano text editor to add text to a file.

I previously learned that directories help me organize subdirectories and files in Linux. As a security analyst, creating, removing, and editing directories and files are core tasks I’ll need to perform to help me manage data.

When data is well organized, I can more easily detect issues and keep data safe.

<h2>Scenario</h2>

In this scenario, I need to ensure that the ```/home/analyst``` directory is properly organized.

I have to make a few changes to the ```/home/analyst``` directory and the files it contains.

I also have to edit a file to record the changes or updates I make to the directory.

When I start, the ```/home/analyst``` directory contains the following subdirectories and files:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/665c680a-b412-4313-bd5f-c67a53b58086)

I need to modify the ```/home/analyst``` directory to the following directory and file structure:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/f46b23bb-516a-4aa6-bb8e-bf2f5cec2eac)

Here’s how I’ll do this: First, I’ll create a new subdirectory called logs in the ```/home/analyst``` directory. Next, I’ll remove the ```temp``` subdirectory. Then, I’ll move the ```Q3patches.txt``` file to the ```reports``` subdirectory and delete the ```tempnotes.txt``` file. Finally, I’ll create a new ```.txt``` file called ```tasks``` in the ```notes``` subdirectory and add a note to the file describing the tasks I've performed.

<h2>Task 1. Create a New Directory</h2>

First, I must create a dedicated subdirectory called ```logs```, which will be used to store all future log files.

1. Create a new subdirectory called ```logs``` in the ```/home/analyst``` directory.
2. List the contents of the ```/home/analyst``` directory to confirm that I’ve successfully created the new ```logs``` subdirectory.

The output should list the original three directories and the new ```logs``` subdirectory:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/0024b14a-ffc8-4d41-ae3d-36a6f14d2c82)

<h2>Task 2. Remove a Directory</h2>

Next, I must remove the ```temp``` directory, as I’ll no longer be placing items in it.

1. Remove the ```/home/analyst/temp``` directory.
2. List the contents of the ```/home/analyst``` directory to confirm that I have removed the ```temp``` subdirectory.

The ```temp``` directory should no longer be listed:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/960101d0-41a3-4840-8bc3-a9e9dc18ad4d)

<h2>Task 3. Move a File</h2>

The ```Q3patches.txt``` file contains notes taken on third-quarter patches and is now in the correct reporting format.

I must move the  ```Q3patches.txt``` file from the ```notes``` directory to the ```reports``` directory.

1. Navigate to the ```/home/analyst/notes``` directory.
2. Move the ```Q3patches.txt``` file from the ```/home/analyst/notes``` directory to the ```/home/analyst/reports``` directory.
3. List the contents of the ```/home/analyst/reports``` directory to confirm that I have moved the file successfully.

When I list the contents of the ```reports``` directory, it should show that three quarterly report files are now in the ```reports``` directory:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/e87cd12a-f595-46c0-a698-36932f75d676)

<h2>Task 4. Remove a file</h2>

Next, I must delete an unused file called ```tempnotes.txt``` from the ```/home/analyst/notes``` directory.

1. Remove the ```tempnotes.txt``` file from the ```/home/analyst/notes``` directory.
2. List the contents of the ```/home/analyst/notes``` directory to confirm that I’ve removed the file successfully.

No files should be listed in the ```notes``` directory:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/a80d9faa-6d3c-4a24-850f-7a9db79d5f77)

<h2>Task 5. Create a new file</h2>

Now, I must create a file named ```tasks.txt``` in the ```/home/analyst/notes``` directory that I’ll use to document completed tasks.

1. Use the ```touch``` command to create an empty file called ```tasks.txt``` in the ```/home/analyst/notes``` directory.
2. List the contents of the ```/home/analyst/notes``` directory to confirm that I have created a new file.

A file called ```tasks.txt``` should now exist in the ```notes``` directory:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/c7db0f18-22ec-455f-b805-b33663463afb)

<h2>Task 6. Edit a file</h2>

Finally, I must use the nano text editor to edit the ```tasks.txt``` file and add a note describing the tasks I’ve completed.

1. Using the nano text editor, open the ```tasks.txt``` file that is located in the ```/home/analyst/notes``` directory.

Note: This action changes the shell from the normal Bash interface to the nano text editor interface.

2. Copy and paste the following text into the text input area of the nano editor:

    Completed tasks

     1. Managed file structure in /home/analyst

5. Press CTRL+X to exit the nano text editor.

This triggers a prompt asking "Save modified bufferer?"

4. Press Y to confirm that you want to save the new data to the file. (Answering "no" will discard changes.)
5. Press ENTER to confirm that File Name to Write is ```tasks.txt```.
6. Note: The recommended sequence of commands for saving a file with the nano text editor is to use CTRL+O to tell nano to save the file and then use CTRL+X to exit immediately.
7. In this web-based lab environment, the CTRL+O command is intercepted by the web browser and is interpreted as a request to save the web page. The sequence used here is a commonly used alternative that achieves the same end result.
8. Use the ```clear``` command to clear the Bash shell window and remove any traces of the nano text input area.

Note: Most Bash shells typically handle the screen cleanup after you exit nano. In this lab environment, nano sometimes leaves some text clutter around the edges of the screen that the ```clear``` command cleans up for me.

9. Display the contents of the ```tasks.txt``` file to confirm that it contains the updated task details.

This file should now contain the contents of the ```tasks.txt``` file that I added and saved in previous steps:

![image](https://github.com/n8som/Manage-Files-With-Linux/assets/110139109/3d39af9e-9dc6-4955-843e-2dd164634940)

<h2>Conclusion</h2>

I now have practical experience in using basic Linux Bash shell commands to

- create and remove directories,
- copy, move, and remove files, and
- edit files with the nano text editor.

I’m well on my way to managing directories and files in a Linux environment!

