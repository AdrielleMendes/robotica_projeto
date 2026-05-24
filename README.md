# SARAS – Sistema Robótico Inteligente Autônomo com Inteligência Artificial

O **SARAS** (Smart Autonomous AI Robotic System) é um robô com inteligência artificial (IA) do tipo "faça você mesmo" (DIY), capaz de realizar navegação básica, visão computacional, interação por voz e comportamento autônomo. Este repositório foca na **construção do hardware**, sendo ideal para estudantes, entusiastas e hobbistas que desejam dar vida à inteligência artificial por meio da robótica física.

Este arquivo resume os componentes de hardware, as etapas de montagem, as instruções de fiação e os objetivos gerais do projeto.

---

## 🚀 Características

* **Chassi modular de 3 camadas:** Projetado para impressão 3D (ou materiais alternativos como acrílico/papelão).
* **Processamento:** Raspberry Pi (3 ou 4B).
* **Interface Visual:** Tela HDMI de 7 polegadas (para o "rosto" do robô).
* **Entrada de Áudio:** Microfone omnidirecional USB (para comandos de voz).
* **Saída de Áudio:** Alto-falante USB (para respostas do robô).
* **Visão Computacional:** Módulo de Câmera oficial da Raspberry Pi.
* **Locomoção:** Controle básico de movimento usando 4 motores CC.
* **Driver de Motores:** Ponte H L298N.
* **Prevenção de Colisões:** Detecção de obstáculos usando 3 sensores ultrassônicos.

---

## 🛠️ Lista de Componentes

| Componente | Quantidade | Notas |
| :--- | :---: | :--- |
| **Motores CC + Redução** | 4 | Motores comuns para chassi de robô |
| **Pneus Grandes** | 4 | Rodas maiores para melhor tração e estética |
| **Driver de Motor L298N** | 1 | Ponte H para controlar a velocidade e direção dos motores CC |
| **Raspberry Pi** | 1 | O "cérebro" principal do robô |
| **Monitor HDMI (7 polegadas)** | 1 | Usado para exibir as expressões e interface do robô |
| **Microfone Omnidirecional USB** | 1 | Para capturar as ordens e comandos de voz |
| **Alto-falante USB** | 1 | Para o feedback e respostas de áudio da IA |
| **Fios Jumper e Espaçadores** | - | Para conexões elétricas e empilhamento das camadas |
| **Baterias 18650 + Suporte** | 2 | Alimentação dedicada para os motores CC |
| **Power Bank (5V)** | 1 | Alimentação estável dedicada para a Raspberry Pi |
| **Sensores Ultrassônicos (HC-SR04)** | 3 | Para leitura de distância (frente, esquerda e direita) |
| **Chassi Modular** | 1 | Estrutura de 3 andares impressa em 3D |

---

## 📐 Visão Geral do Design (Estrutura)

O robô utiliza um design modular empilhado em três níveis distintos:
1. **Camada Base:** Abriga os motores, rodas, o driver L298N e o suporte de baterias dos motores.
2. **Segunda Camada:** Onde fica fixada a Raspberry Pi e o Power Bank.
3. **Terceira Camada (Topo):** Suporte para o microfone, alto-falante, câmera e a tela de 7 polegadas.

---

## 🔌 Resumo das Etapas de Montagem

1. Fixe os motores CC no chassi base, utilizando os espaçadores para garantir que as rodas grandes tenham espaço para girar livremente.
2. Interligue os motores das laterais e conecte-os nas saídas do driver L298N (atenção à polaridade para as rodas não girarem ao contrário).
3. Monte os espaçadores de latão/plástico para erguer a estrutura do segundo andar.
4. Fixe a Raspberry Pi no segundo andar e posicione o banco de energia.
5. Faça a fiação dos pinos de controle do L298N até os pinos **GPIO** da Raspberry Pi.
6. Instale a câmera e os sensores ultrassônicos na estrutura do topo, conectando o monitor, microfone e alto-falante nas portas USB/HDMI da Pi.
7. Ligue os sistemas de alimentação, verifique o boot do sistema e inicie os testes de movimentação.

---

## 👥 Equipe de Desenvolvimento (Equipe Cronnos)

Este projeto está sendo adaptado, montado e programado por:
* **Adrielle Mendes** - [GitHub](https://github.com/AdrielleMendes)
* **Alane Martins**-https://github.com/Alanemmartins
* **Antônio Miranda**-https://github.com/toninhowow

## 📌 Créditos e Referências
* **Projeto Base e Conceito de Hardware:** Baseado no robô inteligente SARAS criado por Anant Sharma https://youtu.be/IT1uBUsOmUY?si=wg5ped7aim7uzl9K
