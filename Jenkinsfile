pipeline {
    agent any
    stages {
        stage('create file') {
            steps {
                 // FILE_NAME 변수 값이 이름인 파일을 생성, 내용은 OUTPUT_TEXT변수의 값
                 writeFile( file: "${FILE_NAME}.txt", text: "${OUTPUT_TEXT}")
                 sh 'ls -la'
                 echo 'I think it is one of the benefits when you use pipeline.'
                 sh "cat ${FILE_NAME}.txt"
            }
        }
    }
}
