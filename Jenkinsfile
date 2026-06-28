pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                git branch: 'main'
              https://github.com/mohan62447/petclinic-devops.git  
            }
        }
        stage ('Build') {
        steps {
            sh 'mvn clean package'
        }
    }
    stage ('code quality analysis'){
        steps {
            sh 'mvn sonar:sonar'
        }
    }

    }
}