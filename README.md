# git-pre-commit-hook
Git pre-commit hook for unit testing and running spotless for spring-boot

Copy the `pre-commit` file to your repository's .git/hooks folder.

Example gradle task:
```gradle
task installGitHooks(type: Copy) {
    from new File(rootProject.RootDir, 'pre-commit')
    into { new File(rootProject.RootDir, '.git/hooks')}
}
```
