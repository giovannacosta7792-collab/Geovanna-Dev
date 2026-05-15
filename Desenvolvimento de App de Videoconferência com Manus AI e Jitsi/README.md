# 📱 DevMentor Live - Videoconferência e Mentoria Técnica com IA

O **DevMentor Live** é uma aplicação mobile nativa para o ecossistema Android, projetada especificamente para conectar desenvolvedores em início de carreira a mentores experientes. Mais do que uma plataforma de comunicação, o aplicativo resolve uma das maiores dores do ensino de programação: a dificuldade que programadores iniciantes têm para articular problemas técnicos complexos e a escassez de feedback estruturado em tempo real.

Através de uma arquitetura robusta, o aplicativo combina chamadas de vídeo de baixa latência com uma camada de inteligência artificial especializada em análise de código (Code Review), transformando videoconferências tradicionais em sessões de mentoria altamente produtivas e interativas.

---

## 🎯 Proposta de Valor e Problema Resolvido

No cenário atual da engenharia de software, o aprendizado assíncrono ou a busca por respostas em fóruns muitas vezes falha devido à incapacidade do estudante de formular a pergunta correta. O DevMentor Live atua diretamente nessa fricção:
- **Pontes de Comunicação:** Permite que o mentor e o mentorado analisem o mesmo trecho de código simultaneamente durante a chamada.
- **Análise Preditiva e Sugestões:** A IA integrada atua como um terceiro participante neutro, gerando documentação instantânea, apontando refatorações e sugerindo melhorias de clean code enquanto a conversa acontece.

---

## 🛠️ Stack Técnica e Arquitetura Mobile

A engenharia do aplicativo foi estruturada utilizando padrões modernos de desenvolvimento para a plataforma Android, garantindo escalabilidade, modularidade e performance:

- **Linguagem Principal:** Kotlin, utilizando coroutines e fluxos (Flow) para gerenciamento de concorrência e operações assíncronas de rede.
- **Ambiente de Desenvolvimento:** Android Studio (Bumblebee ou superior), aplicando o Gradle como sistema de automação de build.
- **Infraestrutura de Vídeo:** SDK do Jitsi Meet, encapsulado para gerenciar salas dinâmicas, streaming de mídia ponto a ponto (P2P) e criptografia de ponta a ponta.
- **Motor de Inteligência Artificial:** Integração com a IA Manus, atuando no processamento de linguagem natural (NLP) e na análise semântica de sintaxe de código fonte durante as sessões.

---

## 📲 Funcionalidades Escaláveis (Features)

### 1. Sistema de Videoconferência Nativo
Integração customizada do Jitsi Meet SDK, permitindo salas privadas de mentoria com controle de áudio, vídeo, partilha de ecrã e chat persistente. A interface foi adaptada para manter o foco visual no código compartilhado.

### 2. Copilot de Mentoria (IA Manus)
Uma barra lateral interativa onde o estudante pode colar trechos de código (ou o mentor pode capturar via tela). A IA analisa o bloco e gera de imediato:
- Diagnóstico de bugs e exceções comuns.
- Sugestões de melhorias de performance e segurança.
- Links para documentações oficiais baseadas na tecnologia discutida.

### 3. Agendamento e Matching Inteligente
Módulo para listagem de mentores disponíveis por Stack (Ex: Mobile, Front-end, Back-end) e agendamento de horários integrados ao calendário nativo do dispositivo Android.

---

## 📂 Modelagem Conceitual da Aplicação

O fluxo de dados do aplicativo é baseado em princípios de arquitetura limpa (Clean Architecture), dividindo-se em camadas de Apresentação (UI), Domínio (Regras de Negócio) e Dados (Repositórios e SDKs):

- **Camada de Apresentação:** Utiliza o padrão MVVM (Model-View-ViewModel) para isolar o estado da interface de usuário dos ciclos de vida do Android.
- **Gerenciamento de Estado:** LiveData/StateFlow observando as mudanças de status da chamada de vídeo e das requisições de IA.
- **Segurança e Tokenização:** Autenticação via tokens JWT para garantir que apenas usuários autorizados tenham acesso às salas de videoconferência privadas criadas dinamicamente.

---

## ⚙️ Diretrizes para Execução Local

Para compilar e rodar o projeto localmente no Android Studio, siga os passos abaixo:

1. **Clonar o Repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/devmentor-live.git](https://github.com/seu-usuario/devmentor-live.git)
