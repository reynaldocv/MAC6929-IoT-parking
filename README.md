
# IoT-project (Vagas no Estacionamento)

- Visão geral do projeto: 

    O projeto consiste em saber se tem vagas (ou não) num estacionamento. 

    A projeto a discutir, pode ajudar às pessoas a saber onde eles podem estacionar seu veiculo (no momento), e
fazer uma estimativa a futuro se no estacionamento.

                            ![stack Overflow](/img/img_car.jpeg)

- Público alvo: 

Toda pessoa que tem um veiculo. 

# Descrição técnica
  
- Módulos:

  - O módulo câmera VGA OV7670 é um módulo que permite a captura e armazenamento de imagens coloridas pelo seu Arduino, com        uma taxa de atualização de até 30 frames por segundo, com resolução máxima de 640 x 480 Pixels.
      ![stack Overflow](/img/ov7670.png)


      - Especificações:      
        - Tensão de Alimentação:  4-30V;
        - Escala Linear: + 10.0 mV/˚C;
        - Temperatura de trabalho em modo básico: 2 a 150ºC;
        - Temperatura de trabalho em range completo: -55 a +150º C;
        - Baixa impedância de saída
      
  - O Módulo Wireless ESP8266 permite conectar o seu Arduino nas redes wireless 802.11 b/g/n, enviando e recebendo dados nos modos AP (Access Point/Ponto de acesso) e STA (Station)  
  ![stack Overflow](/img/Esp8266.png)


      - Especificações:      
        - Conexão à redes padrão 802.11 B/G/N
        - Alcance aproximado: 91 metros
        - Tensão de operação : 3.3 VDC
        - Comunicação serial: pinos TX e RX
        - Modos de operação : Cliente, Access Point, Cliente+Access Point
        - Modos de segurança wireless : OPEN/WEP/WPA_PSK/WPA2_PSK/WPA_WPA2_PSK.
        - Suporta comunicação TCP e UDP, com até 5 conexões simultâneas
      
   
   
   
## Open-design (extra)
(Apresentar o design técnico do projeto utilizando alguma ferramenta de diagrama ou mesmo um desenho à mão. Sugestão de ferramentas: Draw.io, Fritzing.org, Gimp.)

# Descrição da arquitetura

A seguir vamos explicar o fluxo da informação:

Cada vez que uma pessoa, quer saber se tem uma vaga no estacionamento, manda una sinal para o Arduino, 
e tira uma foto (usando o módulo ) no estacionamento, E essa foto é enviada para seu processamento (usando o módulo ).
E o sistema sabendo quantos carros tem na foto, joga o número de vagas.

Com esses dados, podemos fazer um monte de reportes: 
 - (No momento) Quantas vagas tem no estacionamento.
 - (Estimativas pro futuro) Quantas vagas vai ter, segundo aos dados anteriores? 
 
## Referências   
 - https://portal.vidadesilicio.com.br/sensor-de-luz-com-ldr/
 - https://www.filipeflop.com/produto/sensor-de-luminosidade-ldr-5mm/
 - https://portal.vidadesilicio.com.br/lm35-medindo-temperatura-com-arduino/
 - https://www.arduinoecia.com.br/2013/02/lm35-sensor-de-temperatura.html
 - https://www.filipeflop.com/blog/modulo-camera-vga-ov7670/
 - https://www.robocore.net/loja/produtos/modulo-wifi-esp8266.html
 - https://www.embarcados.com.br/modulo-esp8266/


