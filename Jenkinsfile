node{
   stage('SCM Checkout'){
     git 'https://github.com/psboyane/myapp'
   }
   stage('Compile-Package'){
      //get maven home path
    def mvnHome = tool name: 'M3', type: 'maven'
      sh "${mvnHome}/bin/mvn package" 
   }
   stage('Email Notification')
   {
      mail bcc: '', body: '''Your last build is successful!!!!
      Thanks.''', cc: '', from: '', replyTo: '', subject: 'Jenkins_Job', to: 'prachiboyane10@gmail.com'
   }
   
   
}
