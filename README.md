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

## MKDIR

Comando usado para criar diretório/subdiretório. Evite o uso de espaços, acentos e caracteres especiais
```cmd
C:\>mkdir pasta_pai && cd pasta_pai
C:\pasta_pai>mkdir pasta_filho && cd pasta_filho
C:\pasta_pai\pasta_filho>
```
**Nota:** O operador **&& *(AND)*** é usado para que o próximo comando só seja executado se o comando anterior tiver sido executado com sucesso (exit status igual a 0):<br/>Fonte: [Dherik](https://pt.stackoverflow.com/a/82457)

**Bonus:** Criando arquivos
Para gerar um arquivo de texto, monta a seguinte sequência de comandos:
```cmd
C:\>type NUL > arquivo.txt
```
- **type:** Exibi conteúdo de arquivo
- **NUL:** Oculta uma saída
- **Operador ">":** Operador de redirecionamento
O comando **echo** exibe mensagens ou ativa/desativa o recurso de eco de comando.
Se usado sem parâmetros, o eco exibirá a configuração de eco atual.
```cmd
C:\>echo Qualquer mensagem como exemplo
```
Gravar uma saída de texto em arquivo
```cmd
C:\>echo Texto simples para demonstração > arquivo.txt
```
Acrescentar uma saída de texto em arquivo
```cmd
C:\>echo Texto simples para demonstração >> arquivo.txt
```
Para acrescentar o texto foi utilizado o operador de redirecionamento **">>"**<br/>
**Nota:** Para visualizar o conteúdo do arquivo baste usar o comando type:
```cmd
C:\>type arquivo.txt
```
## CD
Permite a navegação entre diretórios, da pasta pai para subpasta filho.
```cmd
C:\pasta_pai> cd pasta_filho
C:\pasta_pai\pasta_filho>
```
Sequência usada para retornar ao diretório anterior, ou pasta pai.
```cmd
C:\pasta_pai\pasta_filho>cd ..
C:\pasta_pai\>
```
Para retornar ao diretório raiz, o mais alto em uma hierarquia
```cmd
C:\pasta_pai\pasta_filho>cd \
C:\
```
**Nota:** Tente sempre que possível usar a tecla ***TAB*** para preencher automaticamente o que está sendo digitado. Usando esta prática você ganha agilidade para a navegação.




