# 🌊 Simulador Interativo de Fenômenos Ondulatórios

Este projeto é uma aplicação web interativa desenvolvida para demonstração acadêmica de física ondulatória. O objetivo é ilustrar de forma visual, acústica e física os conceitos de **ondas senoidais**, **princípio da superposição**, **interferência construtiva/destrutiva** e o **efeito de batimento**.

O projeto combina simulações digitais em tempo real com experimentos físicos integrados (demonstração com cordas e um circuito com Arduino).

---

## 🖥️ Módulos do Projeto

O sistema conta com um **Painel de Controle Central (Menu)** com estética futurista que dá acesso a três módulos independentes:

1. **Módulo 01: Ondas Senoidais e Arduino (`ondassom.html`)**
   - Gráfico dinâmico que mostra duas ondas independentes e a sua onda resultante (soma matemática).
   - Integração com a *Web Audio API* para emitir o som vivo da onda de forma sônica.
   - **Integração Física:** Projetado para interagir com uma caixinha de som externa ligada a um módulo de microfone e LED no Arduino, fazendo com que o circuito físico brilhe forte com interferência construtiva e apague em silêncio absoluto (interferência destrutiva).

2. **Módulo 02: Acelerador de Batimento Acústico (`AceleradorAcustico.html`)**
   - Focado exclusivamente no fenômeno de batimento acústico.
   - Utiliza controles giratórios (*knobs*) analógicos customizados via código para sintonizar frequências ligeiramente desalinhadas (ex: 440 Hz e 442 Hz).
   - Mostra graficamente os "pacotes de energia" sendo criados enquanto o usuário ouve o volume oscilar ritmicamente no tempo.
   - Inclui um botão de parada total de emergência para silêncio absoluto instantâneo.

3. **Módulo 03: Cuba de Ondas Bidimensional (`ondas.html`)**
   - Expansão do conceito de interferência de uma dimensão (cordas) para duas dimensões (2D).
   - Simula uma cuba d'água digital onde o usuário pode clicar na tela para criar fontes de gotas concêntricas.
   - Demonstra de forma gráfica as franjas de interferência (Experimento de Young), evidenciando as linhas de nós (calmaria/interferência destrutiva) e as cristas brilhantes (interferência construtiva).

---

## 🎛️ Aparato Físico Integrado

Para validar os conceitos matemáticos simulados nas telas, a apresentação utiliza:
- **Demonstração Espacial com Cordas:** Uma corda náutica elástica para demonstrar fisicamente a criação de cristas, vales e o ponto fixo de anulação ("nó") em uma dimensão.
- **Hardware Arduino:** Circuito composto por um Arduino, módulo de microfone (captador de intensidade sonora) e um LED de alto brilho para materializar a variação da amplitude da onda resultante em estímulo luminoso.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** (Estruturação e elementos de controle de alcance)
- **CSS3** (Estilização responsiva e interface escura inspirada em terminais cibernéticos)
- **JavaScript Vanila** (Cálculos trigonométricos senoidais e renderização baseada em tempo)
- **HTML5 Canvas API** (Renderização gráfica de alta performance ponto a ponto)
- **Web Audio API** (Geração e modulação de sintetizadores de áudio nativos no navegador)

---

## 🚀 Como Executar

1. Clone o repositório em sua máquina:
   ```bash
   git clone https://github.com
   ```
2. Abra a pasta do projeto.
3. Execute o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox ou Opera).
4. Certifique-se de dar permissão de áudio ao navegador e clique em **Iniciar Acelerador** ou **Ligar Áudio Vivo** para ativar a emissão sonora.
