pipeline{
    agent{label 'cm-cent7x64-p4'}
    stages{
        stage('build'){
            steps{
                sh 'gcc -o add Add.c'
            }
        }
        stage('delivery'){
            steps{
            mail bcc: '', body: 'Hi Pipeline!!!', cc: '', from: '1336580344@qq.com', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com'
            }
        }
    }
        post{
            success{
                script{
                    mail bcc: '', body: 'success!', cc: '', from: '1336580344@qq.com', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com' 
                }
            }
        }
  }

