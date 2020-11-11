# Python

### Ambiente virtual

Quando estamos desenvolvendo alguma aplicação em python podemos acabar necessitando utilizar alguma biblioteca para utilizamos no nosso código. Essas bibliotecas são instaladas utilizando um gerenciador de bibliotecas do Python chamado "pip". Quando utilizamos o gerenciador de bibliotecas para instalar alguma biblioteca, a mesma será instalada no ambiente global do sistema operacional. Com o tempo podemos acabar instalando diversas bibliotecas que foram instaladas para utilizar em diferentes projetos. Isso além de deixar diversas bibliotecas instaladas que futuramente não serão utilizadas mais, também pode causar problemas. 

Sendo assim nós podemos criar ambientes virtuais, de forma que as bibliotecas são instaladas nestes ambientes virtuais e não no ambiente global. Trazendo mais organização e também evita problemas. Cada ambiente virtual possui seus próprios diretórios de instalação que não são acessíveis ou compartilhados entre os demais ambientes virtuais.

Para issto existe o Virtualenv, uma biblioteca em python para criar ambientes virtuais. Podemos isntalar a partir do próprio gerenciador de bibliotecas do python:

```
$ sudo pip install virtualenv
```

Uma vez instalado, para criar um ambiente virtual:

```
$ virtualenv <nome>
```

Será criado um diretório com  o `nome` informado no comando acima no diretório onde o comando foi executado. Com o ambiente virtual criado, devemos ativá-lo para que todos os comandos de instalação de bibliotecas sejam instaladas somente neste ambiente virtual:

```
$ source /<nome>/bin/activate
```

Onde `nome` é o nome do ambiente virtual escolhido no comando da criação. Após a execução do comando nosso terminal sinalizará que nosso ambiente virtual está ativado e que todos os comandos irão rodar apenas nele.

Caso seja necessário utilizar dentro do ambiente virtual uma versão diferente do python, utilizar o comando abaixo na criação do ambiente virtual:

```
$ virtualenv --python=/path/to/python <nome>
```

 ### Exemplos
   - [Aplicação de linha de comando](/pontopy)
