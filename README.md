# git-hooks
A collection of [git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks).

## Usage
git hooks only run when they are
- in the hooks subdirectory of your .git directory
- named appropriately (without any extension) and
- executable

The pre-push hook in this repo doesn't do anything except call another script
to perform an action. It is likely that any new hooks added here will use the
same pattern. This is structure is probably overkill since I don't use hooks
much, but it may have some benefits:
- maintenance is slightly easier because we can easily turn on and off specific
  functionality if a hook does more than one thing
- debugging is easier since we can run the script that does the actual work
  standalone
- more files looks like we did more work
