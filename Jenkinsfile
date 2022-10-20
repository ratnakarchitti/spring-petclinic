pipeline{
    agent { label 'Jenkins' }
    triggers { 
        cron ('* * * * *')

    }
    stages {
        satge ('vcs') {
            steps {
                git url: 'https://github.com/ratnakarchitti/spring-petclinic.git',
                branch : 'devops'

            }
        }
        

    }
}