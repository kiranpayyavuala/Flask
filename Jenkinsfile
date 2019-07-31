 node{
   stage('SCM Checkout'){
     git 'https://github.com/kiranpayyavuala/Flask.git'
   }
   stage('Build Docker Image')
   {
   sh 'docker build -t kiranpayyavuala/flask:1.0 .'
 }
 stage('Push Docker Image')
 {
   sh "docker login -u dockehunusername -p ourdockerhubpassword"
   sh 'docker push kiranpayyavuala/myapp:1.0'
}
}
