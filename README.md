# Automatic File Sorter

This is a Python program that can sort files into different folders based on their file extensions. The program uses the shutil module to move files to their respective folders. The user can specify the path of the folder that needs to be sorted and the names of the folders where the different file types need to be moved. The program checks if the folders already exist and creates them if they do not.

## Requirements

To use the Automatic File Sorter, the user needs to have Python 3 installed on their system. The program also requires the shutil module, which is included in the Python Standard Library.

## Usage

To use the Automatic File Sorter, the user needs to run the program in the command line and specify the path of the folder that needs to be sorted and the names of the folders where the different file types need to be moved.

For example, to sort files in the "Downloads" folder on a Windows system, the user can run the following command:

```
python sorter.py C:\Users\Username\Downloads --docs Documents --music Music --videos Videos --images Pictures
```

This command will sort all files in the "Downloads" folder and move them to their respective folders based on their file extensions. Files with the ".docx", ".pdf", and ".txt" extensions will be moved to the "Documents" folder, files with the ".mp3" and ".wav" extensions will be moved to the "Music" folder, files with the ".mp4" and ".avi" extensions will be moved to the "Videos" folder, and files with the ".jpg", ".png", and ".gif" extensions will be moved to the "Pictures" folder.

## Benefits

This project demonstrates the proficiency in using Python and their ability to work with file operations in Python. It also showcases their problem-solving skills and attention to detail. By creating this program, it shows that they can automate repetitive tasks and enhance the efficiency of file management. Overall, this project is an excellent addition to the portfolio and would be a valuable asset to any team that requires file management automation.

## Implementation Details

The program starts by defining a path variable that points to the folder that needs to be sorted. Next, the program creates three subfolders with predefined names for different types of files. This is done using a for loop that iterates through a list of folder names and creates a folder with that name if it does not exist already.

After creating the subfolders, the program gets a list of all files in the main folder using the os.listdir() method. It then iterates through each file and uses the shutil.move() method to move the file to the appropriate subfolder based on its file extension. For example, if the file has a .jpg extension, it is moved to the "image files" subfolder.

Finally, if a file does not match any of the predefined file extensions, the program prints a message indicating that the file was not moved.

Overall, this program provides an efficient way to organize a cluttered folder by automatically sorting files into different subfolders based on their file types.
