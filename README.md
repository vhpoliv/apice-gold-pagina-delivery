# Página de delivery · Ápice Gold Digital

Página pronta para captar donos de delivery (hamburgueria, pizzaria, açaí, marmitaria). É HTML puro: não precisa de WordPress, plugin nem construtor de página.

## O que tem aqui

- `site/`: a página pronta. `index.html` + as pastas `img/` e `fonts/`. Mantenha as três juntas.
- `material-em-alta/`: as fotos em tamanho original (comida, cozinha, motoboy, suas fotos e o logo), para usar em anúncio, post ou story.

## Como colocar no ar

**Opção 1: subpasta do seu site (Hostinger ou outra hospedagem)**
1. Abra o Gerenciador de Arquivos da hospedagem e entre em `public_html`.
2. Crie a pasta `delivery`.
3. Envie para dentro dela o `index.html` e as pastas `img` e `fonts`.
4. A página fica em `apicegolddigital.com.br/delivery`.

**Opção 2: grátis, em 2 minutos**
Arraste a pasta `site` para https://app.netlify.com/drop. Sai um endereço na hora, que depois pode virar um subdomínio seu.

## Ligar o formulário no seu CRM

Hoje, quando a pessoa termina a comanda, abre o seu WhatsApp com as respostas prontas.
Para cair direto no seu CRM (GHL, RD, n8n ou outro), abra o `index.html` num editor de texto, procure por:

```
var ENDPOINT=''
```

e cole entre as aspas o endereço de webhook do seu CRM. Ele recebe: tipo de delivery, pedidos por dia, canal, o que mais pesa, nome, nome do delivery, cidade e WhatsApp.

## Antes de publicar, confira

- Os números do painel ("412 mensagens", "R$ 13,9 mil") e das notas fiscais são **exemplo**, e a página diz isso. Se tiver um case real de delivery, ele pode entrar no lugar.
- O link "Política de privacidade" no rodapé está vazio (`href="#"`). Aponte para a sua política.
- Pixel da Meta e Google Tag: cole no `<head>` do `index.html`.

Feito pela Regência.
