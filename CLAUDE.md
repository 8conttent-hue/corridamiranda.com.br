# CLAUDE.md — CORRIDAMIRANDA

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** CORRIDAMIRANDA
**Nicho:** Esportes e Fitness
**Keywords:** Ola E um prazer receber voce em meu site meu nome e
**Paleta de cores:** sunset | **Fonte:** lora

Olá! É um prazer receber você em meu site, meu nome é Raquel Miranda, sou corredora profissional a 7 anos, sinta-se a vontade! Criei este site para ajudar todas as pessoas que buscam algum tipo de conhecimento na área da corrida. Ou para as que desejam manter uma vida mais regrada e saudável através de uma dieta ou com simples exercícios diários. Escrevo para este site com toda a minha bagagem e experiência adquirida ao longo dos anos nas pistas de corrida. Quando comecei a me interessar por corrida de rua e de pista, quase não achava conteúdo na internet, então decidi criar esse espaço. Meu objetivo sempre será compartilhar todo o meu conhecimento de forma completamente gratuita, na intenção de ajudar o maior número de pessoas possível.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-E |
| Hero | Hero-H |
| Features | Features-C |
| About Section | About-G |
| Posts | Posts-A |
| Footer | Footer-C |
| Página Sobre | Sobre-C |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
