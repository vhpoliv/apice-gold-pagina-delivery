# Página de delivery · Ápice Gold Digital

Página pronta para captar donos de delivery (hamburgueria, pizzaria, açaí, marmitaria). É HTML puro: não precisa de WordPress, plugin nem construtor. Não mexe no seu site atual.

## O que tem aqui

- `site/`: a página pronta. `index.html` + as pastas `img/` e `fonts/`. As três ficam sempre juntas.
- `site.zip`: a mesma pasta compactada, para subir de uma vez.
- `material-em-alta/`: as fotos em tamanho original (comida, cozinha, motoboy, suas fotos e o logo), para anúncio, post e story.

## Colocar no ar em delivery.apicegolddigital.com.br (Hostinger, 5 minutos)

**1. Criar o subdomínio**
1. Entre no hPanel da Hostinger e abra **Sites > apicegolddigital.com.br > Painel**.
2. No menu lateral, vá em **Domínios > Subdomínios**.
3. Digite `delivery` e clique em **Criar**. A pasta fica `public_html/delivery`. Pode deixar assim.

**2. Subir a página**
1. No menu lateral, abra **Arquivos > Gerenciador de Arquivos** e entre em `public_html/delivery`.
2. Clique no ícone de **Upload** e envie o arquivo `site.zip`.
3. Clique com o botão direito no `site.zip` > **Extrair**. Confira se o `index.html` ficou direto dentro de `delivery`, e não numa subpasta.
4. Apague o `site.zip`.

**3. Ligar o SSL**
Em **Segurança > SSL**, confira se `delivery.apicegolddigital.com.br` aparece como ativo. Se não aparecer, clique em **Instalar SSL** e escolha o subdomínio. Em alguns minutos a página abre com cadeado.

Pronto: https://delivery.apicegolddigital.com.br

> Se o subdomínio não abrir: o DNS do domínio precisa estar apontado para a Hostinger. Hoje ele aponta para servidores da HostGator (ns1058/ns1059.hostgator.com.br). Se o site principal ainda está na HostGator, crie o subdomínio lá, no cPanel, com os mesmos passos (Domínios > Subdomínios, Gerenciador de Arquivos, SSL/TLS Status > Run AutoSSL).

## Página privada até você aprovar

A página sobe **escondida do Google** (tem `noindex` no topo do `index.html`). Só entra quem tiver o link, então você pode revisar com calma e mandar para quem quiser.
Quando aprovar e for anunciar, apague esta linha do `index.html`:

```
<meta name="robots" content="noindex,nofollow">
```

## Ligar o formulário no seu CRM

Hoje, quando a pessoa termina a comanda, abre o seu WhatsApp com as respostas prontas.
Para cair direto no seu CRM (GHL, RD, n8n ou outro), abra o `index.html` no editor do Gerenciador de Arquivos e procure por:

```
var ENDPOINT=''
```

Cole entre as aspas o endereço de webhook do seu CRM. Ele recebe: tipo de delivery, pedidos por dia, canal, o que mais pesa, nome, nome do delivery, cidade e WhatsApp.

## Antes de anunciar, confira

- Os números do painel ("412 mensagens", "R$ 13,9 mil") e das notas fiscais são **exemplo**, e a página diz isso. Se tiver um case real de delivery, ele pode entrar no lugar.
- O link "Política de privacidade" no rodapé está vazio (`href="#"`). Aponte para a sua política.
- Pixel da Meta e Google Tag: cole no `<head>` do `index.html`.

Feito pela Regência.
