<h1>Package Installer for Python</h1>

- Package Installer for Python or "pip" is the primary means to install packages from the Python Package Index.
  - A user can specify other indexes too.
- Pip may need to be installed via the OS package manager.
- If using pip in conjunction with virtualenv, pay special attention to the context of your commands.
  - Avoid listing, installing, or uninstalling packages to the wrong venv or directly to the OS installtion of Python.
- Basic commands below:
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
Install package
</td>
<td width="40%">
python 3 -m pip install $package
</td>
<td width="40%">
</td>
</tr>
<td width="20%">
Uninstall package
</td>
<td width="40%">
python 3 -m pip uninstall $package
</td>
<td width="40%">
</td>
</tr>
<td width="20%">
List packages
</td>
<td width="40%">
python 3 -m pip
</td>
<td width="40%">
-l, --local : only shows packages in venv
</td>
</tr>
<td width="20%">
Show where pip installs
</td>
<td width="40%">
pip -V
</td>
<td width="40%">
Useful when troubleshooting dependencies while using virtualenv
</td>
</tr>
<td width="20%">
Show where python looks for modules
</td>
<td width="40%">
import sysconfig; print(sysconfig.get_paths()["purelib"])
</td>
<td width="40%">
Again useful to see if depencies are working correctly in your venv
</td>
</tr>
</table>