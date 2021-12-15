
pipeline{
    agent any
    stages{
        stage("first stage"){
            steps("first steps"){
                echo "this is first step"
            }
        }
    }
    post{
        always{
            echo "this is ending..."
        }
    }
}