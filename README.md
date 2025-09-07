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

Esse é o protótipo <ins>Smart Lamp</ins>, ou <ins>"Lampada Inteligente"</ins> do grupo **Nexus** com o uso do **ESP32** na plataforma **FIWARE**, podendo interagir e registrar a luminosidade do local por meio do **LDR** e ligar ou desligar a **LED** presente no **ESP32**.
Por ainda estar em fase de protótipo,  não foi definido ainda uma conexão entre a **LED** e a detecção de luminosidade do **LDR**, possivelmente será usado para detectar se um cômodo está claro ou escuro e se ligar ou desligar automaticamente.

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

