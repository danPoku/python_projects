# python_projects

### Website blocker code from Data Flair
This code was originally published by https://data-flair.training/blogs/python-website-blocker-project/

### Update to the Unblock function
The unblock function in the original script was not functional as it could not remove websites from the hosts file
This updated version solves the problem. 
- In the updated version, we open and read the hosts file content to the `file_content` variable
- Then we open the hosts file again but this time, clear the contents of the file and assign the empty file to the variable `f`
- We initialize a variable called `found_website` to `False`. This tracks whether any of the websites to be unblocked are found in the hosts file
- Iterate over each line in the `file_content` list and if a line contains any of the websites from `Website` we set `found_website` to `True`. Else we write the line back to the hosts file
- After iterating through all the lines, we check the value of `found_website`. If it's `True`, we display the "Unblocked" message on the window, indicating that the website(s) have been successfully removed. Otherwise, we display a "Website not found" message to indicate that the specified website(s) were not present in the hosts file.

### Run code as administrator - run_as_admin()
In the original script, you may encounter a permission error when blocking a website. This occurs because the script does not have administrator privileges to write to the hosts system file. The run_as_admin() function added to the script checks if the script is being executed with admin privileges. If not, it will prompt with the User Account Control dialogue box to give admininstrator privileges to run the script.
