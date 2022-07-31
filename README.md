# desafio-02-linux



### reto02

Deberás quitarle todos los permisos con el comando

chmod a-rwx archiv*


```sh
~/Downloads/desafio-02-linux/reto02 (develop*) » sudo chmod a-rwx archiv*                                                                                  
[sudo] password for osboxes: 

~/Downloads/desafio-02-linux/reto02 (develop*) » ls -la                                                                                                    
total 8
drwxrwxr-x 2 osboxes osboxes 4096 Jul 30 17:58 .
drwxrwxr-x 5 osboxes osboxes 4096 Jul 30 17:56 ..
---------- 1 osboxes osboxes    0 Jul 30 17:56 archiv1
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv2
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv3
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv4
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv5
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv6
---------- 1 osboxes osboxes    0 Jul 30 17:57 archiv7
---------- 1 osboxes osboxes    0 Jul 30 17:58 archiv8
---------- 1 osboxes osboxes    0 Jul 30 17:58 archiv9

```


```sh

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rwx,go= archiv1                                                                                   

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rw,go= archiv2                                                                                    

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod a=rwx archiv3                                                                                       

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rwx,g=rw,o=r archiv4                                                                              

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rwx,g=r,o= archiv5                                                                                

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rx,g=rw,o=r archiv6                                                                               

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=r,g=,o=x archiv7                                                                                 

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rw,g=r,o=r archiv8                                                                                

~/Downloads/desafio-02-linux/reto02 (develop*) » chmod u=rw,g=rw,o=r archiv9                                                                               

~/Downloads/desafio-02-linux/reto02 (develop*) » ls -la                                                                                                    
total 8
drwxrwxr-x 2 osboxes osboxes 4096 Jul 30 17:58 .
drwxrwxr-x 5 osboxes osboxes 4096 Jul 30 17:56 ..
-rwx------ 1 osboxes osboxes    0 Jul 30 17:56 archiv1
-rw------- 1 osboxes osboxes    0 Jul 30 17:57 archiv2
-rwxrwxrwx 1 osboxes osboxes    0 Jul 30 17:57 archiv3
-rwxrw-r-- 1 osboxes osboxes    0 Jul 30 17:57 archiv4
-rwxr----- 1 osboxes osboxes    0 Jul 30 17:57 archiv5
-r-xrw-r-- 1 osboxes osboxes    0 Jul 30 17:57 archiv6
-r-------x 1 osboxes osboxes    0 Jul 30 17:57 archiv7
-rw-r--r-- 1 osboxes osboxes    0 Jul 30 17:58 archiv8
-rw-rw-r-- 1 osboxes osboxes    0 Jul 30 17:58 archiv9
```