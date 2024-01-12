pipeline {
    agent any
    stages {
        stage('Hazırlık') {
            steps {
                echo 'Proje hazırlığı yapılıyor...'
            }
        }
        stage('Derleme') {
            steps {
                echo 'Projeyi derleme işlemi yapılıyor...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testler çalıştırılıyor...'
            }
        }
        stage('Dağıtım') {
            steps {
                echo 'Uygulama dağıtılıyor...'
            }
        }
    }
    post {
        success {
            echo 'Başarıyla tamamlandı. Yeni sürüm dağıtıldı!'
        }
        failure {
            echo 'Hata oluştu. Lütfen sorunu kontrol edin.'
        }
        always {
            echo 'Jenkins Pipeline tamamlandı.'
        }
    }
}
