# terraform-activity
Atividade de terraform

# Rodar na raíz do projeto para gerar chaves

ssh-keygen -t rsa -b 4096 -f my-aws-key

# Subir Terraform

terraoform init
terraform apply

# Configurar e subir servidor NGINX com Ansible

chmod 400 my-aws-key

ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i IP_AQUI, -u ubuntu --private-key my-aws-key ../ansible/playbook.yml

