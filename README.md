# Vó Lila Gastrobar · site

Site estático de uma página (HTML, CSS e JavaScript puros), sem dependências de build. Pronto para subir no GitHub e publicar na Vercel.

## Estrutura

```
index.html      página principal (cardápio, sobre, avaliações, contato, dados estruturados)
styles.css      estilos responsivos (paleta preto e branco do logo)
script.js       abas do cardápio com navegação por teclado
assets/logo.jpg logo oficial
vercel.json     configuração de URLs limpas
robots.txt      regras para buscadores
sitemap.xml     mapa do site
```

## Rodar localmente

Basta abrir o `index.html` no navegador. Para testar como no servidor:

```
npx serve .
```

## Subir no GitHub

```
git init
git add .
git commit -m "Site inicial Vó Lila Gastrobar"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/vo-lila-site.git
git push -u origin main
```

## Publicar na Vercel

1. Em vercel.com, clique em "Add New > Project" e importe o repositório.
2. Framework preset: "Other". Não há comando de build nem pasta de saída.
3. Clique em Deploy.
4. Em Settings > Domains, adicione o domínio do cliente e siga as instruções de DNS.

## Antes de publicar: itens a confirmar

Estes pontos estão no PRD e precisam de resposta do dono:

- [ ] Trocar `SEU-DOMINIO.com.br` pelo domínio real em `index.html` (canonical, JSON-LD e imagem) e em `sitemap.xml` e `robots.txt`.
- [ ] Confirmar se o telefone (88) 99781-0603 é WhatsApp. Se não for, ajustar o link `wa.me`.
- [ ] Confirmar o endereço: "R." ou "Av." Monsenhor Frota, 673.
- [ ] Confirmar o horário (11:00 às 23:59, todos os dias).
- [ ] Conferir os preços da seção Cardápio com o Anota AI. Os valores foram lidos em 08/10/2026. Itens sem preço visível nos prints não aparecem no site.
- [ ] Confirmar o texto da seção Sobre com o dono. O texto atual é uma proposta.
- [ ] Confirmar a forma de pagamento e o que o espaço para eventos oferece.
- [ ] Confirmar autorização para usar as duas avaliações citadas (o texto é de avaliações públicas do Google).
- [ ] Confirmar que o Anota AI está ativo no horário comercial.

## Observações

- Os links para o Anota AI, o Instagram e o Google Maps estão diretos no HTML. Se o dono mudar de endereço de delivery, é preciso atualizar em três lugares: hero, cardápio e contato.
- O schema `Restaurant` no `<head>` precisa refletir exatamente o nome, o endereço e o telefone do GBP.
