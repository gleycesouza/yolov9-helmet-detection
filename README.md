# Projeto: Criação de Base de Dados e Treinamento com YOLOv9

Este projeto tem como objetivo desenvolver e treinar uma rede YOLOv9 para realizar a detecção de capacetes de motociclistas. 
O trabalho utiliza uma base de dados rotulada para realizar o treinamento das redes neurais convolucionais.

## Estrutura do Projeto
O projeto inclui as seguintes etapas principais:
1. **Implementação e teste da rede YOLOv9**  
   A rede foi utilizada para realizar previsões em uma imagem e um vídeo. 
   Apesar de obter boas detecções em outras classes, os capacetes não foram detectados adequadamente na rede inicial. 
   Assim, o treinamento foi direcionado para a detecção dessa classe específica.

2. **Base de dados de imagens de capacetes**  
   Foi utilizada uma base de dados rotulada do Roboflow
   (https://universe.roboflow.com/yolo-do-it-yhopz/helmet-detector-9rzmg-bmd6q) 
   
3. **Configuração do YOLOv9**  
   A rede YOLOv9 foi configurada e treinada a partir de uma base de dados inicial para realizar transfer learning. 
   Foram adicionadas 13 novas classes, incluindo diversos tipos de capacetes.

4. **Treinamento da Rede**  
   O treinamento foi iniciado no Colab, utilizando a base de dados rotulada de capacetes. 
   No entanto, devido a limitações de tempo e recursos no Colab, o treinamento foi interrompido após apenas 1 época.

## Ferramentas Utilizadas
- **Base de Imagens Rotuladas**
- **Rede YOLOv9** 
- **Google Colab** 

## Resultados Parciais
- Foram realizadas predições em uma imagem e um vídeo, com boas detecções gerais, mas falha na identificação de capacetes na rede inicial.
- A rede YOLOv9 foi configurada com uma base inicial e treinada para incluir a classe *capacetes de motociclistas*.
- Dados de treinamento limitados a 1 época devido às restrições de execução no Google Colab.

## Próximos Passos
1. Continuar o treinamento para mais épocas, preferencialmente utilizando uma infraestrutura de hardware mais robusta, como GPUs locais ou serviços em nuvem.
2. Avaliar o desempenho da rede após o treinamento completo, utilizando métricas como precisão, recall e F1-Score.
3. Expandir a base de dados rotulada para incluir mais imagens de capacetes e outras classes relacionadas.

## Requisitos
- Python 3.8+
- TensorFlow
- Google Colab ou outro ambiente com suporte a GPU

## Exemplo de Detecção

### Antes do treinamento com capacetes
![Detecção antes do treinamento](caminho/para/imagem_antes.jpg)

### Durante o treinamento com capacetes
![Detecção durante o treinamento](caminho/para/imagem_durante.jpg)