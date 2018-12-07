# URI.CS16.TrabalhoFinalRedesISistemasOperacionaisII
Repositório criado para fornecer um local que centralize todas as informações, códigos e tecnologias utilizadas no trabalho final das disciplinas de Redes I e Sistemas Operacionais II do curso de Ciência de Computação - URI Erechim (2018).

**Para uma réplica completa deste projeto, visualize o arquivo *.pdf* em anexo**

## Aplicação
Esta aplicação é um simples _avaliador_ de códigos. Essa simulação foi criada apenas para servir como motivo de implementação da tecnologia do https://docs.gluster.org/en/latest/ , um software que cria um sistema de arquivos distribuído. Para que esse projeto simulasse um ambiente real, este projeto divide-se em três partes:

### Parte _Frontend_ (Web)
É a parte visual do projeto. Este sistema, criado utilizando o https://www.urionlinejudge.com.br/judge/en/login como base, permite que se crie trechos de códigos para resolver problemas simples de lógica de programação. Existem **três linguagens** de programações disponíveis para serem usadas neste projeto: *C++*; *Python* e *Java*.

> Encontre o código desta aplicação em: https://github.com/joao-vieira/URI.CS16.SimpleJudgeSystem

### Parte _Backend_ (Compilador)
É o backend do projeto em questão, ele é responsável por buscar todos os arquivos que foram criados pelo frontend web, inicialmente localizado no banco de dados e depois na pasta local da máquina. Posteriormente a leitura e compilação do arquivo, o backend envia a resposta para o banco de dados.

> Encontre o código desta aplicação em: https://github.com/viniciusandd/compilador-multilinguagens

### Parte _Gluster_ (Servidor)
O servidor liga as duas partes apresentadas anteriormente, pois utiliza do gluster para criar um sistema de arquivos compartilhados entre as máquinas, replicando e sincronizando os arquivos criados em uma máquina, assim, estes arquivos serão criados nas outras que possuem o volume do gluster. O servidor possui um banco de dados para utilização como fila de processamento das entradas do _avaliador_.

## Observação
Este repositório é apenas um redirecionador para que, caso alguém se interessar pelo assunto e mais especificamente por esse projeto, tenha disponíveis os caminhos e locais onde podem ser encontrados os códigos fontes e manuais desta aplicação.
