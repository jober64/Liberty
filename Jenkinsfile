 node {
  stage 'Build and Test'
    git 'https://github.com/jober64/Liberty.git'
    env.PATH = "${tool 'Maven 3'}/bin:${env.PATH}"
    sh 'mvn clean package'
  stage 'Deploy'

 }