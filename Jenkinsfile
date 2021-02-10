node('master') {
    echo "This is Executed from node"
stage('Checkout') {
    git credentialsId: 'GitHub_123', url: 'https://github.com/dhamodaranv/Devops-project.git'
 echo "Code Checout completed from Git"
}
stage('check condition') {
    when {
        expression {
            BRANCH_NAME == 'test' || BRANCH_NAME == 'master'
        }
    }
}
stage('Compile') {
    sh 'ls -ltr && $pwd'
}
}
