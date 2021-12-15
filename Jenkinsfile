pipeline{
    agent any
    stage('Checkout') {
         steps {
             echo ">>>>>>>> Checkout branch ${params.BRANCH}"
         }
     }
    stage('Install') {
         when {
             expression {
                 return params.INSTALL
             }
         }
         steps {
             echo ">>>>>>>> Install ${params.INSTALL}..."
             sh "cd ${WORKSPACE}"
         }
    }
}