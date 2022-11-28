pipeline {
agent {
label {
		label "built-in"
		customWorkspace "/var/onkar"
		
		}
		}
    stages
    {
        stage(clone)
        {
            steps
            {
                sh "sudo rm -rf *"
                sh "sleep 5"
                sh "sudo git clone https://github.com/Onkar-Borwar/myportfolio.git"
                
            }
        }
        stage(copy)
        {
            steps
            {
                sh "sudo chmod -R 755 /var/www/html"
                sh "sleep 5"
                sh "sudo cp -R /var/onkar/myportfolio/* /var/www/html"
            }
        }
        
    }
}
