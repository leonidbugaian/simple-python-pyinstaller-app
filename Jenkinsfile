pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'python:2-alpine'
                }
            }
            steps {
                sh 'python -m py_compilr sources/add2vals.py sources/calc.py'
            }
        }
    }
}
