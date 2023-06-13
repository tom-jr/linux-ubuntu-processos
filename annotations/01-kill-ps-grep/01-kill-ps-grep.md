# Processos
Cada processo que invocamos esta sendo executado pelo CPU

**ps** lista os processos que estão sendo executados no bash atual
~~~ bash
ps
~~~

*-e* lista todos os processos no CPU
~~~ bash
ps -e
~~~
o output é renderizado com o id do processo 

[19004 ?        00:00:00 msedge]

*-f* informa mais colunas no out put
~~~ bash
ps -ef
~~~
    UID          PID    PPID  C STIME TTY          TIME CMD
    root           1       0  0 03:54 ?        00:00:02 /sbin/init splash


Usamos o character '|' para redirecionar o output para outro programa, no caso o grep, que do output filtra os processos informado
com arg, no caso o chrome.
Poderíamos pegar um arquivo txt e redirecionar a Saida do cat para o grep e informar um param, que apenas as linhas com aquele para ia ser retornado no output do grep
~~~ bash
ps -e | grep chrome
~~~




**kill** mata o processo com o id informado
~~~ bash
kill [number_process]
~~~

*-9* mata o processo como um force
~~~ bash
kill -9 [process]
~~~

