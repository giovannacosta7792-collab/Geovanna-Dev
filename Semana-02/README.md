Laborat-rio-de-Classifica-o-Visual
Laboratório de Classificação Visual

📌 Sobre o Projeto

Este projeto utiliza a plataforma Teachable Machine para demonstrar como modelos de Inteligência Artificial podem desenvolver vieses quando treinados com dados limitados e estereotipados.

O experimento evidencia como decisões automatizadas podem reproduzir discriminação, exclusão e interpretações incorretas da realidade devido à baixa diversidade nos dados utilizados durante o treinamento.

🎯 Objetivo

Treinar um modelo de classificação de imagens utilizando duas categorias:

Perfil Liderança Perfil Operacional

O objetivo é observar como a IA reage diante de pessoas que não seguem os padrões presentes no dataset inicial.

🧠 Desenvolvimento do Experimento 📂 Definição das Categorias

Foram criadas duas classes de classificação:

Categoria Critério Utilizado Perfil Liderança Pessoas utilizando roupas formais Perfil Operacional Pessoas utilizando roupas casuais 📸 Alimentação de Dados

O modelo recebeu:

Aproximadamente 20 imagens por categoria Capturas realizadas pela webcam Dados selecionados propositalmente de forma enviesada

O experimento demonstra como a limitação de diversidade interfere diretamente no comportamento da IA.

⚠️ Teste de Inferência

Após o treinamento, o modelo foi testado com pessoas que não correspondiam aos padrões utilizados no dataset.

Durante os testes, o sistema apresentou:

Falsos positivos Falsos negativos Classificações incorretas baseadas em aparência visual 🖼️ Evidência da Falha

Print do modelo realizando uma classificação incorreta devido ao viés dos dados de treinamento:

⚖️ Memorial de Impacto e Ética 🧩 Mecanismo do Viés

A seleção restrita de dados corrompe a lógica do algoritmo porque limita a diversidade das informações utilizadas durante o treinamento. O sistema aprende padrões superficiais e associa determinadas características visuais a funções específicas, desenvolvendo uma visão distorcida da realidade.

👥 Consequência Social

A classificação enviesada gera impactos emocionais e profissionais sobre indivíduos marginalizados pelo sistema. A pessoa pode sofrer exclusão, constrangimento e perda de oportunidades devido a interpretações incorretas feitas pela IA.

Além disso, modelos enviesados reforçam desigualdades sociais e preconceitos estruturais.

🛡️ Ação Mitigadora

Uma intervenção de Human-in-the-loop garante maior equidade durante a curadoria dos dados.

Revisores humanos analisam continuamente o dataset antes da implementação do modelo, verificando:

Diversidade Representatividade Possíveis padrões discriminatórios

Esse acompanhamento reduz vieses e aumenta a confiabilidade das decisões automatizadas.

🛠️ Tecnologias Utilizadas Teachable Machine Inteligência Artificial Machine Learning Classificação de Imagens Webcam 📚 Conclusão

O experimento demonstra que a qualidade e diversidade dos dados influenciam diretamente o comportamento da Inteligência Artificial.

Modelos treinados com informações enviesadas reproduzem discriminação e erros de interpretação, evidenciando a importância da supervisão humana e da responsabilidade ética no desenvolvimento de sistemas inteligentes.
