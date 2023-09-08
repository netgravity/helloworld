pipeline {
    agent any 
    parameters {
      string defaultValue: 'sunny', description: 'who to say hello!', name: 'PERSON', trim: true
      string defaultValue: 'version/X.X.X', description: 'xxx', name: 'RELEASE_BRANCH', trim: true
      string description: 'xxx', name: 'INPUT_RELEASE_VERSION', trim: true
      string description: 'xxx', name: 'NEXT_SNAPSHOT_BUILD_NUMBER', trim: true
      
    }

    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!'
                echo "Hello ${params.PERSON}"
                echo "Hello Branch version ${params.RELEASE_BRANCH}"
                echo "Hello input release version ${params.INPUT_RELEASE_VERSION}"
                echo "Hello input release version ${params.NEXT_SNAPSHOT_BUILD_NUMBER}"
                
            }
        }
    }
}
