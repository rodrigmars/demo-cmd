# Demo-mistificar cmd

## DIR

Exibe uma lista de arquivos e subdiretórios de um diretório
Lista todos os arquivos no diretório atual com extensões *.txt
```cmd
C:\> dir *.txt
```
Redireciona a saída do comando dir para um arquivo
```cmd
C:\> dir > arquivo.txt
```
>obs: Operador ">" usado para redirecionamento

## CD

Permite a navegação entre diretórios, da pasta pai para subpasta filho.
```cmd
C:\pasta_pai> cd pasta_filho
C:\pasta_pai\pasta_filho>
```
Sequência usada para retornar ao diretório anterior, ou pasta pai.
```cmd
C:\pasta_pai\pasta_filho> cd ..
C:\pasta_pai\>
```
Para retornar ao diretório raiz, o mais alto em uma hierarquia
```cmd
C:\pasta_pai\pasta_filho> cd \
C:\
```
>Obs: Tente sempre que possível usar a tecla TAB para preencher automaticamente o que está sendo digitado. Usando esta prática você ganha agilidade para acessar pastas, caminhos e comandos




