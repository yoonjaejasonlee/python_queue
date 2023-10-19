## Git Commit Intervention Setup

To Setup commit intervention with the extension our "pre-commit" script can be used.

### Usage

1. Copy the `pre-commit` file from the `src` directory to the `.git/hooks/` directory of your Git repository.

On Windows: Navigate to projects root directory and run `copy "src\commitIntervention\pre-commit" .git\hooks\`
On Linux: Navigate to projects root directory and run `cp commitIntervention/pre-commit .git/hooks/`

2. Make the script executable by running the following command in your repository's root directory: `chmod +x .git/hooks/pre-commit` (Linux Only).

3. Change line 5 of the script `export RUN_CODE_REVIEW=false` to `export RUN_CODE_REVIEW=true` to toggle automatic review when commit on. (Remember to re-copy file to `.git/hooks/` after changing this variable).
