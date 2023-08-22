# Some Python and Conda Memo

## Virtualenv Tutorial 
- https://www.simononsoftware.com/virtualenv-tutorial-part-2/
- https://web.archive.org/web/20160404222648/
- https://iamzed.com/2009/05/07/a-primer-on-virtualenv/
- https://www.dabapps.com/insights/introduction-to-pip-and-virtualenv-python/
- https://thepythonguru.com/python-virtualenv-guide/
- https://realpython.com/python-virtual-environments-a-primer/
- https://realpython.com/python-virtual-environments-a-primer/
- https://github.com/zookeepr/zookeepr/wiki
- A Complete Guide to Python Virtual Environments https://www.dataquest.io/blog/a-complete-guide-to-python-virtual-environments/

## Memo about Conda
### Packages:
- _*conda install/remove/update/list package_name*_
- _*conda create -n env_name (python = x.x0) list_of_packages*_
- _*conda activate env_name*_
- _*conda deactivate*_
- _*conda env remove -n env_name*_
- _*conda env list*_
- _*conda env export > env_conf_name.yaml*_
- _*conda env create -f env_conf_name.yaml*_

### Uninstalling Anaconda Distribution
1. Full Uninstall
    1. conda install anaconda-clean
    2. anaconda-clean —yes
2. Simple remove
    1. rm -rf anaconda3
    2. rm -rf ~/anaconda3
    3. rm -rf ~/opt/anaconda3
    4. Remove from path: export PATH="/Users/jsmith/anaconda3/bin:$PATH"

## Memo about Python Management
### Uninstall
#### For Mac - Manually:
1. Open Activity Monitor and check whether some processes are still active.
2. Then go to the Application folder in Finder and move Python to Trash.
3. Find and remove all the service files Python has created while you were using it.
    * ~/Library/Frameworks/Python.framework
    * ~/Library/Application Support/com.apple.sharedfilelist/com.apple.LSSharedFileList.ApplicationRecentDocuments/org.python.idle.sfl
    * ~/Library/Application Support/com.apple.sharedfilelist/com.apple.LSSharedFileList.ApplicationRecentDocuments/org.python.pythonlauncher.sfl
    * ~/Library/Saved Application State/org.python.IDLE.savedState
    * ~/Library/Saved Application State/org.python.PythonLauncher.savedState
    * ~/private/var/db/receipts/org.python.Python.PythonUnixTools-3.6.bom
    * ~/private/var/db/receipts/org.python.Python.PythonFramework-3.6.bom
    * ~/private/var/db/receipts/org.python.Python.PythonDocumentation-3.6.bom
    * ~/private/var/db/receipts/org.python.Python.PythonApplications-3.6.bom
    * ~/private/var/db/receipts/org.python.Python.PythonFramework-3.6.plist
    * ~/private/var/db/receipts/org.python.Python.PythonUnixTools-3.6.plist
    * ~/private/var/db/receipts/org.python.Python.PythonApplications-3.6.plist
    * ~/private/var/db/receipts/org.python.Python.PythonDocumentation-3.6.plist
#### For Mac - Terminal:
1. Move Python to Trash.
2. Open the Terminal app and type the following command in the window: ~ [user name] sudo rm -rf /Applications/Python\ 3.6/
3. It will require you to enter your administrator password to confirm the deletion.


