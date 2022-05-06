---
layout: post
title: Máquina de Turing
subtitle: Uma introdução ao modelo por trás de toda a teoria da informação e computação moderna.
cover: /assets/images/automato/turing/cover.svg
tags: automato teórico
project: automato
color: mahogany 
---

# Máquina de Turing

#### [[Post Original]](https://iq.opengenus.org/general-introduction-to-turing-machine/)

<br />

O matemático **Alan Turing** contribuiu massivamente com vários dos conceitos que 
são utilizados hoje no universo computacional, sendo o responsável por conceber 
a base da teoria da computação moderna. Seu modelo de máquina automática 
(conhecida posteriormente como Máquina de Turing) provou diversas propriedades 
que possibilitou os computadores modernos. 

O principal objetivo de Turing ao criar seu modelo matemático foi contornar o 
problema das máquinas eletromecânicas da época, as quais eram construídas para 
resolverem problemas específicos. Caso fosse necessário ajustar o cálculo, o 
mecânismo da máquina em si deveria ser projetado novamente, o que poderia levar 
meses.

A **Máquina de Turing** opera de forma diferente, seu modelo é 
controlado por um mecânismo de propósito geral, o qual pode ser reprogramado para 
cumprir diferentes tarefas. Algo bem parecido com a ideia de um computador 
digital moderno, podemos dizer que os dois são equivalentes, apesar dos 
computadores atuais terem mais limitações se comparados à uma Máquina de Turing teórica.


# Definição

O modelo criado por **Turing** consiste em: um **controlador** finito, uma **fita** de entrada 
com infinitas células e uma **cabeça** de leitura / escrita. Cada célula pode ter 
escrito um símbolo de um conjunto restrito de caracteres, junto com o símbolo especial 
em branco (**B**), para representar as células sem nenhuma entrada. 

[imagem de partes da máquina de turing]

Uma vez programada, a máquina age de forma iterativa e cíclica onde:
- A cabeça de leitura se posiciona em frente a uma célula da fita de entrada,
- Lê o símbolo presente naquela célula e envia para o controlador,  
- Uma vez interpretado, o controlador envia para a cabeça de escrita um novo valor 
para sobreescrever aquela célula e para qual direção a fita deve se mover a seguir,
- Mover a fita para a próxima posição.

O controlador pode ser definido por meio de uma máquina de estados finita, a qual 
tem um **estado inicial** e um ou mais **estados finais**. Junto com os estados, o 
controlador contêm um conjunto de **funções de transições**, que permitem a mudança 
entre os estados a partir dos símbolos escritos na fita de entrada. 

A fita de entrada será validada pela máquina se, a partir do estado inicial, o 
controlador consiga chegar a um dos seus estados finais, terminando a sua operação 
com sucesso. O controlador abaixo escreve a sequência **quadrado triangulo quadrado**
em uma fita em branco.

# Exemplo

# Máquina de Turing Universal