# Detector de Luminosidade com Lanterna Automatica

Aplicativo Android desenvolvido em Kotlin que utiliza o sensor de luz ambiente do dispositivo para alterar dinamicamente o tema da interface e controlar o acionamento da lanterna traseira de forma automatizada.

## Sobre o projeto

O objetivo principal deste projeto foi explorar a integração do desenvolvimento Android com os componentes físicos (hardware) do smartphone. O aplicativo monitora constantemente a iluminação do ambiente por meio do sensor de luminosidade do aparelho.

Caso o sensor detecte um nível de iluminação abaixo de **50 lux** (indicando um ambiente escuro ou que o sensor foi coberto), a interface do aplicativo muda instantaneamente para uma cor escura e a lanterna do dispositivo é ligada de forma automática. Quando a luminosidade volta a subir, a interface retorna ao modo claro e a lanterna é desligada.

## Funcionalidades

- Leitura em tempo real dos dados do sensor de luminosidade física (Sensor.TYPE_LIGHT) em lux;
- Interface adaptativa dinâmica (muda as cores de fundo e de texto de acordo com a luz ambiente);
- Controle automatizado de hardware para ligar e desligar a lanterna (CameraManager) sem necessidade de cliques;
- Exibição do status atual da lanterna e da medição exata em lux na tela;
- Interface personalizada com a identidade visual do IFSul Campus Pelotas.

## Tecnologias utilizadas

- Kotlin
- Android Studio
- Android SDK (SensorManager e CameraManager)

## Contexto acadêmico

Projeto prático desenvolvido durante o Curso Técnico em Eletrônica do Instituto Federal Sul-rio-grandense (IFSul) – Campus Pelotas, com o intuito de aplicar conceitos de programação mobile voltados à automação e leitura de sensores.

## Objetivos de aprendizagem

Durante o desenvolvimento deste projeto foram praticados conceitos como:

- Configuração e ciclo de vida de sensores no ecossistema Android;
- Tratamento de eventos de hardware em tempo real com listeners;
- Gerenciamento de permissões de hardware e acesso a periféricos do sistema (câmera/flash);
- Manipulação dinâmica de estilos e estados de componentes da interface gráfica;
- Estruturação de código em Kotlin para respostas rápidas a estímulos externos.

### Interface em Ambiente Escuro

Quando o sensor detecta menos de 50 lux (por exemplo, 0,0 lux ao ser totalmente tampado), a tela escurece e exibe o texto informativo, acionando a lanterna do aparelho simultaneamente.

<img width="720" height="1549" alt="WhatsApp Image 2026-06-16 at 21 58 03" src="https://github.com/user-attachments/assets/936d4c99-7187-4023-9dd6-f423e2635112" />

### Interface em Ambiente Claro

Quando o sensor detecta uma luminosidade igual ou superior a 50 lux, a interface do aplicativo permanece clara e estável. Nesse estado, a lanterna do dispositivo continua desligada e o aplicativo apenas exibe na tela o nível atual de iluminação ambiente capturado em tempo real.

<img width="720" height="1549" alt="WhatsApp Image 2026-06-16 at 21 58 03 (1)" src="https://github.com/user-attachments/assets/f1f3d1ed-a647-4b14-aed3-5a748375eb2d" />


## Observações

Este projeto possui caráter educacional, servindo como demonstração prática de integração entre software e sensores físicos no ambiente Android.
