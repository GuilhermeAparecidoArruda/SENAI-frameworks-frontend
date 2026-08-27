## Aula 02 - Configuração do Ambiente de Desenvolvimento

**Objetivo da Aula:** 
Capacitar o aluno a preparar um ambiente de desenvolvimento profissional, compreendendo a importância do controle de versão, o uso de ferramentas essenciais (linha de comando, IDEs, gerenciadores de pacotes) e o fluxo inicial de criação e deploy de uma aplicação web.

---

**Resumo dos Tópicos:**
* **Controle de Versão vs. Backup Tradicional:** Diferente de um backup comum, que apenas salva o estado atual dos arquivos, o versionamento atua como uma máquina do tempo para o projeto. Ele registra um histórico completo detalhando quem fez a alteração, o que foi modificado e quando ocorreu, o que é fundamental para equipes trabalharem simultaneamente no mesmo código sem gerar conflitos.
* **Versionamento Semântico (SemVer):** Para organizar as atualizações de software, utiliza-se o padrão MAJOR.MINOR.PATCH (por exemplo, versão 2.1.3). O número MAJOR muda quando há quebras de compatibilidade, o MINOR quando novas funcionalidades são adicionadas sem quebrar o que já existe, e o PATCH é reservado para pequenas correções de bugs.

* **Boas Práticas com Git:** O Git é a ferramenta padrão de linha de comando para esse controle. A aula reforçou práticas como fazer commits pequenos e focados, escrever mensagens claras e utilizar *branches* (ramificações) para desenvolver novas funcionalidades isoladas e *tags* para marcar versões de lançamento.

* **Ecossistema de Ferramentas:** O ambiente do desenvolvedor moderno exige boas ferramentas. O Visual Studio Code foi apresentado como a IDE principal. O Node.js foi introduzido como o ambiente que permite executar JavaScript fora do navegador (no servidor), e o NPM (Node Package Manager) como o gerenciador essencial para instalar e atualizar bibliotecas de terceiros.

* **Início com React e Deploy:** A aula culminou na prática, demonstrando como inicializar um projeto React rapidamente usando o pacote `create-react-app`. Em seguida, foi mostrado como colocar essa aplicação no ar (deploy contínuo) de forma acessível utilizando a plataforma de hospedagem Vercel.

---

**Conclusão da Aula:** 
O domínio das ferramentas de base, como Git, Node.js e plataformas de hospedagem em nuvem, é o primeiro passo essencial para qualquer desenvolvedor. Compreender e configurar corretamente esse ecossistema garante um fluxo de trabalho seguro, colaborativo, escalável e alinhado com as exigências e boas práticas do mercado de tecnologia.