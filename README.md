# 🌟 Sistema de Pontos Semanal

![Visão Geral da Aplicação](https://i.imgur.com/8a6zXfF.png )

## 🎯 Sobre o Projeto

Este projeto é uma aplicação web interativa e em tempo real para gerenciar um sistema semanal de pontos e recompensas, para as pequenas tarefas domésticas do meu filho. 
Ele foi desenvolvido para ser uma solução prática, 
multi-usuário e *serverless*, eliminando a necessidade de um backend tradicional.

A aplicação permite que usuários "editores" (pais) marquem tarefas e preencham campos, com os dados sendo salvos e sincronizados instantaneamente para 
todos os clientes conectados. Um modo de "apenas leitura" também está disponível para usuários específicos (filho).

---

## 🚀 Arquitetura e Tecnologias Utilizadas

A solução foi construída com uma abordagem 100% *serverless*, utilizando as seguintes tecnologias:

*   **Front-End:** HTML5, CSS3, JavaScript (Vanilla)
*   **Banco de Dados Real-Time:** [Firebase Realtime Database](https://firebase.google.com/products/realtime-database )
*   **Hospedagem & Deploy:** [Netlify](https://www.netlify.com/ )

![Diagrama de Arquitetura](https://i.imgur.com/JjYv2eK.png )

---

## ✨ Funcionalidades Principais

*   **Sincronização em Tempo Real:** Alterações feitas por um usuário são refletidas instantaneamente para todos os outros.
*   **Persistência de Dados:** Os dados do formulário são armazenados na nuvem (Firebase) e persistem entre sessões.
*   **Controle de Acesso por URL:**
    *   **Modo Edição:** Acesso padrão, permite alterar todos os dados.
    *   **Modo Leitura:** Ativado via parâmetro de URL (`/?user=filho`), desabilita todos os campos para visualização.
*   **Salvamento Automático:** Não há botão "Salvar". Todas as mudanças são salvas automaticamente.
*   **Controles Administrativos:** Um botão para "Limpar a Semana" está disponível apenas para usuários no modo de edição.

---


