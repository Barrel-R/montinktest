Projeto Montink

Projeto de backend com frontend básico para gerenciar produtos, estoques, cupons e pedidos, com regras específicas de frete e integração com ViaCEP. Desenvolvido como solução para processo seletivo.

🧰 Tecnologias Utilizadas
Backend: PHP

Frontend: HTML / JS / Bootstrap

Banco de Dados: MySQL 

API externa: ViaCEP

Email: Mailtrap (para testes)

Webhooks: Endpoint público ou ngrok para testes locais

✅ Funcionalidades
CRUD de produtos, com controle de variações e estoque

Tela única para:

Cadastro e edição de produtos

Controle de estoque por variação

Ação de compra com gerenciamento de carrinho

Cálculo de frete baseado no subtotal:

R$20,00 padrão

R$15,00 entre R$52,00 e R$166,59

Grátis acima de R$200,00

Consulta de CEP via API ViaCEP

Criação e validação de cupons com regras de mínimo e validade

Envio de e-mail com os dados do pedido finalizado

Webhook para alteração de status do pedido (ou exclusão se for cancelado)

🗂️ Estrutura de Banco de Dados
Produtos: nome, preço base

Variações: cor, tamanho etc. (opcional)

Estoque: relação com produtos/variações, quantidade disponível

Pedidos: subtotal, frete, total, status, endereço

Cupons: código, valor de desconto, validade, mínimo

📬 Como Rodar Localmente
```
git clone https://github.com/Barrel-R/montinktest

cd montinktest
```

# Configure o ambiente
```
cp .env.example .env
```

# Inicie o servidor


📌 Considerações Finais
O foco foi manter o projeto simples, funcional e com boa manutenção

Todas as regras de negócio e integrações estão documentadas no código

A lógica foi separada em camadas (MVC) respeitando boas práticas
