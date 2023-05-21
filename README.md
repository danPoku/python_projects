# python_projects

### Website blocker code from Data Flair
This code was originally published by https://data-flair.training/blogs/python-website-blocker-project/

### Update to the Unblock function
The unblock function in the original script was not functional as it could not remove websites from the hosts file
This updated version solves the problem

### Run code as administrator - run_as_admin()
In the original script, you may encounter a permission error when blocking a website. This occurs because the script does not have administrator privileges to write to the hosts system file. The run_as_admin() function added to the script checks if the script is being executed with admin privileges. If not, it will prompt with the User Account Control dialogue box to give admininstrator privileges to run the script.
