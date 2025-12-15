pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "Without docker"
                    ls -la
                    touch container-no.txt
                    ls -al
                '''
            }
        }
        stage("Test") {
            steps {
                echo "This is Test Stage"
		sh "test -f build/index.html"

            }
        }
    }
}
