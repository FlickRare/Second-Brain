<h1>Python Virtual Enviroments</h1>

- Python Virtual Enviroments, virtualenv or "venvs" allow developers to create isolated enviroments.
- Each venv has a self contained set of dependencies including differing python versions and module installations.
- This allows development on multiple projects to be done on a single machine, without potential conflicts between dependencies.
- Below are some basic commands to get your venv up and running.
  - Be sure to use theses within your project directory.
  - Standard convention is to name the venv "venv" or ".venv".

<table>
<tr>
<td width="20%">
<strong>
Purpose
</strong>
</td>
<td width="40%">
<strong>
Command
</strong>
</td>
<td width="40%">
<strong>
Notes & Flags
</strong>
</td>
</tr>
<td width="20%">
Create venv
</td>
<td width="40%">
python3 -m venv $.venv_name
</td>
<td width="40%">
will create directory if one doesn't exist
</td>
</tr>
<td width="20%">
Activate venv
</td>
<td width="40%">
source $project_folder/bin/activate
</td>
<td width="40%">
if within project folder: .venv/bin/activate
</td>
</tr>
<td width="20%">
Deactivate venv
</td>
<td width="40%">
deactivate
</td>
<td width="40%">
</td>
</tr>
</table>