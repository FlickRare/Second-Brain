<h1>git</h1>
- Git is a version control system that operateas independantly of network access to a central server.
<h1>Commands:</h1>
<table>
<tr>
<td width="40%">
<strong>
Purpose
</strong>
</td>
<td width="20%">
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
<tr>
<td width="40%">
<strong>
Display the state of the working dir and staging area
</strong>
</td>
<td width="20%">
<strong>
git status
</strong>
</td>
<td width="40%">
<strong>
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Lists commits in reverse chronological order
</strong>
</td>
<td width="20%">
<strong>
git log
</strong>
</td>
<td width="40%">
<strong>
--all ensures all refs/ and HEAD are listed as well
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Add altered files to staging area ahead of commit
</strong>
</td>
<td width="20%">
<strong>
git add
</strong>
</td>
<td width="40%">
<strong>
"git add ." adds all changed made within the dir
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Reset staging area
</strong>
</td>
<td width="20%">
<strong>
git reset HEAD
</strong>
</td>
<td width="40%">
<strong>
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Save changed from staging area to the repo
</strong>
</td>
<td width="20%">
<strong>
git commit
</strong>
</td>
<td width="40%">
<strong>
-m "$message" to bypass text edit for simpler commits
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Revert the repo to a previous version (version control!)
</strong>
</td>
<td width="20%">
<strong>
git reset ($sha1)
</strong>
</td>
<td width="40%">
<strong>
"$sha1" = the ID of specfic commit you want ot revert to 
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Add your changes to a remote repo (github?)
</strong>
</td>
<td width="20%">
<strong>
git push
</strong>
</td>
<td width="40%">
<strong>
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Set the location of the remote repo for current instance of git
</strong>
</td>
<td width="20%">
<strong>
git remote add origin $url
</strong>
</td>
<td width="40%">
<strong>
"$url" = url of remote repository (click green "code" button)
</strong>
</td>
</tr>
<tr>
<td width="40%">
<strong>
Download a remote repository
</strong>
</td>
<td width="20%">
<strong>
git clone $url
</strong>
</td>
<td width="40%">
<strong>
$url = url of remote repository
</strong>
</td>
</tr>