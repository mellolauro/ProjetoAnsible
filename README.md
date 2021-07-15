# ProjetoAnsible
Criando Estrutura Linux com terraform (Azure) e Implantando WordPress com Ansible

Criando Estrutura Linux com terraform

Alterar os arquivos (terraform.tfvars, e o main.tf) computer_name = "VNET-02" e admin_username = "admintftec"

Utilizar os comandos

terraform fmt
terraform init
terraform validate 
terraform plan -out ftplan
terraform apply ftplan

Com a criação da estrutura o seu arquivo terraform.tfstate trará a chave publica para configurar o acesso para a utilização do Ansible.

Ansible

arquivo - 000-defaut.conf (arquivo de configuração do apache.)
https://gist.github.com/tjtoml/942d696c868b22a25259

Arquivo generatepress (Thema(template do WordPress - dashborad))
https://generatepress.com/category/development/

Criação da estrutura Ansible
Comandos 
ansible-playbook -i hosts provisionar.yml -u ubuntu --private-key ~/.ssh (seria a forma de como se conectar no servidor)
