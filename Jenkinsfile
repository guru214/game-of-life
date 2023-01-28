pipeline {
    agent any
    stages{
        stage('test') {
            steps {
                sh 'echo hello'
            }
        }
        stage('learning') {
            agent {'JDK11MVN'}
            steps {
                git url:'https://github.com/muthyalasaikiran/game-of-life.git',
                    branch: 'master'
            }
        }
    }
}