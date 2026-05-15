Vou expandir e profissionalizar a documentação do seu projeto OrçaPro. Para atingir a densidade de 2.500 caracteres, estruturei o texto focando em Engenharia de Software No-Code, princípios de Clean App no Bubble.io, modelagem de dados e usabilidade.

Aqui está o conteúdo completo para o seu README.md:

Markdown
# 📑 OrçaPro - Gestão Comercial e Engenharia de Software com Bubble.io

O **OrçaPro** é uma solução avançada de SaaS (Software as a Service) desenvolvida para otimizar a gestão comercial de profissionais autônomos e empresas. O foco central do projeto é a centralização da governança de dados, automação de fluxos de venda e a entrega de uma experiência de utilizador (UX) que minimize a fricção operacional no ciclo de vida de um orçamento.

Este projeto foi concebido sob os princípios da **Engenharia de Software No-Code**, utilizando a plataforma **Bubble.io** para implementar uma arquitetura relacional robusta, fluxos de trabalho (workflows) otimizados e camadas de segurança de nível empresarial.

---

## 🚀 Funcionalidades Estratégicas

### 1. Dashboard de Business Intelligence (BI)
Diferente de listas simples, o OrçaPro oferece um painel analítico que traduz dados brutos em inteligência de negócio. Através de grupos de dados dinâmicos, o utilizador visualiza instantaneamente a saúde financeira:
- **Indicadores de Performance:** Volume total de orçamentos vs. taxa de conversão (aprovados).
- **Controle de Pipeline:** Monitorização de propostas em estado de rascunho, enviadas e aguardando retorno.

### 2. Ecossistema de Gestão de Propostas
O núcleo da aplicação permite o registo detalhado de cada serviço, incluindo títulos semânticos, valores monetários com formatação dinâmica e prazos de validade automáticos para evitar perdas contratuais.

### 3. Governança de Clientes e CRM
Um banco de dados estruturado para garantir a integridade da informação. Inclui validação de campos obrigatórios (como CNPJ/NIF) e máscaras de input para assegurar que os dados de contacto corporativo estejam sempre prontos para uso em comunicações automáticas.

### 4. Fluxo de Estados (Finite State Machine)
A lógica da aplicação é baseada num sistema visual de estados. Cada orçamento percorre uma jornada lógica:
**Rascunho** → **Enviado** → **Aprovado** ou **Recusado**.
Esta transição é gerida por workflows que garantem que nenhuma proposta "se perca" no processo comercial.

---

## 🛠️ Stack Técnica e Arquitetura de Sistemas

A implementação técnica afasta-se do amadorismo "drag-and-drop", focando em escalabilidade:

- **Plataforma:** Bubble.io (Engine de execução de lógica e interface).
- **Base de Dados:** Estrutura relacional otimizada com normalização de dados para evitar redundância.
- **Lógica de Back-end:** Workflows configurados com foco em performance (Single Page Application - SPA), utilizando estados customizados para reduzir o carregamento do servidor.
- **Design System:** Implementado via estilos globais, garantindo consistência visual em todos os módulos do sistema.

---

## 📂 Modelagem de Dados (Data Engineering)

A arquitetura lógica foi desenhada para suportar relacionamentos complexos:

| Objeto de Dado | Campo Principal | Tipo | Descrição Técnica |
| :--- | :--- | :--- | :--- |
| **User** | Nome / Empresa | `Text` | Identidade do Tenant (Organização). |
| **Cliente** | CNPJ / NIF | `Text` | Chave única para validação fiscal e governança. |
| **Orçamento** | Status | `Option Set` | Atributo estático para alta performance em filtros. |
| **Orçamento** | Valor Total | `Number` | Campo numérico para cálculos agregados no Dashboard. |
| **Relacionamento** | Link Cliente | `Relational` | Vinculação entre a tabela de Orçamentos e Clientes. |

---

## 🔒 Segurança, Privacidade e LGPD/RGPD

Seguindo as melhores práticas de Engenharia de Software, o OrçaPro não expõe dados sensíveis no lado do cliente (Client-side):

1. **Privacy Rules:** Regras aplicadas diretamente no servidor. Um utilizador nunca terá acesso aos orçamentos de outra organização, mesmo que tente manipular o DOM da aplicação.
2. **Condicionais de Acesso:** Grupos e elementos visuais possuem regras de visibilidade baseadas no estado `Current User is Logged In`.
3. **Prevenção de Injeção:** Como o Bubble gere a base de dados de forma encapsulada, o sistema é nativamente protegido contra SQL Injection.
4. **Data Integrity:** O uso de *Auto-binding* é restrito e monitorizado para evitar alterações acidentais em campos críticos de faturamento.

---

## ⚙️ Implementação e Utilização

Por ser uma aplicação nativa na nuvem, o OrçaPro elimina barreiras de entrada técnica:

1. **Acesso:** Disponível via navegador (Web-based).
2. **Autenticação:** Sistema de login seguro com encriptação de palavras-passe.
3. **Operação:**
   - Utilize o botão **+ Novo Orçamento** para instanciar um novo registo na base de dados.
   - O sistema calculará automaticamente as métricas no Dashboard assim que o status for alterado.

---

## ✒️ Considerações Académicas

Este projeto integra o portfólio de estudos em **Análise e Desenvolvimento de Sist
