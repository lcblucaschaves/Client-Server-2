#Projeto: Super Mario World - Inteligência Artificial - 2023.Q3

Prof. Fabrício Olivetti de França (folivetti@ufabc.edu.br) - UFABC

## Enunciado

Esse é um projeto onde implementamos um agente inteligente capaz de jogar a fase *YoshiIsland2* do jogo Super Mario World, utilizando um dos algoritmos apresentados em aula na segunda metade do curso.

Os algoritmos devem ser escritos em Python e farão uso da biblioteca Retro Gym (https://github.com/openai/retro).

## Grupos

Esse projeto foi realizado por:

```
Nome: CARLOS HENRIQUE ALENCAR LIMA  RA: 11202021040. 
Nome: LUCAS CHAVES BATISTA         	RA: 11201921079.
```

##Instruções de Instalação

Previamente, é necessário que o `pyenv` já esteja instalado para gerenciar o ambiente e as diferentes versões do python. Após instalado, siga estes comandos:

```bash
pyenv install 3.8.0
pyenv shell 3.8.0
python -m venv marioenv #(esse comando vai criar o ambiente do mario)
.\marioenv\source\activate #(caso esteja em linux, utilize source marioenv/bin/activate)
pip install -r requeriments.txt #(isso vai instalar todas as bibliotecas necessarias, cujos comandos estao escritos em requeriments.txt)
cp rom.sfc .\marioenv\site-packages\retro\data\stable\supermarioworld-snes\ #isso copia a rom do jogo para a pasta do retro. Você pode fazer manualmente se quiser
 ```
Com isso, as bibliotecas estão instaladas. 

##Como rodar o código

Certifique-se de que o ambiente está ativado digitando os seguintes comandos no terminal:

```bash
pyenv shell 3.8.0
.\marioenv\source\activate #(caso esteja em linux, utilize source marioenv/bin/activate)
```

###Treinamento do Agente

Para *TREINAR* o agente em alguma fase, utilize o comando `python train.py` e em seguida informe a fase desejada, a permissão para paralelismo, e a opção de visualização quando solicitado. O treinamento será iniciado.

###Execução do Agente

Para *EXECUTAR* o agente em alguma fase, utilize o comando `python play.py`, em seguida informe a fase desejada, e o agente será iniciado, permitindo que você observe o agente jogando a fase escolhida.
