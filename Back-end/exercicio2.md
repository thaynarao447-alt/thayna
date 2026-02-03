**1.** O que é o **Node.js**?
Explique sua finalidade e por que ele é considerado um ambiente de execução e não uma linguagem de programação.
 Node.js é um ambiente de execução (runtime environment) de código aberto e multiplataforma, construído sobre o motor V8 JavaScript do Google Chrome.A principal finalidade do Node.js é permitir o desenvolvimento de aplicações de rede, servidores web e APIs (Application Programming Interfaces) rápidas e escaláveis, utilizando JavaScript em ambos os lados (frontend e backend). 

---

**2.** Qual a diferença entre **Node.js** e **JavaScript executado no navegador**?
Cite pelo menos **duas diferenças**.
Enquanto o JavaScript no navegador foca na interface do usuário (frontend), o Node.js é usado para criar aplicações de servidor (backend). 

---

**3.** O que é o **V8 Engine** e qual sua importância para o funcionamento do Node.js?
é um motor de JavaScript (JavaScript engine) de alto desempenho, de código aberto, desenvolvido pelo Google em C++

---

**4.** Explique o conceito de **I/O não bloqueante** no Node.js.
Por que isso melhora o desempenho de aplicações?
O I/O (Input/Output - Entrada/Saída) não bloqueante no Node.js é um modelo de execução onde as operações que envolvem leitura de arquivos, consultas a banco de dados ou requisições de rede não travam a thread principal (o "processo principal") enquanto aguardam a conclusão. 

---

**5.** O que é o **Event Loop**?
Descreva, de forma resumida, como ele funciona.
O Event Loop (Loop de Eventos) é o mecanismo central do JavaScript (tanto no navegador quanto no Node.js) responsável por gerenciar a execução de código assíncrono, permitindo que a linguagem seja "não bloqueante" (non-blocking), mesmo sendo single-threaded (executa uma coisa de cada vez). 

---

**6.** O que são **módulos** no Node.js?
Explique a diferença entre:

* Módulos internos
* Módulos externos
* Módulos criados pelo desenvolvedor
* 1. Módulos Internos (ou Core Modules) 
São módulos nativos que vêm incorporados ao próprio ambiente de execução do Node.js no momento da instalação. Eles oferecem as funcionalidades essenciais para o servidor (sistema de arquivos, rede, etc.).
2. Módulos Externos (ou Third-party Modules)
São bibliotecas criadas pela comunidade ou por terceiros e disponibilizadas através do repositório npm (Node Package Manager). Eles estendem as capacidades da aplicação além do que o Node.js nativo oferece.
3. Módulos criados pelo desenvolvedor (ou Local Modules) 
São arquivos JavaScript criados por você dentro da sua própria aplicação para organizar a lógica de negócios, separar responsabilidades e reutilizar código localmente. 

**7.** Para que serve o arquivo **package.json** em um projeto Node.js?
Cite pelo menos **três informações** que ele pode conter.
O arquivo package.json é fundamental em projetos Node.js, servindo como o manifesto ou coração do projeto 

---

**8.** O que é o **npm**?
Explique sua função no desenvolvimento de aplicações Node.js.
é o gerenciador de pacotes padrão para o ambiente de execução Node.js e o maior registro de software de código aberto do mundo

---

**9.** O que é uma **API REST** e como o Node.js pode ser usado para desenvolvê-la?
Uma API REST (Representational State Transfer) é um estilo arquitetural para projetar aplicações em rede que utiliza o protocolo HTTP para permitir que sistemas diferentes troquem informações, como um front-end web e um banco de dados. Ela é baseada em recursos (identificados por URIs) e métodos HTTP (GET, POST, PUT, DELETE) para realizar operações, sendo amplamente adotada por sua escalabilidade, flexibilidade e uso leve. 

---

**10.** Cite **duas vantagens** e **duas desvantagens** do uso do Node.js em aplicações web.
Vantagens
Alta Performance e Escalabilidade (I/O não bloqueante): O Node.js utiliza um modelo de E/S (entrada/saída) orientado a eventos e não bloqueante, o que o torna extremamente eficiente e rápido, especialmente para aplicações em tempo real (como chats e streaming) e sistemas que lidam com muitas conexões simultâneas.
Uso de Linguagem Única (Full-Stack JS): Permite que desenvolvedores utilizem JavaScript tanto no front-end quanto no back-end. Isso simplifica o desenvolvimento, facilita o compartilhamento de código entre as camadas e reduz a necessidade de duas equipes especializadas em linguagens diferentes. 
Desvantagens
Desempenho Ruim em Tarefas de CPU Intensa: Como o Node.js roda em uma única thread, cálculos pesados (processamento de imagem, vídeo, criptografia pesada) bloqueiam o "event loop", o que atrasa todas as outras requisições e degrada o desempenho.
Complexidade da Programação Assíncrona (Callback Hell): A dependência intensa de callbacks para lidar com assincronismo pode tornar o código difícil de ler, manter e depurar, resultando no conhecido "callback hell" (ou "pirâmide do destino"), embora o uso de Promises e Async/Await ajude a mitigar esse problema. 

---
