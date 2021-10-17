# Comandos avançados

- `ps` -> verifica os processos em execução do bash atual
- `ps -e` -> todos processos do sistema
- `ps -ef` -> todos processos do sistema com mais detalhes
- `ps -ef | grep firefox` -> filtra apenas os processos que contem firefox

- `kill 16218` -> mata o processo de id 16218
- `kill -9 16218` -> mata o processo sem aguardar retorno
- `killall firefox` -> mata todos processos firefox

- `top` -> mostra situação da CPU e memória

- `pstree` -> mostra os processos em arvore

- `firefox` -> abrir o firefox no bash atual
- **"CTRL + Z"** -> pausar o processo aberto no bash
- `jobs` -> verifica os processos do bash atual
- `bg 1` -> joga para processamento background o job 1 do bash atual
- `fg 1` -> volta o job 1 para foreground
- `gedit &` -> abrir o editor gedit direto em background

- `sh myscript` -> executa um scrip com comandos shell

## CHMOD

- `chmod +rwx myfile` -> adiciona permissões de leitura, escrita e execução ao arquivo "myfile"
- `chmod +x myfile` -> adiciona permissão de execução ao arquivo "myfile"
- `chmod -x myfile` -> remove permissão de execução ao arquivo "myfile"
- `chmod o-rx myfile` -> remove permissão de leitura e execução de "outros" ao arquivo "myfile"

----------------------------------------------------

- `locate firefox` -> localiza o diretório do programa firefox
- `wich firefox` -> qual arquivo será executado se chamar "firefox"
- `sudo` -> executar como usuário root
- `sudo updatedb` -> atualiza o DB do linux
- `passwd` -> mudar senha do usuário atual
- `sudo` passwd -> mudar senha do usuário root
- `su root` -> fazer login com o usuário "root"
- `su george` -> fazer login com o usuário "george"
- `adduser` -> adiciona um novo usuário ao linux

- `env` -> exibir as variáveis de ambiente
- `gedit .bashrc` -> Editar arquivos com variáveis de ambiente do bash
- `PATH=$PATH:/home/george/workspace` -> adiciona o diretório ao PATH do SO
	
## apt

- `apt-get update` -> atualiza programas instalados
- `apt-cache search ftp` -> procura aplicativos sobre ftp
- `apt-get install vsftpd` -> instala o aplicativo vsftpd
- `apt-get remove vsftpd` -> remove o aplicativo vsftpd

- `dpkg -i my_application.deb` -> instala uma aplicação .deb (ubunto/debian) que está no diretório atual
- `dpkg -r my_application` -> remove uma aplicação

----------------------------------------------------

- `service vsftpd stop` -> parar o serviço vsftpd
- `service vsftpd start` -> iniciar o serviço vsftpd (/etc/init.d <- contem os serviços que serão inicializados com a máquina)

## SSH

- `apt-get install ssh` -> instala o ssh client e server no linux
- `ssh george@myhost` -> faz acesso remoto com usuário george na máquina "myhost"
- `ssh -X george@myhost` -> faz acesso remoto com odo gráfico (-X)
- `scp myfile.zip george@myhost:~/` -> copia para o home do usuário acessado o arquivo myfile.zip
- `scp -r myfolder george@myhost:~/` -> copia para o home do usuário acessado a pasta myfolder de forma recursiva
