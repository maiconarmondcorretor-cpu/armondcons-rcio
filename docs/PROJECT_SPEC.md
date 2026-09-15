# Especificação — Armond Consórcios

## Posicionamento
Plataforma premium de consórcios com protagonismo imobiliário. Linguagem de fintech/private banking/wealth management/proptech: conquista, patrimônio, planejamento, tecnologia e simplicidade.

## Hero
Headline: **Transforme planejamento em patrimônio.**

Subheadline: Use o consórcio para conquistar seu imóvel, investir, ampliar seu patrimônio ou realizar novos projetos de forma planejada.

CTAs: `SIMULE SEU CONSÓRCIO` e `ENTENDA COMO FUNCIONA`.

Confiança: Simulação online • Sem compromisso • Atendimento especializado.

O Hero deve ter fundo visual premium que transmita conquista, liberdade, futuro e patrimônio e conter o início do simulador.

## Simulador
1. Categoria: Imóvel, Carro, Moto, Veículos Pesados, Serviços.
2. Crédito: campo monetário. Para imóvel, atalhos R$300 mil, R$500 mil, R$800 mil, R$1 milhão e outro.
3. Objetivo imobiliário: comprar meu imóvel; investir em imóveis; construir patrimônio; comprar outro imóvel; construir/reformar; ainda avaliando.
4. Contato: nome, WhatsApp, e-mail, LGPD.
5. Opções: inicialmente mock de desenvolvimento; futuramente planos reais Embracon.

Todos os CTAs Simular usam o mesmo fluxo e preservam a categoria selecionada.

## Home
- Header transparente → sólido no scroll.
- Hero + simulador.
- “Consórcio pode ser muito mais do que comprar um imóvel”: Conquistar, Investir, Construir Patrimônio.
- “Seu próximo imóvel pode fazer parte de um plano maior”: compra, investimento, renda, patrimônio, construção, reforma.
- “Patrimônio não acontece por acaso. Ele é construído.”: Planejamento → Carta de crédito → Aquisição → Novo ativo → Patrimônio.
- Planejamento patrimonial de longo prazo.
- Categorias de consórcio.
- Como funciona em 4 etapas.
- Por que Armond Consórcios: experiência imobiliária, visão patrimonial, atendimento especializado, tecnologia.
- FAQ completo.
- CTA final: “Todo patrimônio começa com uma decisão.”
- WhatsApp flutuante.
- Footer institucional Armond Imóveis.

## Dados institucionais
Não inventar CNPJ, endereço, telefone, e-mail ou CRECI. Centralizar em `companyConfig` para preenchimento posterior.

## Rotas
`/`, `/simulador`, `/consorcio-imobiliario`, `/consorcio-auto`, `/consorcio-moto`, `/consorcio-pesados`, `/consorcio-servicos`, `/como-funciona`, `/sobre`, `/contato`, `/politica-de-privacidade`, `/termos-de-uso`.

## Analytics
Preparar: GA4, GTM, Meta Pixel/CAPI e Google Ads, sem IDs fictícios. Eventos: simulation_started, category_selected, credit_selected, simulation_completed, lead_created, plan_viewed, plan_selected, proposal_started, proposal_completed, payment_started, contract_completed. Capturar UTMs, fbclid e gclid.

## Segurança
Nenhuma chave privada no frontend. `.env.example`. Validação server-side quando houver backend. Arquitetura compatível com LGPD.

## Embracon
Criar adapter/provider isolado. Nunca inventar endpoints. O mock deve estar explicitamente marcado como desenvolvimento. Futuramente: produtos, créditos, grupos, planos, parcelas, prazos, taxas, simulação, proposta, cliente, status, pagamento e contratação.

## Performance e SEO
Mobile-first, Core Web Vitals, lazy loading, imagens WebP/AVIF, SEO técnico, Open Graph, canonical, sitemap, robots e dados estruturados quando aplicável.
