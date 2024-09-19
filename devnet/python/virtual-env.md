# Python Virtual Enviroments
- Python Virtual Enviroments, virtualenv or "venvs" allow developers to create isolated enviroments.
- Each venv has a self contained set of dependencies including differing python versions and module installations.
- This allows development on multiple projects to be done on a single machine, without potential conflicts between dependencies.
- Below are some basic commands to get your venv up and running.
  - Be sure to use theses within your project directory.
  - Standard convention is to name the venv "venv" or ".venv".

| Purpose         	| Command                             	| Notes & Flags                                	|
|-----------------	|-------------------------------------	|----------------------------------------------	|
| Create venv     	| python3 -m venv $.venv_name         	| will create directory if one doesn't exist   	|
| Activate venv   	| source $project_folder/bin/activate 	| if within project folder: .venv/bin/activate 	|
| Deactivate venv 	| deactivate                          	|                                              	|
