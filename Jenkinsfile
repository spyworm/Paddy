node
{
stage "Create Build Output"
sh "mkdir -p output"
writeFile file:"output/usefulfile.txt",text:"This is a useful file."
writeFile file:"output/uselessfile.md",text:"This is a useless file."
stage "Archive Build Output"
archiveArtifacts artifacts:"output/*.txt",excludes:"output/*.md"
}
