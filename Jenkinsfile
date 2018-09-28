node{
   stage('SCM Checkout'){
     git 'https://github.com/psboyane/myapp'
   }
   stage('Compile-Package'){
    sh 'mvn package' 
   }
}
