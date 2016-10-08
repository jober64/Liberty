 node ('linux'){
  stage 'Build and Test'
  env.PATH = "${tool 'Maven 3'}/bin:${env.PATH}"
  git 'https://github.com/jober64/Liberty.git'
  sh 'mvn clean package'
 }