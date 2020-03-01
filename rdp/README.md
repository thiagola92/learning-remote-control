# Client
* Instalar Remmina
  * Vem instalado no Ubuntu normal, mas não na instalação mínima  
  * `sudo snap install remmina`  
* Abrir Remmina
* Criar nova conexão
  * ![Botão de criar nova conexão](remmina_01.png)
* Selecionar o protocolo RDP    
  * ![Seleção do protocolo](remmina_02.png)  
  * ![Protocolo selecionado](remmina_03.png)  
* Inserir o IP  
  * ![Caixa de texto do IP](remmina_04.png)  
* Clicar no botão de conectar  
* Preencher com o login e senha de um usuário do computador  
  * O usuário **não** pode estar logado  
  * ![Entrar com login e senha do usuário do computador](remmina_05.png)

# Server
* Instalar Xrdp
  * `sudo apt install xrdp`  
* Verificar se está executando
  * `systemctl status xrdp`
  * Se não estiver
    * `systemctl start xrdp`  
    * Abrir automaticamente na inicialização do sistema
      * `systemctl enable xrdp`  

# Font
https://websiteforstudents.com/connect-to-ubuntu-16-04-17-10-18-04-desktop-via-remote-desktop-connection-rdp-with-xrdp/  