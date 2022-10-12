# cauda_tiffany
A Tiffany é uma hexapod desenvolvida para andar de forma autônoma ou para ser controlada pelo celular. Para que possa transmitir o que vê e interagir com o meio, foi desenvolvida um cauda de escorpião, um manipulador robótico para ela. Esse manipulador é controlado por uma ESP32CAM e pode ser utilizado desacoplado da hexapod.

# Estrutura física
A estrutura física do manipulador é composta por quatro motores. Eles são fixadas a peças de PLA para deixar o manipulador firme. As peças são todas projetadas em 3D e foram impressas utilizando PLA, podendo ser encontradas na pasta Pecas_3d deste projeto.

<img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/tiffany_cauda.png" width="400"> <img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/cauda.png" width="300">

## Peças 3D em STL
Na pasta Pecas_3d, estão listadas as peças desenvolvidas neste projeto em STL. Para ajudar, segue abaixo uma lista de todas as peças que devem ser impressas e qual o valor da sua maior dimensão (para ajudar na escolha da impressora):
* Base
  * 1x [TIFFANY_SLIPNATTACH_FOUNDATION.STL (62 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_SLIPNATTACH_FOUNDATION.STL)
  * 1x [TIFFANY_OMBRO_DOWN_TAIL.STL (61 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_OMBRO_DOWN_TAIL.STL)
  * 1x [TIFFANY_OMBRO_UP.STL (61 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_OMBRO_UP.STL)
* Cauda
  * 8x [TUBINHO.STL (7 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TUBINHO.STL)
  * 1x [TIFFANY_CAUDA_MEIO_RIGHT.STL (178 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_RIGHT.STL)
  * 1x [TIFFANY_CAUDA_MEIO_LEFT.STL (178 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_LEFT.STL)
  * 1x [TIFFANY_ATTACHMENT_PGS_SRV.STL (114 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_ATTACHMENT_PGS_SRV.STL)
  * 1x [TIFFANY_ATTACHMENT_PGS_ROL.STL (118 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_ATTACHMENT_PGS_ROL.STL)
  * 1x [ESPCAM_CASE_BACK.STL (60 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/ESPCAM_CASE_BACK.STL)
  * 1x [ESPCAM_CASE_FRONT.STL (60 mm diagonal)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/ESPCAM_CASE_FRONT.STL)
  * 1x [TIFFANY_FEMUR_FRONT.STL (110 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_FEMUR_FRONT.STL)
  * 1x [TIFFANY_FEMUR_BACK.STL (118 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_FEMUR_BACK.STL)
 * Motor
  * 3x [TIFFANY_TAMPA_MOTOR.STL (41 mm)](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_TAMPA_MOTOR.STL)

Obs: a tampa de 3 motores deverão ser trocadas pelas peças [TIFFANY_TAMPA_MOTOR.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_TAMPA_MOTOR.STL) para que seja possível fixar os rolamentos nas patas. Serão utilizados 3 rolamentos por pata. Os tubinhos [TUBINHO.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TUBINHO.STL) servem como espaçadores das peças [TIFFANY_CAUDA_MEIO_RIGHT.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_RIGHT.STL) e [TIFFANY_CAUDA_MEIO_LEFT.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_LEFT.STL):

<img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/cauda_explodida.png" width="500">

Obs2: a base da antena da ESP32CAM fica presa na peças [ESPCAM_CASE_BACK.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/ESPCAM_CASE_BACK.STL) e [TIFFANY_ATTACHMENT_PGS_ROL.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_ATTACHMENT_PGS_ROL.STL) com ajuda da porca que vem junto dela:

<img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/antena_montagem.png" width="500">

## Outros itens da estrutura
Alguns outros itens são necessários para finalizar a estrutura da cauda da Tiffany:
* 4x Parafusos m4 de cm: prender as peças [TIFFANY_OMBRO_DOWN_TAIL.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_OMBRO_DOWN_TAIL.STL) e [TIFFANY_OMBRO_UP.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_OMBRO_UP.STL)
* 8x Parafusos m3 de cm: prender as peças [TIFFANY_CAUDA_MEIO_RIGHT.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_RIGHT.STL) e [TIFFANY_CAUDA_MEIO_LEFT.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_CAUDA_MEIO_LEFT.STL) nos motores
* 6x Parafusos de 2,4mm de diâmetro com ponta: prender as peças [TIFFANY_ATTACHMENT_PGS_SRV.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_ATTACHMENT_PGS_SRV.STL) e [TIFFANY_ATTACHMENT_PGS_ROL.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/TIFFANY_ATTACHMENT_PGS_ROL.STL) nas peças [ESPCAM_CASE_BACK.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/ESPCAM_CASE_BACK.STL) e [ESPCAM_CASE_FRONT.STL](https://github.com/Penguin-Lab/cauda_tiffany/blob/main/Pecas_3d/ESPCAM_CASE_FRONT.STL)

## Placas de circuito impresso
No projeto, foram desenvolvidas duas placas de circuito para servir como:
* Shield para a ESP32CAM
* Placa de alimentação dos motores

<img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/shield_espcam.png" width="220"> <img src="https://github.com/Penguin-Lab/cauda_tiffany/blob/main/images/alimentacao.png" width="220">

## Componentes eletrônicos
Os componentes eletrônicos embarcados no robô e equipamentos utilizados são:
* Controlador com Wi-fi
  * 1x ESP32CAM (com antena externa)
* Motores
  * 4x Servo TowerPro MG995 Metálico
* Alimentação
  * Bateria de 9V (ESP32)
  * Bateria Zippy 1100mAh 2s 6,6v (motores)

# Software
Na pasta de códigos, há o código de programação da ESP32CAM. Este é um exemplo em C++ de comando de movimentação dos motores e de transmissão de imagens da câmera. A ESP32CAM é controlada pelo próprio web server que ela gera (192.168.1.1) para apresentar as imagens.
