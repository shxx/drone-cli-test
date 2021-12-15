pipeline{
    agent any
    stages{
        stage("first stage"){
            stages{  // 嵌套在stage里
                stage("inside"){
                    steps{
                        echo "inside"
                    }
                }
            }
        }
        stage("stage2"){
            steps{
                echo "outside"
            }
        }
    }
}