pipeline{
    agent (label 'JDK-11-MVN')
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