# TesteCheckListFacil

Pré-requisitos

- Descompactar os arquivos zipados do projeto no diretório "C" do computador que realizará os testes.
- O Docker e Selenium precisam estar instalados e funcionando.
- As imagens do Selenium, Selenium Chrome headless precisam ser extraídas do Docker Hub.
- Use o seguinte comando no CMD (Como administrador) para extrair as imagens do Docker Hub: "docker pull selenium/hub && docker pull selenium/node-chrome && docker pull selenium/node-chrome-debug"

Antes de executar os testes

Antes de executar os testes, certifique-se de que os contêineres do Selenium hub e Chrome headless estão ativos e em execução.

Use "docker ps -a" para verificar se eles estão funcionando.
Se eles não estiverem em execução, entre via CMD na pasta "C:\TesteCheckList" e use o comando "docker-compose up -d" para iniciá-los.

- Para reiniciar o uso de containers use "docker-compose restart".
- Para desligar os recipientes, use: "docker-compose down".

Verificando a grade do Selenium

Com os contêineres instalados e em execução, acesse a seguinte URL em seu navegador para verificar se a grade do Selenium foi configurada corretamente: http://localhost:4444/grid/console .

Executando os testes

Para executar os testes você deve abrir o Eclipse, clicar no menu File, Open Projects from File System, Directory, selecionar a pasta "TesteCheckList" que deve estar no diretório C da maquina e por ultimo no botão Finish.
Ao abrir o projeto, basta clicar com o botão direito do mouse na pasta "TesteCheckList", ir até a opção "Run As" e selecionar a opção "JUnit Test".
