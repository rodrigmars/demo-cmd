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
**Nota:📌** O operador **&& *(AND)*** é usado para que o próximo comando só seja executado se o comando anterior tiver sido executado com sucesso (exit status igual a 0):<br/>Fonte: [Dherik](https://pt.stackoverflow.com/a/82457)

**Bonus:✨** Criando arquivos
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
C:\>echo Sempre foi mais fácil destruir do que criar.(Spock)
```
Gravar uma saída de texto em arquivo
```cmd
C:\>echo A lógica é apenas o princípio da sabedoria, e não o seu fim.(Spock) > arquivo.txt
```
Acrescentar uma saída de texto em arquivo
```cmd
C:\pasta_pai\pasta_filho>echo A vida é como um jardim.(Spock) >> arquivo.txt
```
Para acrescentar o texto foi utilizado o operador de redirecionamento **">>"**<br/>
**Nota:📌** Para visualizar o conteúdo do arquivo baste usar o comando type:
```cmd
C:\pasta_pai\pasta_filho>type arquivo.txt
```
## CD
Permite a navegação entre diretórios, da pasta pai para subpasta filho.
```cmd
C:\pasta_pai\pasta_filho>cd \
C:\>cd pasta_pai
C:\pasta_pai>cd pasta_filho
C:\pasta_pai\pasta_filho>cd \
C:\>
C:\>cd pasta_pai\pasta_filho
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
**Nota:📌** Tente sempre que possível usar a tecla ***TAB*** para preencher automaticamente o que está sendo digitado. Usando esta prática você ganha agilidade para a navegação.

## REN 
O comando **ren** quando lançado renomeia arquivos ou diretórios.<br/>
Renomeando uma 📂:
```cmd
C:\pasta_pai\ren pasta_filho pasta_filho_2
C:\pasta_pai>cd pasta_filho_2
C:\pasta_pai\pasta_filho_2>
```
Renomeando um arquivo:
```cmd
c:\pasta_pai\pasta_filho_2>ren teste_1.txt teste_2.txt
```
## MOVE
Move um ou mais arquivos de uma 📁 para outra.
```cmd
C:\pasta_pai>move arquivo.txt pasta_filho
Overwrite C:\pasta_pai\pasta_filho_2\arquivo.txt? (Yes/No/All): Y
        1 file(s) moved.
```
## RMDIR 🗑️
Comando usado para excluir 📁
```cmd
C:\>rmdir /s pasta_pai
```
**Nota:📌** Emitindo o Parâmetro **/s** é possível excluir o diretório e seus subdiretórios, incluindo todos os arquivos.

