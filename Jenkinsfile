pipeline{
    agent (label 'springpetclinic')
    triggers { ('* * * * *')

    }
    stages {
        satge ('vcs') {
            steps {
                git url: 'https://github.com/ratnakarchitti/spring-petclinic.git'
            }
        }
        stage {
            steps ('build') {
                sh 'mvn package'
            }
        }

    }
}