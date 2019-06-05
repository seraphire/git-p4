**2019-06-05** 
Make the following changes:
  - Changed the default format for the diffcmd in p4 submit method. Added the `--git-dir` and `--work-tree` parameters to the git command. Before this command is executed, the directory is changed, and the git repository cannot be located.
  - Added a check for `core.autocrlf` if patching fais and the Operating System is Windows. This will show a helpful message suggesting that it be set.
  - Added a new hook - `p4-pre-edit-changelist` that allows for a hook that will modify the generated changelist document prior to showing it for edit.
  - Added a new method `pathJoin` that will strip off quotes if a portion of the path is escaped.
  - Moved the code for running a hook to `runHook` to allow for more generalization and executing other hooks (like the p4-pre-edit-changelist noted above.)

**2019-06-04**

  - Added a Visual Studio 2019 project. This is optional and provided for Windows Debugging.
