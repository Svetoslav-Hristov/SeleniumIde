pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Restore Dependencies"){
            steps{
                bat "dotnet restore"
            }
            
        }
        stage("Build code"){
            steps{
                bat "dotnet build"
            }
        }
        stage("Run Tests"){
            steps{
                bat "dotnet test"
            }
        }
    }
   
}