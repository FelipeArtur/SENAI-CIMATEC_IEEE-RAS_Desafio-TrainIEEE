# Projeto RAS Equipe B
## Introdução

Este repositório foi criado para o desenvolvimento do Desafio TrainIEEE referente ao processo seletivo realizado em 2021.2.

O desafio consistia na criação de um Sistema de assistente de estacionamento baseado em sensores ultrassônicos, os materiais necessários para o desenvolvimento do projeto foram: 
- 01 - Arduino UNO;
- 03 - Sensores Ultrassônicos (HC-SR04);
- 03 - Vermelho LED;
- 03 - Amarelo LED;
- 03 - Verde LED;
- 01 - Piezo; 
- 01 - Motor CC;
- 09 - Resistor 200Ω;

## Organização
A seguinte organização das pastas foi seguida: 
- `Code`: Contêm o código com extensão .ino;
- `Circuit`: Contêm o versionamento dos circuitos;
- `Resources`: Pasta de apoio para conteúdos do README.md

## Instalação
### Repositório GitHub
Para fazer o download deste repositório basta clonar numa pasta de sua `preferência`.

```

$ git clone https://github.com/FelipeArtur/Projeto-RAS-Equipe-B

```

### Arduino
- Para instalação da IDE Arduino acesse https://www.arduino.cc/en/software e escolha a opção referente ao seu sistema operacional.
- Caso prefira, é possível acessar o compilador online https://create.arduino.cc/editor

## Desenvolvimento
### Hardware
O circuito do projeto pode ser visto na imagem a seguir: 

![banner](https://github.com/FelipeArtur/Projeto-RAS-Equipe-B/blob/main/Circuit/TrainIEEE%20RAS%20v.2.png?raw=true)

### Software
Abra o arquivo code.ino localizado na pasta Projeto-RAS-Equipe-B/Code e carregue-o no seu Arduino

## Simulação
O sistema alerta o motorista com diferentes tipos de sinais a distancia que o sensor se encontrar do obstáculo: 

### Led Verde: OK
  - Caso a distáncia entre o sensor e o obstaculo seja maior que 50cm este caso está ativo;
  - Não há emissão de sinal sonoro;
  - Há a emissão de uma luz verde pulsante;

### Led Amarela: ATENÇÃO 
  - Caso a distáncia entre o sensor e o obstaculo seja maior que 20cm e menor ou igual a 50cm este caso está ativo;
  - Não há emissão de sinal sonoro;
  - Há a emissão de uma luz amarela pulsante;

### Led Vermelha: PERIGO
  - Caso a distáncia entre o sensor e o obstaculo seja menor que 20cm este caso está ativo;
  - Há emissão de sinal sonoro estridente e curto em sintonia com o sinal visual;
  - Há a emissão de uma luz vermelha pulsante;

### Observações: 
  - Cada sensor tem um conjunto de três led's para o pleno funcionamento do sistema.
  - Há apenas um piezo responsável pela emissão do sinal sonoro, desta forma, o som é repetido de forma cíclica começando pelo sensor trazeiro, seguindo para o dá direita e finalizando com o da esquerda. 

## Informações para contato

### **Felipe Artur Macedo Lima**
- E-mail: felipe.lima@aln.senaicimatec.edu.br
- GitHub: https://github.com/FelipeArtur
- LinkedIn: https://www.linkedin.com/in/felipeartur/

### **Felipe Valente Santos Fiscina**
- E-mail: felipe.fiscina@aln.senaicimatec.edu.br
- GitHub: https://github.com/ValenteSF
- LinkedIn: https://www.linkedin.com/in/felipefiscina/

### **Nicolas Christian de Souza Dunham**
- E-mail: nicolas.dunham@aln.senaicimatec.edu.br 
- GitHub: https://github.com/braviun
- LinkedIn: https://www.linkedin.com/in/nicolas-christian-de-souza-dunham-922bb5222/
