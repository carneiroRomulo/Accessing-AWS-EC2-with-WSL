# Acessar AWS EC2 através da WSL e 

## Passo 01
Ao logar na AWS, clicar no menu superior esquerdo de Serviços e abrir o EC2

![tela01](Images/tela01.jpeg)

---

## Passo 02
Iniciar uma nova instância clicando no botão ``Launch Instance``

![tela02](Images/tela02.jpeg)

---

## Passo 03
Selecionar a ``AMI`` desejada

![tela03](Images/tela03.jpeg)

---

## Passo 04
Escolher o ``Tipo de Instância`` desejada

![tela04](Images/tela04.jpeg)

---

## Passo 05
Configurar os detalhes da instância

![tela05](Images/tela05.jpeg)

---

## Passo 06
Escolher os detalhes de armazenamento desejada

![tela06](Images/tela06.jpeg)

---

## Passo 07
Adicionar tags caso necessário

![tela07](Images/tela07.jpeg)

---

## Passo 08
Configurar o ``Grupo de Segurança``

![tela08](Images/tela08.jpg)

---

## Passo 09
Checar se está tudo certo e clicar em ``Launch``

![tela09](Images/tela09.jpg)

---

## Passo 10
Criar um novo ``Key Pair``, fazer seu download e armazená-lo em um local seguro, pois ela te dará acesso a instância, se for perdida não é possível acesar mais a instância. Feito isso, basta clicar em ``Launch Instances``

![tela10](Images/tela10.jpeg)

---

## Passo 11
Ao ser redirecionado para a página do Status, clicar em ``View Instances``

![tela11](Images/tela11.jpeg)

---

## Passo 12
Selecionar a instância criada clicando no ID da mesma

![tela12](Images/tela12.jpeg)

---

## Passo 13
Clicar em ``Connect`` e ir para para a aba ``SSH Client``

![tela13](Images/tela13.jpeg)
![tela14](Images/tela14.jpeg)

---

## Passo 14
Abrir o terminal do WSL no diretório em que se encontra o ``Key Pair`` e rodar os comandos indicados no ``Passo 13``. A partir daí estará dentro da intância na AWS

![tela15](Images/tela15.jpeg)

## Passo 15
Para rodar um script periodicamente pode-se usar comandos ``cron``. Com a implementação de um código python simples que gera um arquivo com a data atual, basta checar a localização do diretório atual e criar um arquivo ``.cron``.

![tela16](Images/tela16.jpeg)

---

## Passo 16
Abrindo-o basta preenche-lo com o formato:

``min hour day(month) month day(week) python3 LocalDoArquivo``

Para fins de teste o código foi executado a cada minuto. Para formatar um crontab com alguma outra frequência o site [crontab guru](https://crontab.guru/#*_*_*_*) pode ajudar. 

![tela17](Images/tela17.jpeg)

---

## Passo 17
Para que a tarefa cron funcione corretamente basta executar o arquivo cron e o código irá rodar periodicamente no tempo desejado.

![tela18](Images/tela18.jpeg)
![tela19](Images/tela19.jpeg)
