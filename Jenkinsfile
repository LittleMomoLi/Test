Jenkinsfile (Scripted Pipeline)
/* Requires the Docker Pipeline plugin */
node('cm-cent7x64-p2') {
    checkout scm
    stage('Build') {
        docker.image('maven:3.3.3').inside {
            sh 'mvn --version'
        }
    }
}
