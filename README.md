# Chaves Quânticas & Simulação de Sistemas Seguros

---

## Visão Geral do Projeto

Este projeto tem como objetivo tornar a computação quântica compreensível e aplicada, explorando desde seus fundamentos teóricos até uma simulação prática de distribuição de chaves quânticas **(Quantum Key Distribution - QKD)**.

A proposta é unir educação e aplicação real, mostrando como os princípios que regem os qubits, superposição e entrelaçamento, normalmente vistos como conceitos abstratos, podem inspirar formas seguras de transferência e autenticação de informação no mundo real.

---

## Estrutura do Projeto

O projeto foi desenvolvido em formato de notebook interativo **(Google Colab)**, onde cada etapa é explicada de forma didática e acompanhada por exemplos práticos em Qiskit.

Cada seção introduz um conceito teórico, seguido de uma analogia simples e de um circuito real executável em simuladores quânticos da IBM.

---

## Como os temas são abordados

O aprendizado é progressivo: começamos com os fundamentos da computação quântica e finalizamos aplicando o conceito de chaves quânticas a um caso prático de transferência segura de informação, simulando o comportamento de sistemas de pagamento ou de autenticação inspirados em princípios de criptografia quântica.

### Etapas principais

#### Computação Quântica e Qubits
Explicamos o que é a computação quântica, como ela difere da clássica e por que os **qubits** são unidades de informação mais poderosas.
Usamos analogias e visualizações para ilustrar os conceitos de **superposição** e **emaranhamento**.

#### Qiskit, O "Hello World" Quântico
Configuramos o ambiente com Qiskit e criamos um circuito simples (estado de Bell) que representa o “Hello World” da computação quântica, o primeiro passo para observar o **entrelaçamento entre qubits**.

#### Operadores Quânticos Fundamentais
Exploramos duas portas essenciais:
- **Hadamard (H):** cria superposição, o qubit passa a ser 0 e 1 ao mesmo tempo.
> Analogia: um feixe de luz que vibra em duas direções ao mesmo tempo.
- **CNOT (Controlled-NOT):** conecta qubits, o estado de um passa a depender do outro.
> Analogia: duas lâmpadas inteligentes sincronizadas.

Cada operador é explicado conceitualmente e visualmente, com exemplos práticos em Qiskit e histogramas mostrando os resultados das medições.

---

## Chaves Quânticas (QKD): O que é?

A **Distribuição de Chaves Quânticas (QKD)** permite que duas pessoas (vamos chamá-las de **Alice** e **Bob**) criem uma chave secreta compartilhada usando as propriedades da física quântica.

O truque é o seguinte: se alguém tentar espionar a comunicação, os estados quânticos dos qubits mudam automaticamente.
É como se a própria natureza delatasse o espião.
Com isso, Alice e Bob conseguem perceber se há algo errado e descartar aquela tentativa de conexão.

---

### Como funciona na prática?

1. Alice prepara vários qubits em estados aleatórios e manda para Bob.
2. Bob mede esses qubits, também escolhendo aleatoriamente em qual base vai medir cada um.
3. Depois, eles conversam publicamente sobre as bases usadas (não sobre os resultados).
4. Eles descartam os qubits medidos em bases diferentes e ficam apenas com os compatíveis, essa é a chave bruta.
5. Para garantir que ninguém interferiu, eles comparam uma pequena parte da chave.
6. Se tudo estiver certo, fazem ajustes e correções finais e pronto: têm uma chave secreta que só eles conhecem.

---

### O que fizemos neste projeto

Nós simulamos esse processo de criação e compartilhamento de uma chave quântica entre Alice e Bob.
A ideia é demonstrar como a mecânica quântica garante a segurança da comunicação, sem depender apenas de fórmulas matemáticas.

Essa chave depois pode ser usada em algoritmos de criptografia clássicos (como o **AES** ou o **One-Time Pad**), garantindo que só quem tem a chave consegue ler a mensagem.
E se alguém tentar copiar ou interceptar a chave, o sistema detecta automaticamente a interferência.

> **Resumindo:** não é a matemática que protege, é a física.
> Mexeu no estado do qubit? Foi denunciado.

---


## Objetivos Educacionais

- Explicar os fundamentos da computação e criptografia quântica de forma simples e acessível.
- Mostrar na prática como Qiskit é usado para criar e simular circuitos quânticos reais.
- Demonstrar o entrelaçamento e a geração de chaves quânticas de maneira visual e intuitiva.
- Fazer um paralelo com aplicações do mundo real, especialmente em segurança da informação e autenticação.

---

## Ferramentas Utilizadas

- **Qiskit:** framework principal para desenvolvimento quântico.
- **Matplotlib:** visualização de resultados (histogramas e gráficos).
- **IBM Quantum Platform:** execução e simulação em backends reais.
- **Google Colab:** ambiente interativo e colaborativo de aprendizado.

---

## Conclusão

Nosso projeto mostra que as chaves quânticas representam um dos primeiros passos concretos rumo à segurança digital absoluta.
Ao compreender suas bases físicas e aplicá-las em experimentos simulados, percebemos que essa tecnologia pode ser o futuro da comunicação segura e criptografia.

---

### Quem são os integrantes?

Nosso grupo é formado por profissionais e estagiários que atuam em diferentes áreas da IBM, unindo engenharia, arquitetura de soluções e inteligência artificial para explorar o potencial da computação e segurança quântica de forma aplicada e acessível.

- **Alberto Rubinho Peruchi**
*Platform Engineer Intern* na equipe de **Client Engineering – Ecosystem** da IBM.
Atua na construção e integração de produtos e plataformas escaláveis, com foco em automação, AI, cloud e arquitetura de infraestrutura.

Email: albertoperuchi@ibm.com

- **Giovani Kisz**
*Solution Architect* no **IBM Innovation Studio**.
Especialista em design de soluções inovadoras e arquitetura corporativa, trazendo a visão prática de como tecnologias emergentes podem ser aplicadas em ambientes empresariais reais.

Email: kisz@ibm.com

- **Guilherme Indiciate**
*AI Engineer Intern* na equipe de **Client Engineering – Ecosystem** da IBM.
Responsável pelo desenvolvimento de agentes de IA, microserviços e aplicações baseadas em modelos generativos, apoiando parceiros na integração dessas soluções em seus próprios sistemas.

Email: guilherme.indiciate@ibm.com

- **Rayara Amaro Figueiredo**
*AI Engineer Intern* na equipe de **Client Engineering – Ecosystem** da IBM.
Responsável pelo desenvolvimento de agentes de IA, microserviços e aplicações baseadas em modelos generativos, apoiando parceiros na integração dessas soluções em seus próprios sistemas.

Email: rayaraamaro@ibm.com

---