# Acessando AWS EC2 através da WSL

## Passo 01
Ao logar na AWS, clicar no menu superior esquerdo de Serviços e abrir o EC2

![Image](Images/tela01.jpeg)

---

## Passo 02
Iniciar uma nova instância clicando no botão ``Launch Instance``

![Image](Images/tela02.jpeg)

---

## Passo 03
Selecionar a ``AMI`` desejada

![Image](Images/tela03.jpeg)

---

## Passo 04
Escolher o ``Tipo de Instância`` desejada

![Image](Images/tela04.jpeg)

---

## Passo 05
Configurar os detalhes da instância

![Image](Images/tela05.jpeg)

---

## Passo 06
Escolher os detalhes de armazenamento desejada

![Image](Images/tela06.jpeg)

---

## Passo 07
Adicionar tags caso necessário

![Image](Images/tela07.jpeg)

---

## Passo 08
Configurar o ``Grupo de Segurança``

![Image](Images/tela08.jpeg)

---

## Passo 09
Checar se está tudo certo e clicar em ``Launch``

![Image](Images/tela09.jpeg)

---

## Passo 10
Criar um novo ``Key Pair``, fazer seu download e armazená-lo em um local seguro, pois ela te dará acesso a instância, se for perdida não é possível acesar mais a instância. Feito isso, basta clicar em ``Launch Instances``

![Image](Images/tela10.jpeg)

---

## Passo 11
Ao ser redirecionado para a página do Status, clicar em ``View Instances``

![Image](Images/tela11.jpeg)

---

## Passo 12
Selecionar a instância criada clicando no ID da mesma

![Image](Images/tela12.jpeg)

---

## Passo 13
Clicar em ``Connect`` e ir para para a aba ``SSH Client``

![Image](Images/tela13.jpeg)
![Image](Images/tela14.jpeg)

---

## Passo 14
Abrir o terminal do WSL no diretório em que se encontra o ``Key Pair`` e rodar os comandos indicados no [Passo 13](##-Passo-13)

![Image](Images/tela15.jpeg)