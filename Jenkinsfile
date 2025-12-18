pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch: "main", url: "https://github.com/devops-project-manisha/Petclinic.git"
            }
        }
        stage('build'){
            steps{
                sh "mvn clean package"
            }
        }
        stage('Test'){
            steps{
                sh "mvn clean test"
            }
        }
    }
}