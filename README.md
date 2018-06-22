# hdpdev


Obs: 
- privileged √© necess√°rio por causa do systemd
- Container foi instalado com o hostname horton.single.node
- Portas para exposi√√o 8080 = Ambari
  Colocar as demais portas se necess√rio


#Ex: Para iniciar o container
docker --name horton -d --privileged -h horton.single.node -p 8080:8080 horton

#Ex: Para executar comandos dentro do container
docker exec -it horton bash
