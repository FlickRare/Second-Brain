# Package Installer for Python

- Package Installer for Python or "pip" is the primary means to install packages from the Python Package Index.
  - A user can specify other indexes too.
- Pip may need to be installed via the OS package manager.
- If using pip in conjunction with virtualenv, pay special attention to the context of your commands.
  - Avoid listing, installing, or uninstalling packages to the wrong venv or directly to the OS installtion of Python.
- Basic commands below:

| Purpose                             	| Command                                                   	| Notes & Flags                                                       	|
|-------------------------------------	|-----------------------------------------------------------	|---------------------------------------------------------------------	|
| Install package                     	| python 3 -m pip install $package                          	|                                                                     	|
| Uninstall package                   	| python 3 -m pip uninstall $package                        	|                                                                     	|
| List packages                       	| python 3 -m pip                                           	| -l, --local : only shows packages in venv                           	|
| Show where pip installs             	| pip -V                                                    	| Useful when troubleshooting dependencies while using virtualenv     	|
| Show where python looks for modules 	| import sysconfig; print(sysconfig.get_paths()["purelib"]) 	| Again useful to see if depencies are working correctly in your venv 	|