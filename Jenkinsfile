
pipeline{
    agent any
//     options {
//         buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
//         disableConcurrentBuilds()
//     }
    stages{
        stage("Hello"){
            steps{
                echo "hello chand!"
            }
        }
//         stage("for the fix branch"){
//             when{
//                 branch "fix-*"
//             }
//             steps {
//                 echo "Execute for fix branch"
//             }
//         }
        stage("for the PR"){
            when{
                branch 'PR-*'
            }
            
            steps {
                echo "this only runs for PRs"
            }
        }
    }
}
