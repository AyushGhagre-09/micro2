node
{
    stage("Hello")
    {
     echo "hello from jenkins file"
    }

     // For the 'fix' branch
    if (env.BRANCH_NAME.startsWith("fix-")) {
        stage('for the fix branch') {
            // Commands specific to the 'fix' branch go here
        echo "branch name : ${env.BRANCH_NAME}"
          
        }
    }
     if (env.BRANCH_NAME.startsWith("PR-")) {
        stage('for the PR') {
            // Commands specific to PRs go here
            echo "this only runs for the PRs: ${env.BRANCH_NAME.startsWith("PR-")}"
        }
    }
    
}
