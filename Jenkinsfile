pipeline{
    agent{label 'cm-cent7x64-p4'}
    stages{
        stage('build'){
            steps{
                sh 'gcc -o add Add.c'
            }
        }
        stage('test'){
             steps{
                echo 'Test'
                }
        }
        stage('delivery'){
            steps{
            mail bcc: '', body: 'Hi Pipeline', cc: '', from: '', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com'
            }
        }
    }
  }

