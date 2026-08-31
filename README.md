# Augusto Digital — sistema pessoal gratuito

Esta é uma primeira versão web, responsiva, feita para uso pessoal da Alice na Augusto Estamparia Digital.

## O que já funciona
- Dashboard de vendas e comissão
- Clientes
- Novo pedido
- Várias estampas por pedido
- Imagem + tecido + quantidade por item
- Galeria reutilizável de imagens, sem códigos de estampas
- Total de peças automático
- Status do pedido
- Sinal recebido, valor total, saldo e comissão de 1%
- Fechamento financeiro no mês em que o valor total é informado
- Geração de PDF do pedido
- Backup/importação em JSON
- Identidade visual azul/dourado e logo da Augusto

## Regra financeira
A comissão é sempre 1% do VALOR TOTAL do pedido. O sinal não é descontado da base da comissão; ele só reduz o saldo a receber.

A venda entra no mês em que o campo "Valor total do pedido" é preenchido.

## Importante sobre a versão gratuita
Esta versão usa armazenamento do navegador (localStorage) para manter os dados. Isso é ótimo para começar sem servidor/banco de dados, mas os dados não sincronizam automaticamente entre computador e celular.

Use a área "Backup" regularmente para exportar uma cópia.

## Como colocar online de graça
1. Crie uma conta no GitHub.
2. Crie um repositório novo, por exemplo `augusto-digital`.
3. Envie `index.html` e `logo.jpg`.
4. No repositório, abra Settings > Pages.
5. Em "Build and deployment", selecione "Deploy from a branch", escolha `main` e a pasta `/root`.
6. Salve e aguarde o GitHub Pages publicar.
7. O GitHub fornecerá um endereço `https://SEUUSUARIO.github.io/augusto-digital/`.

Também pode ser hospedado em serviços de páginas estáticas que aceitem upload do arquivo.

## Segurança
A senha inicial da versão demonstrativa é a mesma que foi usada no protótipo do Emergent. Como esta é uma aplicação estática, essa senha é apenas uma barreira de interface e NÃO deve ser considerada segurança de nível bancário. Para dados realmente sensíveis, a próxima versão deve usar autenticação e banco de dados no servidor (por exemplo, Supabase).
