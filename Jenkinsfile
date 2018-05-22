pipeline{
    agent{label 'cm-cent7x64-p4'}
        stage('test'){
             steps{
                echo 'Test'
                }
        }
        stage(
    stages{
        stage('build'){
            steps{
                sh 'gcc -o add Add.c'
            }
        }'delivery'){
            steps{
            mail bcc: '', body: 'Hi Pipeline!!!', cc: '', from: '1336580344@qq.com', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com'
            }
        }
    }
        post{
            success{
                script{
                    mail bcc: '', body: '${JOB_NAME}success', cc: '', from: '1336580344@qq.com', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com' 
                }
            }
        }
  }

