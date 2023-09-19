Instalação do NODE

1-Abra o Terminal do seu Linux com o comando ctrl + alt + t

2-Digite e aguarde: sudo apt install python3-pip

3-Digite e aguarde: pip3 install --user nodeenv

4-Teste a instalação do nodeenv digitando: nodeenv --version

!!!:Caso não funcione o comando ‘nodeenv’ precisará ser ativado.

-Digite no terminal: source ~/.profile ou reinicie a maquina virtual

5-Abra um terminal, selecione a pasta onde ficará a pasta que irá
conter o NodeJs. Digite: nodeenv nodejs-env

- "nodejs-env" é o nome da pasta nesse caso, mas você pode mudar
  
6-Digite: source nodejs-env/bin/activate (substituindo o nome nodejs-env pelo nome da sua pasta, pois o nome pode não ser o mesmo do citado no código)

7-Para testarmos iremos instalar o Node-Red, digite: npm install -g node-red

8-Ative o Node-red, digite: node-red

9-No computador host digite no navegador: http://localhost:1880

Após a instalação:

1-Abra o Terminal do seu Linux com o comando ctrl + alt + t

2-Abra a pasta onde está o seu node-js com o comando: cd "substitua p/ pasta onde está o seu node-js"/src e digite o comando: sudo nano index.js

3-Copie o codigo que está no arquivo .zip disponivel no repositório e cole no arquivo index.js que foi aberto no nano do terminal.

4-Use o atalho de teclado ctrl + O e de Enter, depois ctrl + X

5-Digite: sudo chown "seu nome de usuário":"nome do grupo" index.js. Exemplo: sudo chown pedro:pedro index.js

6-Digite: cd ~

7-Digite: source nodejs-env/bin/activate (substituindo o nome nodejs-env pelo nome da sua pasta, pois o nome pode não ser o mesmo do citado no código)

8-Digite: node index.js ou node "caminho da sua pasta"/index.js Exemplo: node nodejs-env/src/index.js

9-Agora é só escrever no seu navegador (chrome, mozilla, edge) localhost:"porta configurada no arquivo index.js" no caso a porta configurada neste repositório é a 8012. Fica assim: localhost:8012

10-Para desativar digite: deactivate_node
