# Port-scanner-py
Port scanner de IPs, simples e pratico com relatório
Scanner TCP com Python Socket

Scanner de portas TCP desenvolvido em Python utilizando apenas sockets nativos, com interface gráfica em Tkinter, multithreading, banner grabbing e geração de relatório em PDF.

Funcionalidades

✔ Scanner TCP usando socket
✔ Interface gráfica simples com Tkinter
✔ Varredura de range de portas
✔ Multithreading para maior velocidade
✔ Detecção de portas abertas/fechadas
✔ Identificação de serviço padrão da porta
✔ Banner grabbing
✔ Exportação TXT/CSV
✔ Geração de relatório PDF
✔ Timeout configurável
✔ Exibição do tempo total da varredura

Tecnologias Utilizadas
Python 3
Socket
Tkinter
concurrent.futures
ReportLab
Estrutura do Projeto
scanner-portas/
│
├── port-scanner.py
├── README.md
└── requirements.txt
Instalação

Clone o repositório:

git clone https://github.com/SEU-USUARIO/scanner-portas.git

Entre na pasta:

cd scanner-portas

Instale as dependências:

pip install reportlab
Execução

Execute o programa:

python port-scanner.py
Como Funciona

O scanner realiza conexões TCP utilizando o método:

socket.connect_ex()

Durante a conexão ocorre o processo do TCP Three-Way Handshake:

SYN → SYN/ACK → ACK

Se a conexão for aceita:

a porta é considerada aberta
o serviço é identificado
o banner pode ser capturado
Interface

O sistema possui:

Campo para IP alvo
Porta inicial
Porta final
Botão de varredura
Exportação TXT/CSV
Geração de PDF
Tabela em tempo real
Relatório PDF

O programa gera automaticamente um relatório contendo:

IP escaneado
portas abertas
serviços identificados
banners capturados
Exemplo de Uso
IP: 172.16.32.53
Porta Inicial: 1
Porta Final: 1000

Resultado esperado:

22/tcp  ABERTA  ssh
80/tcp  ABERTA  http
3306/tcp ABERTA mysql
Objetivo Acadêmico

Projeto desenvolvido para fins educacionais em estudos de:

Redes de Computadores
Cybersecurity
Enumeração de Serviços
TCP/IP
Programação em Python
Autor

Rafael Benjamin Aquino Silva

Licença

Projeto para fins educacionais.
