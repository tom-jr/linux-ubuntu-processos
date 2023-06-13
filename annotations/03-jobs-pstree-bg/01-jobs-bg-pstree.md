
**pstree** lista todos os processos do sistema em uma gráfico de tree
~~~ bash
pstree
~~~

'control+z' para o processo que esta rodando no bash atualmente
o comando **jobs** lista os comando parados do sistema
~~~ bash
jobs
~~~

o comando **bg+n**, onde n é o numero do item listado comando job permite que o processo volte a ser executado em background no 
bash, assim mantendo o bash livre para outros comandos. Apos rodarmos novamente o programa em bg o comando jobs lista o processo com
o status de *running*
~~~ bash
bg + [n]
~~~

o Comando **fg** trás o programa que esta rodando em bg para rodar no bash. Com o comando 'contro+c' paramos definitivamente o 
processo 
~~~ bash
fg [n]
~~~

quando executamos o programa com o '&' estamos informando ao sistema que é para rodar o processo em background direto
~~~ bash
[program_name] &
~~~