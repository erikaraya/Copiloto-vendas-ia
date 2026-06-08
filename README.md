# 🚀 Copiloto de Vendas com IA - Salgaderia Sabor & Cia

Este repositório contém a estrutura e os prompts para um assistente de inteligência artificial desenhado para atuar como retaguarda e apoio para a equipe de atendimento e vendas de uma salgaderia.

---

## 📌 Perguntas do Projeto & Definições

### 1. Qual tema você escolheu?
O tema escolhido foi o setor de **Alimentação e Eventos**, focando especificamente no modelo de negócios de uma **Salgaderia (Sabor & Cia)**. O negócio atende tanto o cliente final (famílias organizando festas, estudantes e trabalhadores buscando um lanche rápido - B2C) quanto o mercado corporativo (buffets infantis e lanchonetes parceiras que compram salgados congelados em grande escala para revenda - B2B).

### 2. Qual problema o copiloto ajuda a resolver?
O copiloto resolve três gargalos principais no atendimento comercial:
*   **Demora no atendimento:** Centraliza as respostas para dúvidas frequentes (prazos, entregas, formatos), evitando que o vendedor perca tempo procurando tabelas de preços.
*   **Perda de vendas por objeções:** Municia o vendedor instantaneamente com argumentos técnicos de qualidade e estratégias de fechamento quando o cliente reclama do preço ou demonstra insegurança.
*   **Falta de proatividade (Próximo Passo):** Ajuda o vendedor a não deixar a conversa "morrer", sugerindo ganchos comerciais (perguntas simples, kits de degustação) para conduzir o cliente até o fechamento da compra.

### 3. Qual abordagem você usou (Chatbot, Copiloto ou Agente)?
Foi utilizada a abordagem de **Copiloto de Vendas**. 
*   **Por que essa escolha?** Em vez de colocar a IA para conversar diretamente com o cliente final (como um Chatbot tradicional de linha de frente), o modelo de Copiloto atua como um assistente de retaguarda para o atendente humano. Isso garante o "toque humano" na negociação, evita respostas robotizadas para o cliente e impede que a IA tome decisões erradas isoladamente, unindo a eficiência da automação com a segurança da supervisão humana.

### 4. Quais informações foram usadas?
A IA foi alimentada com uma estrutura de dados dividida em três pilares na pasta `knowledge/`:
*   `produtos.md`: Detalhes dos salgados fritos e assados, pesos (150g e 20g), preços de balcão e a política de descontos progressivos para parceiros B2B (atacado).
*   `perguntas-frequentes.md`: Regras de logística de entrega (raio de 10km), prazos de antecedência mínimos para pedidos de festa e formatos de envio (frito vs. congelado).
*   `objecoes.md`: Matriz de respostas para contornar reclamações de preço alto frente à concorrência, medo do produto chegar frio ou insegurança de novos revendedores.

### 5. Um exemplo de conversa ou resposta gerada
*   **Entrada enviada pelo vendedor à IA:** *"O dono de uma lanchonete achou o cento de R$ 90,00 muito caro e disse que no concorrente é R$ 70,00."*
*   **Resposta gerada pelo Copiloto (Retorno da IA):**
    > **Análise:** Objeção de preço no setor B2B. Aplicar desconto por volume ou focar na conversão com teste.
    >
    > **Sugestão de Resposta (Copiar/Colar):** *"Entendo perfeitamente a sua preocupação com o custo, afinal, comércio precisa de margem! O nosso diferencial é que usamos produtos de primeira linha (como Catupiry original), o que fideliza muito o cliente. Mas olha, para parcerias com lanchonetes, se você pedir acima de 5 centos por semana, conseguimos fazer o cento congelado a R$ 75,00! Que tal fazermos um kit degustação essa semana a preço de custo para você testar com seus clientes?"*
    >
    > **Próximo Passo:** Tentar fechar o kit degustação para ele comprovar a qualidade sem riscos.

### 6. Possíveis melhorias futuras
Para as próximas versões do projeto, mapeamos as seguintes evoluções:
1.  **Calculadora Automática de Centos:** Integrar uma função onde o copiloto calcula automaticamente a quantidade exata de salgados com base no número de adultos e crianças que o vendedor informar.
2.  **Integração com API de CRM (ex: Hubspot/Pipefy):** Permitir que o copiloto puxe o histórico de compras anteriores daquele cliente para sugerir os sabores favoritos dele.
3.  **Módulo de Agente Autônomo (`AGENTS.md`):** Evoluir a abordagem para um Agente capaz de checar em tempo real a planilha de produção da cozinha para saber quais sabores de salgados estão disponíveis imediatamente para pronta-entrega.