node
{
stage "1. Create Build Output"
sh "mkdir -p output"
writeFile file:"output/usefulfile.txt",text:"This is a useful file."
writeFile file:"output/uselessfile.md",text:"This is a useless file."
writeFile file:"output/git.html",text:"This is a useless file from git repository."
stage "2. Archive Build Output"
archiveArtifacts artifacts:"output/*.txt",excludes:"output/*.md"
stage "3. Build the code"
echo "Building the code from SCM"
stage "4. Another step"
sh "touch another.html"
stage "4. Another step"
sh "touch another_git_repo.html"
}
