pipeline {

    agent any

    stages 
    {
        // Get current branch
        stage('Verify git branch') 
        {
            steps {
            echo "$GIT_BRANCH"
            }
        }
    }
    // clean up the workspace
    post
    {
        always
        {
            sh "echo 'GoodBye the pipeline run successfully'"
            deleteDir()
        }
    }
}
