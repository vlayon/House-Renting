pipeline{
    agent any
    
    stages{
        stage("Restore project"){
            steps{
                bar "dotnet restore"
            }
        }
        stage("Build project"){
            steps{
                bar "dotnet build --no-restore"
            }
        }
        stage("Run tests"){
            steps{
                bar "dotnet test --no-build --verbosity normal"
            }
        }
    }    
}