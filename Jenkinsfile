pipeline {
    agent {
  label {
    label 'rhel'
    retries 3
  }
}
    stages {
        stage('Test') {
            steps {
                echo 'OS Info'
                sh 'usage.sh'
                ''' sh 'scp usage.sh sp@192.168.60.135:/tmp/' '''
                ''' sh 'ssh sp@192.168.60.135 'sh /tmp/usage.sh ' '''
            }
        }
    }
}
