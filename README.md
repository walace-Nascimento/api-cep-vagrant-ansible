
# cenario-vagrant-ansibLe
=======
# cenario-vagrant-ansible
Tópicos

* [Descrição do Projeto](#descrição-do-projeto)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Demonstração da Aplicação](#passo-a-passo-da-aplicação)

# Descrição do Projeto
  Automatização de uma API-CEP dos Correios para verificação do CEP utilizando Vagrant e Ansible aplicada no serviço Nginx
 
# Tecnologias utilizadas
**Ansible**

**Vagrant**

**Nginx**

**VirtualBox**

# Passo-a-passo da aplicação

## Passo 1
  Instalar o vagrant na sua máquina e criar o vagrantfile com o comando:

```vagrant init ubuntu/focal64```

  As configurações editadas de acordo com a necesidade da aplicação estão descritas no vagrantfile, com a instalação automatizada do *Ansible* e do *Nginx*.

## Passo 2 
  Criação das roles ***files, tasks, handlers, vars*** todos arquivos declarados em YAML
  
  O arquivo Cep.html é uma API dos correios para consultar CEP

## Passo 3 
  Criação do playbook para que a role possa ser executada diversas vezes, automatizando a aplicação.
## Passo 4 
  Para executar a máquina virtual, basta digitar o comando:

``` vagrant up ```

  Com o processo de criação da máquina, acontece a instalação do **Nginx** e do **Ansible**

## Passo 5 
  Como foi escolhida no vagrantfile a opção "Public_Network", a aplicação pode ser testada com o seguinte caminho:

*SEUIP/Cep.html*
