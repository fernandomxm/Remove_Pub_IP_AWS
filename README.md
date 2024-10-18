Como melhor prática de segurança, é necessário que não se utilize IPs públicos diretamente nas instâncias EC2.

Segue abaixo, qual a forma mais simples de se retirar o IP Público sem precisar parar a instância:

1) Alocar Elastic IP e associá-lo a instância que quer remover IP público

2) Cria interface de rede temporária na mesma subnet e região da instância que quer remover IP público

3) Associar interface de rede temporária a instância que quer remover IP público

4) Desassociar Elastic IP criado no passo 1 a instância que quer remover IP público

5) Dessassociar interface de rede temporária a instância que quer remover IP público

6) Deletar Elastic IP e interface de rede temporária criados

https://youtu.be/EL-_ipaE4W4
