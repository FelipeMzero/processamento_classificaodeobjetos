# Processamento de Imagens - BSI 2022.2 

## Classificação de Imagens

### ![Descrição](https://img.icons8.com/fluency/48/000000/document.png) Descrição do Projeto
O projeto visa treinar um modelo de machine learning para a classificação de objetos utilizando a plataforma **Teachable Machine**. O modelo será treinado com **5 diferentes classes de objetos** e, após o treinamento, será exportado nos formatos `labels.txt` e `keras_model.h5` para uso em um código Python. No ambiente Python, o modelo será aplicado para classificar os objetos que aparecem na filmagem, seguida da verificação da acurácia através da comparação entre as previsões realizadas e as classes reais dos objetos. O objetivo final é avaliar o desempenho do modelo, calculando o percentual de acertos das classificações.

### ![Instalação](https://img.icons8.com/fluency/48/000000/download.png) Instruções de Instalação
1. Após o treinamento do modelo no Teachable Machine, exporte os arquivos:
   - `labels.txt`: contém os rótulos das classes.
   - `keras_model.h5`: contém o modelo treinado.

2. Salve ambos os arquivos na mesma pasta onde estará o código Python que será usado para carregar o modelo e realizar a classificação de objetos. **Certifique-se de que ambos os arquivos estejam no mesmo diretório que o código**, para garantir que o Python possa acessá-los corretamente durante a execução.

### ![Uso](https://img.icons8.com/fluency/48/000000/settings.png) Instruções de Uso
O código incluído no repositório utiliza a **Iriun Webcam** como fonte de vídeo, que transforma o celular em uma webcam. Para usá-la, siga estes passos:

1. Instale o aplicativo Iriun no celular e no computador.
2. Conecte ambos na mesma rede Wi-Fi ou via cabo USB.
3. Execute o código Python.

O código carregará automaticamente o modelo treinado (`keras_model.h5`) e usará a câmera para capturar imagens em tempo real e classificá-las. Foram criadas 5 classes de objetos:
-  Boneco do Batman
-  Bola
-  Máquina de cartão
- Pasta térmica
-  HD

Caso deseje utilizar uma webcam diferente (como a do seu laptop ou outra câmera externa), será necessário alterar o índice da câmera no código Python. Normalmente, o índice **0** corresponde à webcam padrão do laptop, enquanto **1**, **2**, etc., referem-se a câmeras externas. Ajuste essa numeração no método `cv2.VideoCapture()`, alterando o número conforme a câmera que deseja usar.

###  Créditos
**Felipe Monteiro Picanço**  
Avaliação realizada remotamente via **Anaconda Python**
