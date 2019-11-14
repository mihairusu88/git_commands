### Initialize
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><code>git init</code></td>
			<td>Initialize a local Git repository</td>
		</tr>
	</tbody>
</table>


### Create
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git clone https://github.com/[username]/[repository].git</code><br/>
				<code>git clone ssh://git@github.com/[username]/[repository].git</code>
			</td>
			<td>Create a local copy of a remote repository</td>
		</tr>
		<tr>
			<td colspan="2"><b>E.g:</b> <code>git clone https://github.com/johndoe/my-repository.git</code></td>
		</tr>
		<tr>
			<td colspan="2"><b>E.g:</b> <code>git clone ssh://git@github.com/johndoe/my-repository.git</code></td>
		</tr>
	</tbody>
</table>

### Status
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git status</code>
			</td>
			<td>Check status</td>
		</tr>
	</tbody>
</table>

### Adding files
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git add [filename]</code>
			</td>
			<td>Add a filename to the staging area</td>
		</tr>
		<tr>
			<td>
				<code>git add -A</code><br />
				<code>git add .</code>
			</td>
			<td>Add all new and changed files to the staging area</td>
		</tr>
	</tbody>
</table>

### Commit changes
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git commit -m "[message]"</code>
			</td>
			<td>Commit changes</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git commit -m "Added some new code in index.html"</code>
			</td>
		</tr>
	</tbody>
</table>

### Branching & Merging
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git branch</code>
			</td>
			<td>List branches (the asterisk denotes the current branch)</td>
		</tr>
		<tr>
			<td>
				<code>git branch -a</code>
			</td>
			<td>List all branches (local and remote)</td>
		</tr>
		<tr>
			<td>
				<code>git branch [branch_name]</code>
			</td>
			<td>Create a new branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git branch development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git branch -d [branch_name]</code>
			</td>
			<td>Delete a branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git branch -d development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git checkout -b [branch_name]</code>
			</td>
			<td>Create a new branch and switch to it</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git checkout -b development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git checkout [branch_name]</code>
			</td>
			<td>Switch to a branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git checkout development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git checkout -</code>
			</td>
			<td>Switch to the branch last checked out</td>
		</tr>
		<tr>
			<td>
				<code>git checkout -- [filename]</code>
			</td>
			<td>Discard changes to a file</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git checkout -- index.html</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git merge [branch_name]</code>
			</td>
			<td>Merge a branch into the active branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git merge development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git merge [source_branch] [target_branch]</code>
			</td>
			<td>Merge a branch into a target branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git merge development master</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git stash</code>
			</td>
			<td>Stash changes in a dirty working directory</td>
		</tr>
		<tr>
			<td>
				<code>git stash clear</code>
			</td>
			<td>Remove all stashed entries</td>
		</tr>
	</tbody>
</table>

### Updating Projects
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git push origin [branch_name]</code>
			</td>
			<td>Push a branch to your remote repository</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git push origin development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git push -u origin [branch_name]</code>
			</td>
			<td>Push changes to remote repository (and remember the branch)</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git push -u origin development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git push</code>
			</td>
			<td>Push changes to remote repository (remembered branch)</td>
		</tr>
		<tr>
			<td>
				<code>git push origin --delete [branch name]</code>
			</td>
			<td>Delete a remote branch</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git push origin --delete development</code>
			</td>
		</tr>
		<tr>
			<td>
				<code>git reset --hard HEAD</code>
			</td>
			<td>Scrap uncommitted state and return the working tree to the last committed state</td>
		</tr>
		<tr>
			<td>
				<code>git reset --hard HEAD~1</code><br>and then<br>
				<code>git push origin master --force</code>
			</td>
			<td>Delete the latest commit, and return to the one previous (one before HEAD)</td>
		</tr>
		<tr>
			<td>
				<code>git rm --cached [file/folder]</code>
			</td>
			<td>Stop a file being tracked (but do not delete it from the working directory, add to .gitignore etc after this)</td>
		</tr>
	</tbody>
</table>

### Inspection & Comparison
***
<table>
	<thead>
		<tr>
			<th>Command</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				<code>git log</code>
			</td>
			<td>View changes</td>
		</tr>
		<tr>
			<td>
				<code>git log --summary</code>
			</td>
			<td>View changes (detailed)</td>
		</tr>
		<tr>
			<td>
				<code>git diff [source_branch] [target_branch]</code>
			</td>
			<td>Preview changes before merging</td>
		</tr>
		<tr>
			<td colspan="2">
				<b>E.g:</b> <code>git diff development master</code>
			</td>
		</tr>
	</tbody>
</table>
