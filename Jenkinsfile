 node {
  stage 'Build and Test'
    git 'https://github.com/jober64/Liberty.git'
    env.PATH = "${tool 'Maven 3'}/bin:${env.PATH}"
    sh 'mvn -f Hello/pom.xml clean package'

  stage 'Deploy'
    sh 'cp Hello/target/*.war /opt/app/wlp/usr/servers/defaultServer/dropins/'
 }