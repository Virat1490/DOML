pipeline {
agent any

stages {
stage('Clone') {
steps {
git 'https://github.com/Virat1490/DOML.git'
}
}

stage('Install') {
steps {
bat 'pip install -r requirements.txt'
}
}

stage('Train') {
steps {
bat 'python train.py'
}
}

stage('Test') {
steps {
bat 'python test.py'
}
}

stage('Deploy') {
steps {
bat 'python app.py'
}
}
}
}
