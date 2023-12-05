Super Mario AI
Instruções de Instalação
Antes de começar, certifique-se de ter o pyenv instalado para gerenciar o ambiente e as diferentes versões do Python. Siga os passos abaixo após a instalação do pyenv:

Instale o Python 3.8.0 utilizando o comando:

bash
Copy code
pyenv install 3.8.0
Defina o Python 3.8.0 como padrão para o seu ambiente:

bash
Copy code
pyenv shell 3.8.0
Crie um ambiente virtual chamado marioenv utilizando o comando:

bash
Copy code
python -m venv marioenv
Ative o ambiente virtual (Linux):

bash
Copy code
source marioenv/bin/activate
Ou ative o ambiente virtual no Windows:

bash
Copy code
.\marioenv\Scripts\activate
Instale as bibliotecas necessárias listadas no arquivo requirements.txt:

bash
Copy code
pip install -r requirements.txt
Copie o arquivo de ROM (rom.sfc) para o diretório do ambiente virtual:

bash
Copy code
cp rom.sfc .\marioenv\site-packages\retro\data\stable\supermarioworld-snes\
Agora, todas as bibliotecas estão instaladas e o ambiente está configurado.

Como Rodar o Código
Certifique-se de que o ambiente está ativado digitando os seguintes comandos no terminal:

bash
Copy code
pyenv shell 3.8.0
source marioenv/bin/activate  # (ou .\marioenv\Scripts\activate no Windows)
Treinamento do Agente
Para treinar o agente em uma fase específica, utilize o comando:

bash
Copy code
python train.py
Informe a fase desejada, a permissão para paralelismo e a opção de visualização quando solicitado. O treinamento será iniciado.

Execução do Agente
Para executar o agente em uma fase específica, utilize o comando:

bash
Copy code
python play.py
Informe a fase desejada e o agente será iniciado, permitindo que você observe o agente jogando a fase escolhida.

Divirta-se jogando com o Super Mario AI!




