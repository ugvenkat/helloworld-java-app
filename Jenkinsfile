@Library('my-shared-library') _

pipeline {
    agent any
    stages{
        stage('Git Checkout'){
            steps {
                script{

                    gitCheckout(
                        branch: "main", 
                        url: "https://github.com/ugvenkat/helloworld-java-app.git"
                    )

                }
            } 
            
        }

        stage('Unit Test Maven'){
            steps {
                script{
                    mvnTest()
                }
            } 
            
        }

    }

}