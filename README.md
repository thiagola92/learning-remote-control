# Information
O objetivo é aprender a conectar em outra máquina.  

**Sistema operacional**: Ubuntu  

**Client**: Máquina que vai acessar outra  
**Server**: Máquina que vai ser acessada  

**Descobrir o IP Local**: `ip addr show`  
**Descobrir o IP Público**: Pesquise "IP" no Google  

# Rede Pública
Para que um client fora da sua rede local se conecte ao seu server, é preciso fazer um redirecionamento no seu roteador.  

[Configurando o MEU roteador](/public/README.md)

# Command-line Interface
* [SSH](ssh/README.md)

# Graphical Interface
* [VNC](vnc/README.md)
  * VNC é um protocolo simples
    * É como se tirasse um print da tela do server e transmitisse para o client.  
    * Os controles passados pelo client são processados no server como se fosse ele mesmo executando (mouse movendo, teclas do teclado, ...).  
* [RDP](rdp/README.md)
  * RDP é um protocolo complicado
    * Tem idéia do que são botões, fontes de texto e outras coisas gráficas básicas. Comprime essa informação antes de enviar pela rede e recria ela no client.  
      * VNC - transmite a imagem de um botão
      * RDP - transmite que existe um botão de largura *W* e altura *H*, na posição *X* e *Y*  
    * Funciona da mesma maneira como se um usuário tivesse logando na máquina.  
      * Por padrão apenas um usuário pode estar logado em uma conta ao mesmo tempo, por isso é preciso deslogar da conta para o client acessar.  
      * Por causa disso é possível que multiplas pessoas acessem usuários diferentes na mesma máquina.  