pipeline {
         agent any
         stages {
                 stage('Code sync') {
                 steps {
                     echo 'Stage : 1'
                 }
                 }
                 stage('Two') {
                 steps {
                    echo 'Stage : 2'
                 }
                 }
                 stage('Three') {
                 
                 steps {
                       echo "Stage : 3"
                 }
                 }
                 stage('Four') {
                 parallel { 
                            stage('Unit Test') {
                              steps {
                                echo "Running the unit test..."
                           }
                           }
                            stage('Integration test') {
                              steps {
                                echo "Running the integration test..."
                              }
                           }
                           }
                           }
              }
}