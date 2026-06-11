# Projeto de Detecção de Veículos com YOLOv8

---

### Objetivo

O principal objetivo deste projeto é implementar e demonstrar a técnica de **Transfer Learning** (Transferência de Aprendizado) utilizando o modelo YOLOv8 para uma tarefa específica de visão computacional. O modelo, que foi inicialmente treinado no vasto dataset COCO, foi ajustado (fine-tuned) para detectar e localizar com precisão vários tipos de **veículos** (carros, caminhões, ônibus) em imagens.

---

### Metodologia

O projeto seguiu um pipeline padrão de detecção de objetos:

1.  **Aquisição de Dados:** Um dataset de veículos já anotado (com as caixas delimitadoras) foi obtido no **Roboflow Universe**, garantindo que os dados estivessem no formato ideal para o YOLO.
2.  **Configuração do Ambiente:** O ambiente Google Colab foi configurado, e a biblioteca `ultralytics` (YOLOv8) foi instalada.
3.  **Transfer Learning:** Um modelo YOLOv8 'nano' pré-treinado (`yolov8n.pt`) foi carregado e retreinado por 20 épocas usando o dataset personalizado de veículos.
4.  **Avaliação:** O desempenho do modelo foi analisado usando métricas cruciais como o mAP (mean Average Precision) e a matriz de confusão.
5.  **Inferência (Teste):** O modelo de melhor desempenho (`best.pt`) foi testado em imagens que ele nunca havia visto para validar sua capacidade de detecção.

---

### Tecnologias Utilizadas

| Tecnologia | Finalidade |
| :--- | :--- |
| **YOLOv8** | Modelo de detecção de objetos de última geração (da Ultralytics). |
| **PyTorch** | Framework de Deep Learning utilizado como base para o YOLOv8. |
| **Google Colab (GPU)** | Ambiente baseado em nuvem que fornece o poder de processamento necessário para o treinamento. |
| **Roboflow** | Plataforma utilizada para aquisição e formatação do dataset. |
| **Python** | Linguagem de programação principal utilizada para o desenvolvimento e execução. |

## Uso de IA
Este projeto contou com auxílio de ferramentas de Inteligência Artificial para geração de trechos de código e ideias de implementação. Todo o material foi revisado, adaptado e testado manualmente antes da publicação.
