# Protótipo: Smart Lamp	

## Esse protótipo foi desenvolvido pelo grupo <ins>Nexus</ins>, Formados por:

|Nome|RM|
|--|--|
|[Lucas de Almeida Pires](https://github.com/LucasAllPires) | RM: 562757 |
|[Daniel Oliveira de Souza](https://github.com/xdlimao) | RM: 566284 |
|[João Pedro Raimundo Marcilio](https://github.com/Jonausss) | RM: 561603 |
|[Lucas Zanella Clemente](https://github.com/LucasZanellaClemente) | RM: 563880 |
|[João Pedro Ribeiro Palermo](https://github.com/jpPalermo) | RM: 562077 |
|[Felipe Campos Vianna Peres](https://github.com/camp0s0s) | RM: 562752 |

## Índice

1. [Descrição](#descrição)
   
2. [Funcionalidades](#funcionalidades)
   
3. [Componentes Físicos](#componentes-físicos)
  
4. [Como usar](#como-usar)
   
5. [Links](#links-para-visualização)

---

### Descrição

O projeto <ins>Smart Lamp</ins> do grupo **Nexus** é  um protótipo de lâmpada inteligente que se conecta à internet. Utilizando um **ESP32**, o dispositivo é capaz de interagir com uma plataforma de backend para oferecer controle e monitoramento remoto.

O sistema possui um ***sensor de luz LDR*** que mede a claridade do ambiente. Esses dados são transmitidos em tempo real para a plataforma **FIWARE**, onde podem ser acessados e visualizados online. Além de enviar dados, o Smart Lamp também pode receber comandos. Através da plataforma, é possível ligar ou desligar seu LED remotamente, demonstrando uma comunicação bidirecional completa.

---

### Componentes físicos

| Componente | Quantidade |
|--|--|
|ESP32 DEVKIT V1|1|
|LDR|1|
|Jumpers|3|

<img width="300" height=auto alt="esquema_fisico" src="https://github.com/user-attachments/assets/386b4d9d-56b5-4640-bd52-10864b7461e3" />  

> Screenshot do projeto dentro do WokWi

---

### Funcionalidades

***Lampada e luminosidade (☀️)***

Mede a intensidade da luz no ambiente por meio de um sensor LDR, e disponibiliza um medimento no terminal de quão claro está. Com base nesse medimento, o projeto decidir se ele irá ligar a lampada ou mante-la desligada

---
### Como usar

- Logue na sua plataforma de nuvem (no tutorial sera feito no azure)
1. Acesse Máquina Virtual e vamos criar uma nova instância de uma VM
<img width="400" height="auto" alt="image" src="https://github.com/user-attachments/assets/322b49ab-335e-45da-909f-a2720bc15095" />


2. Vamos criar na opção simples.
<img width="400" height="auto" alt="image" src="https://github.com/user-attachments/assets/4c05dd7b-c1a5-47fe-8444-25a0533ec0fa" />


3. Durante a configuração (seleção de plano, região, nome) selecione um OS de distribuição Linux (Recomendado Debian ou Ubuntu)
<img width="700" height="auto" alt="image" src="https://github.com/user-attachments/assets/cc497b34-cdfe-4c65-9560-142b1f0f5b75" />


4. Selecione um modelo de VM que tenha no mínimo 1 cpu e 1GiB de memória de ram, e adicione memória interna até atingir no mínimo 20GB
<img width="700" height="auto" alt="image" src="https://github.com/user-attachments/assets/9f7105e6-f22e-4437-b423-20e022a19195" />


5. Configure um IP Público
<img width="700" height="auto" alt="image" src="https://github.com/user-attachments/assets/9cb8da4e-68a3-474b-acd9-c46408728f37" />


6. Revise a máquina e crie ela caso esteja de acordo  
<img width="700" height="auto" alt="image" src="https://github.com/user-attachments/assets/cb2e2f3a-48dd-42bf-9a08-67dddfbffa53" />

7. E por último, após a criação da VM, libere as seguintes portas de entrada
<img width="1007" height="200" alt="image" src="https://github.com/user-attachments/assets/1ea3822d-a251-4a29-a772-e5842d396c99" />

---
**Instalação do Docker no ambiente Linux (Feito em um sistema com gerenciador de pacotes "apt")**  
1. Digite apt upgrade para atualizar a lista de pacotes do sistema  
```sudo apt upgrade -y```

2. Vamos instalar o docker e o docer-compose no sistema  
```sudo apt install docker.io && sudo apt install docker-compose```

3. Faça download do fiware descomplicado usando o git  
```git clone https://github.com/fabiocabrini/fiware```

4. Entre no diretório  
```cd fiware```

5. Faça o buld  do projeto no docker  
```sudo docker-compose up -d```

**Pronto sistema montado!**


---

|Bíblioteca|Função|
|--|--|
|[WiFi.h](https://docs.arduino.cc/libraries/wifi)|Permite que o arduino conecte a internete WiFi|
|[PubSubClient.h](https://docs.arduino.cc/libraries/pubsubclient)|Permite que o arduino mande e receba mensagens MQTT|


---
### Links para visualização

[Simulação no WokWi](https://wokwi.com/projects/441460431040464897)  
[Video no YouTube demonstrando o projeto](https://youtu.be/L4Cd7HWDTmM)

---

> Criado pelo [Grupo Nexus](https://github.com/Nexus-Consulting-FIAP)

