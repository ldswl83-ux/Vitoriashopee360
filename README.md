# Lara Shopee 360 — Android

MVP Android para encontrar produtos da Shopee por:
- Mais vendidos
- Maior comissão
- Top performance
- Palavra-chave
- Comissão mínima

A tela mostra preço, vendas, comissão total, comissão do vendedor, comissão Shopee, loja e link de oferta.

## Importante
A Shopee disponibiliza a Open API de Afiliados. Para consultar dados reais, é necessário ter acesso à API e usar App ID + App Secret da sua conta. O app pede essas credenciais na tela Configurações e guarda-as apenas no armazenamento privado do aplicativo.

Endpoint usado:
https://open-api.affiliate.shopee.com.br/graphql

A autenticação é feita por assinatura SHA-256 conforme a documentação pública disponível.

## Como abrir
1. Instale o Android Studio.
2. Abra a pasta `larashopee360`.
3. Espere o Gradle sincronizar.
4. Rode no celular Android.
5. Abra Configurações e informe App ID e App Secret.
6. Escolha um modo e toque em "Buscar produtos".

## Observação de segurança
Para um aplicativo publicado na Play Store, o ideal é mover o App Secret para um backend próprio, em vez de mantê-lo no celular. Este MVP é pensado para uso pessoal/teste.

## Recursos desta versão
- índice de oportunidade de 0 a 100, calculado localmente a partir de vendas, comissão, avaliação e faixa de preço;
- botão ROBÔ SHOPEE para gerar roteiro, gancho, legenda e hashtags e compartilhar o texto;
- abrir produto e compartilhar oferta;
- filtros de mais vendidos, maior comissão e top performance;
- filtro por comissão mínima.

## Próximas evoluções
- favoritos e histórico persistentes;
- alertas de produtos que cruzarem uma comissão definida;
- filtros por categoria, preço e volume de vendas;
- geração automática de título, frase para tela e prompt de até 900 caracteres;
- painel diário com novos produtos e variações de comissão.
