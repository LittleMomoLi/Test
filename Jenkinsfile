pipeline{
    agent{label 'cm-cent7x64-p4'}
    string(name:'')
    }
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
            mail bcc: '', body: 'Hi Pipeline!!!', cc: '', from: '1336580344@qq.com', replyTo: '', subject: 'PipelineTest', to: 'v-lmengn@microsoft.com'
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
  }

