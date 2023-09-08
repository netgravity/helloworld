pipeline {
    agent any 
    parameters {
      string defaultValue: 'sunny', description: 'who to say hello!', name: 'PERSON', trim: true
      string defaultValue: 'version/X.X.X', description: 'Branch to be released. Eg: develop or version/1.X or feature/jenkins_release_build', name: 'RELEASE_BRANCH', trim: true
      string description: 'Release version number to override the default. Eg: 1.2.3', name: 'INPUT_RELEASE_VERSION', trim: true
      string description: 'Next snapshot build number without -SNAPSHOT to override the default. Eg: 1.2.4', name: 'NEXT_SNAPSHOT_BUILD_NUMBER', trim: true
      
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
