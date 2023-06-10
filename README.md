**Automated Downloads Organizer**

This script helps organize files in the `Downloads` folder by moving them to specific folders based on their file extensions. It also includes an additional feature to move screenshots from the desktop to a separate folder.

### Prerequisites

- Python 3.x installed on your system

### Usage

1. Open a text editor and create a new file.

2. Copy and paste the provided code into the file.

3. Save the file with a `.py` extension, for example, `downloads_organizer.py`.

4. Open a terminal or command prompt and navigate to the directory where the script file is saved.

5. Run the script by executing the following command:

   ```shell
   python downloads_organizer.py
   ```

6. The script will start monitoring the `Downloads` folder and automatically move files to their respective folders based on their extensions.

7. Screenshots saved on the desktop will also be moved to a separate `Screenshots` folder.

8. The script will run continuously until you manually stop it by pressing `Ctrl + C`.

### Configuration

The script comes with pre-defined destination folders for various file extensions. You can modify these folders according to your preferences by editing the `file_extensions` dictionary in the script.

```python
file_extensions = {
    ".jpg": images_folder,
    ".jpeg": images_folder,
    ".gif": images_folder,
    ".png": images_folder,
    ".mp4": videos_folder,
    ".mov": videos_folder,
    ".avi": videos_folder,
    ".mp3": audios_folder,
    ".wav": audios_folder,
    ".aac": audios_folder,
    ".zip": os.path.join(downloads_folder, "Project"),
    ".sql": os.path.join(downloads_folder, "Database"),
    ".pdf": pdf_folder,
    ".dmg": software_folder
}
```

You can add, remove, or modify file extensions and their corresponding destination folders to suit your needs.

### Note

Make sure to keep the script running in the background to continuously organize your files. You can add the script to your system's startup programs to automate the process.

Please note that this script is provided as a starting point and may require customization based on your specific requirements and folder structure.

**Disclaimer**: Use this script at your own risk. Make sure to backup important files before running the script, as it involves moving files on your system. The script is provided as-is without any warranty.

