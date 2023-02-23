Cria usuário:
   - /usr/sbin/useradd -c "COMENTÁRIO" -d /home/xpto -s /bin/bash -p "senhaxpto" -g "grupo1" -G "grupo2" -m xpto;

#Deletar usuário
  - userdel -r xpto

Adicionar grupos:
	- groupadd -g 60021 xpto
	- groupadd -g 2000 xpto

Visualizar os grupos
  - less /etc/group

Remover usuário do grupo
 - gpasswd -d xpto  wheel
  

Novo password do usuário:
 - O root pode trocar a senha do usuário:
   - passwd xpto

Lock password para o usuário:
  - passwd -l xpto

Unloking password para o usuário:
  -  passwd -u xpto
