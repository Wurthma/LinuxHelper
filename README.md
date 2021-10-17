#Linux Helper

## Comandos básicos - terminal linux

`man` -> comando para receber ajuda (exemplo: man pwd)

`pwd` -> verificar diretório atual

- `ls` -> listar diretórios e arquivos
- `ls -l` -> listar diretórios e arquivos com mais detalhes
- `ls -la` -> inclui arquivos/diretórios ocultos

- `echo "Olá, mundo!" > myfile.txt` -> Criar arquivo myfile.txt com o contéudo "Olá, mundo!"
- `echo "Adicionando mais conteúdo..." >> myfile.txt` -> Duas setas (>>) indica que estamos incluindo mais conteúdo ao mesmo arquivo

- `cat myfile.txt` -> Exibi o conteúdo do arquivo myfile.txt

- `head myfile.txt` -> Exibi as 10 primeiras linhas do arquivo
- `head -n 3  myfile.txt` -> Exibi as 3 primeiras linhas do arquivo

- `tail myfile.txt` -> Exibi as 10 ultimas linhas do arquivo
- `tail -n 3  myfile.txt` -> Exibi as 3 ultimas linhas do arquivo

- `cd myfolder` -> Acessar a pasta especificada

- `mkdir myfolder` -> cria a pasta especificada

- `rm myfile.txt` -> remove o arquivo especificado
- `rm -r myfolder` -> remove recursivamente todos arquivos do diretório

- `rmdir myfolder` -> remove o diretório especificado se o mesmo estiver vazio

- `cp myfile1.txt myfile2.txt` -> copiar o conteúdo do "myfile1.txt" para "myfile2.txt"
- `cp -r myfolder1 myfolder2` -> copiar recursivamente o conteúdo da pasta "myfolder1" para "myfolder2"

- `mv myfile1.txt renamedfile.txt` -> renomeia/move o arquivo "myfile1.txt" para "renamedfile.txt"
- `mv myfile1.txt myfolder` -> move o arquivo "myfile1.txt" para a pata "myfolder"
- `mv myfile1.txt myfolder myfilerenamed.txt` -> move o arquivo "myfile1.txt" para a pata "myfolder" com um novo nome

## Compactando e descompactando

- `tar -cz myfolder myfile.tar.gz`  -> compacta o conteúdo da pasta myfolder recursivamente no arquivo myfile.tar.gz
- `tar -xz < myfile.tar.gz` -> descompactar o conteúdo do arquivo myfile.tar.gz para a pasta atual
- `tar -czf myfile.tar.gz myfolder` -> descompactar o conteúdo do arquivo myfile.tar.gz para a pasta myfolder
- `tar -xzf myfile.tar.gz` -> descompactar o conteúdo do arquivo myfile.tar.gz para a pasta atual

## Podemos também utilizar o ZIP no linux

- `zip -r mycompatedfiles.zip myfolder/` -> compacta o conteúdo da pasta myfolder recursivamente
- `unzip -l mycompatedfiles.zip` -> mostra o conteúdo do arquivo zip
- `unzip mycompatedfiles.zip` -> descompacta o conteúdo do arquivo zip

## Editor VI

- **"i"** mudar do modo navegação para inserção/edição
- **"ESC"** para voltar ao modo de navegação
- **":w"** para salvar o arquivo
- **"x"** para remover caracteres
- **"11x"** para remover 11 caracteres
- **"dd"** remover a linha
- **":q"** para sair do VI
- **":wq"** para salvar e sair do VI
- **":q!"** para sair e ignorar alterações do VI
- **"1G"** vai pra primeira linha
- **"10G"** vai pra linha 10
- **"G"** vai pra ultima linha
- **"0"** inicio da linha
- **"$"** final da linha
- **"/programador"** localizar a palavra "programador" (use "n" para localizar próximas ocorrências e "N" para anterior)
- **"yy"** copiar linha
- **"3yy"** copiar 3 linhas
- **"p"** colar linha
