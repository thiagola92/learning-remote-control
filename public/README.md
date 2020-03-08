## Pré-requisito
* Descubra seu **IP na rede local** e **MAC address**
  * ![configurações do ubuntu](config.png)
  * ![mac e ipv4 ou ipv6](ipmac.png)
* Porta da aplicação
  * Procure no google para descobrir a porta da aplicação
    * **SSH**: 22  
    * **VNC**: 5900  

## Configurar Roteador
* Logue na conta admin do seu roteador  
  * A conta admin pode ser uma padrão da máquina  
    * **Mude a senha se for o caso, é muito perigoso deixar a senha padrão**
  * A conta admin pode estar escrita em algum lugar do seu roteador (olhe embaixo dele)  
  * Sua operadora pode ter lhe passado em algum lugar a conta admin e senha  
  * ![logando](login.png)  
* Vá na tab **Advanced**  
  * ![tab avançado](avancado.png)  
* Selecione **Forwarding**
  * ![Forwarding](forwarding.png)
* Selecionoe **Create IPv4** ou **Create IPv6**
  * Só lembre de usar o IP relacionado a opção criada
* Preencha as informações
  * **Local IP**: IP da sua máquina na rede local
  * **Local Start Port**: Porta utilizada pela aplicação
  * **Local End Port**: Mesma porta da "Local Start Port"
  * **External IP**: 0.0.0.0
  * **External Start Port**: Mesma porta da "Local Start Port"
  * **External End Port**: Mesma porta da "Local Start Port"
  * **Protocol**: TCP
  * **Enabled**: On
* Clique em **Apply**
* Selecione **Port Triggers**
  * ![Ports](ports.png)  
* Selecione **Create**
* Preencha as informações
  * **Trigger Start Port**: Porta utilizada pela aplicação
  * **Trigger End Port**: Mesma porta da "Trigger Start Port"
  * **Target Start Port**: Mesma porta da "Trigger Start Port"
  * **Target End Port**: Mesma porta da "Trigger Start Port"
  * **Protocol**: TCP
  * **Enabled**: On
* Clqiue em **Apply**


