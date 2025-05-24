pipeline {
    agent any

    stages {
        stage('Mailtrap Email Test') {
            steps {
                emailext (
                    to: 'test@example.com',  // Any email; Mailtrap will intercept it
                    subject: '✅ Jenkins-Mailtrap Email Test',
                    body: '''Hello Mitali,

This is a test email sent from Jenkins using Mailtrap SMTP.

If you are reading this in your Mailtrap inbox, then everything is working correctly. 🎉

Regards,
Jenkins CI''',
                    mimeType: 'text/plain'
                )
            }
        }
    }
}
