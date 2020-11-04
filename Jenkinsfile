pipeline {
    agent any
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello')
    }
    stages {
        stage("Stage 1"){
            steps {
                sh 'echo "$params.Greeting World!"'
            }
        }
        stage("Stage 2"){
            steps {
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    '''
                }
        }
    }
}
