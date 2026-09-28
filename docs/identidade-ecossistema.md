# Identidade do ecossistema Ishtar Sink

> Referência para nomear e desenhar cada novo projeto open source do ecossistema. Cole a
> seção **"Bloco para colar em um novo prompt"** no início do prompt-mãe de qualquer app
> novo, antes de descrever o que ele faz.
>
> Nasceu junto do [Nebula](https://github.com/Ishtar-Sink/Nebula/blob/main/README.md), o
> primeiro produto do ecossistema. A paleta em vigor foi revisada durante o refinamento do
> segundo produto, o [Atria](https://github.com/Ishtar-Sink/Atria) — a mudança de rosa para
> ciano e a adoção de um tema claro oficial vêm de lá, com Nebula preservando os valores
> antigos até migrar. **Este arquivo descreve uma convenção do ecossistema, não é específico
> de nenhum produto** — por isso mora aqui, no repositório `.github` da organização.

## A organização: Ishtar Sink

**A regra de nomeação dos produtos não vale para a organização.** São problemas diferentes:
o nome de um produto é lido e precisa explicar o que ele faz; o nome da organização é
*digitado* — em URL, em `git clone`, em escopo de pacote, em import — e precisa antes de
tudo ser fácil de lembrar e de escrever. Por isso a organização não precisa justificar
metáfora funcional nenhuma.

O nome vem do universo de **Destiny**, por significado pessoal de quem mantém o projeto. O
Ishtar Sink é a região de Vênus onde ficava a Ishtar Collective, a organização científica da
Era de Ouro dedicada a investigar e **arquivar** conhecimento — que é a razão de a referência
ter surgido: investigação aberta e conhecimento preservado, não poder nem conquista.

Por que este termo e não "Ishtar Collective", que era a primeira escolha:

- **`ishtar-collective.net` já existe** — é o arquivo de lore de Destiny mantido pela
  comunidade, ele próprio um recurso livre e gratuito. Usar o nome criaria confusão direta e
  pegaria carona na boa vontade de outro projeto livre. Incompatível com a premissa do
  ecossistema de não causar dano a ninguém.
- **Encurta de 17 para 11 caracteres** no handle (`ishtar-sink`), o que importa num nome que
  é digitado o tempo todo.

O termo também passa nas duas verificações que a organização precisa cumprir:

1. **Não é um corpo celeste.** É uma região, um lugar. Se os produtos são corpos celestes, a
   organização sendo outro faria parecer que ela é o produto principal e os demais, satélites
   dela. Uma bacia onde as coisas se acumulam é justamente a relação certa com os produtos.
2. **Fácil de digitar**: duas palavras curtas, grafia sem ambiguidade, pronúncia estável em
   português e inglês.

**Bônus que dispensa renomear nada**: Ishtar Terra é uma região real de Vênus. O nome já é
astronômico por origem, então os produtos seguem a convenção de astronomia sem nenhum atrito
— Nebula continua coerente ao lado dele.

**Ressalva conhecida e aceita**: em software, "sink" tem o sentido técnico de "para onde o
dado vai e não volta", oposto de "source" — um eco meio infeliz num ecossistema *open
source*. Foi pesado contra a leitura alternativa (uma bacia onde as coisas se reúnem) e
contra o fato de o termo ser neutro para o público em português, e considerado aceitável.

Histórico da busca anterior, encerrada: Cosmodrome, Gantry, Trajectory, Perigee e Ignition
saíram por indisponibilidade ou por não agradarem; Atlas, Axis, Parsec, Apex e Almanac eram
fáceis mas todos disputados. A conclusão que fechou essa linha: **nessa faixa de tamanho,
toda palavra fácil e temática já está registrada** — sempre cede um dos quatro critérios. Foi
o que levou a buscar o nome fora do jogo de metáforas, no significado pessoal.

## Como nomear um novo produto

Regra dupla, sem exceção: o nome precisa carregar **(a)** o tema do ecossistema
(astronomia) **e (b)** uma metáfora funcional específica daquele produto — não "soa
espacial", mas "o fenômeno real descreve o que o software faz". Um nome que só cumpre (a) é
decoração; um nome que só cumpre (b) quebra a família.

Checklist antes de fechar um nome:

1. O mecanismo físico do termo corresponde à mecânica central do produto (não à categoria
   genérica dele — "app de produtividade" não é mecânica, "várias peças formando um padrão"
   é)?
2. Curto, fácil de pronunciar em português e inglês, sem caractere que quebre em URL ou
   nome de pacote?
3. `npm view <nome>`, domínio e organização/repositório no GitHub livres, ou variação
   aceitável (`<nome>-app`, `use<nome>`) se não estiverem?
4. Não colide com um projeto open source grande já usando o termo?

**Nomes decididos até agora:**

| Produto | Termo | Por que se qualifica |
|---|---|---|
| **Nebula** | nuvem de gás e poeira que forma estrelas | player de música — organiza mídia solta em biblioteca; nascimento a partir de partes dispersas |
| **Atria** | α Trianguli Australis, estrela mais brilhante do Triângulo Austral | hub pessoal (financeiro, tarefas, diário, notas, acervo) — *átrio*: o pátio central da casa romana para onde todos os cômodos se abrem e por onde entra a luz, também a câmara do coração onde tudo chega antes de ser distribuído; módulos independentes que se abrem para um centro comum |

## Sistema visual: paleta única em todo o ecossistema

Decisão deliberada: **todo produto usa exatamente a mesma paleta**, não uma variação por
app. Prioriza reconhecimento de marca forte sobre diferenciação visual entre produtos — a
identidade visual diz "isto é Ishtar Sink", o nome e o ícone dizem qual produto é.

### 2026 — migração de roxo → rosa para roxo → ciano, com tema claro oficial

> Decidida durante o refinamento do Atria (`Ishtar-Sink/Atria`, spec `SPEC-001.md`), que é
> por isso o primeiro produto a nascer já nos valores novos.

O gradiente de marca passa de **roxo → rosa, somente dark** para **roxo → ciano, com tema
claro oficial e dark equivalente**. Rosa não teve nenhum problema — a mudança é de
posicionamento: **branco vira o padrão do ecossistema**, dark vira a alternativa, não o
único modo. Isso muda o que "cor de marca" significa: uma cor pensada só para fundo escuro
raramente sobrevive à travessia para fundo claro sem virar outra cor.

Racional do ciano contra o rosa: rosa saturado sobre fundo claro é agressivo e puxa a leitura
emocional para urgência. Ciano é frio, recua no fundo e funciona bem como cor de dado — gráfico,
barra de progresso, estado informativo.

**Rosa vira legado, não erro.** O Nebula continua rodando com os valores antigos (`#A855F7 →
#EC4899`, só dark) e migra quando for conveniente para o projeto — nada quebra por causa
desta mudança de convenção.

#### Restrição de contraste que definiu os valores do tema claro

Medido contra o fundo claro `#FAFAFC` (WCAG AA, texto normal ≥ 4,5:1):

| Cor | Contraste | Uso permitido |
|---|---|---|
| `#A855F7` (roxo vivo) | ≈ 4,0:1 | **reprova** AA para texto — só preenchimento, gradiente e ilustração |
| `#7C3AED` | ≈ 5,5:1 | aprova AA — é o roxo de **texto, link e ícone** no tema claro |
| `#06B6D4` (ciano vivo) | ≈ 2,4:1 | só preenchimento, gráfico e borda |
| `#0E7490` | ≈ 5,1:1 | aprova AA — é o ciano de **texto e link** no tema claro |

Consequência prática que todo produto novo herda: **no tema claro a cor de marca visível em
texto é `#7C3AED`, não `#A855F7`.** O `#A855F7` sobrevive em fundo de área, gradiente e
ilustração, onde contraste de texto não se aplica.

#### Tokens

```ts
// packages/theme/src/tokens.ts — fonte única; nenhum app redeclara cor.

export const light = {
  bg:            '#FAFAFC', // branco levemente frio; branco puro em tela cheia cansa
  bgElevated:    '#FFFFFF',
  surface:       '#FFFFFF',
  surfaceMuted:  '#F4F3F8',
  surfaceHover:  '#EFEDF6',
  border:        '#E6E3EF',
  borderStrong:  '#D5D0E3',

  primary:       '#7C3AED', // texto, link, ícone, botão primário
  primaryHover:  '#6D28D9',
  primaryBright: '#A855F7', // só preenchimento e gradiente
  primarySoft:   '#F3EBFF', // fundo do item ativo/hover da sidebar
  primaryOn:     '#FFFFFF',

  accent:        '#0E7490', // ciano de texto
  accentFill:    '#06B6D4', // ciano de gráfico e barra
  accentBright:  '#22D3EE',
  accentSoft:    '#E0F7FB',

  text:          '#1B1630',
  textMuted:     '#5C5478',
  textFaint:     '#8B84A3',

  success:       '#047857',
  warning:       '#B45309',
  danger:        '#BE123C',
  info:          '#0E7490',
};

export const dark = {
  bg:            '#0A0713', // preservado da paleta anterior — fundo violeta quase preto
  bgElevated:    '#120C22',
  surface:       '#1A1130',
  surfaceMuted:  '#150F28',
  surfaceHover:  '#241740',
  border:        '#2E1F52',
  borderStrong:  '#3D2A6B',

  primary:       '#A855F7',
  primaryHover:  '#C084FC',
  primaryBright: '#C084FC',
  primarySoft:   '#241740',
  primaryOn:     '#0A0713',

  accent:        '#22D3EE',
  accentFill:    '#06B6D4',
  accentBright:  '#67E8F9',
  accentSoft:    '#0E3A44',

  text:          '#F6F2FF',
  textMuted:     '#A99CC8',
  textFaint:     '#6E6190',

  success:       '#34D399',
  warning:       '#FBBF24',
  danger:        '#FB7185',
  info:          '#22D3EE',
};

export const gradients = {
  brand: ['#7C3AED', '#06B6D4'], // roxo → ciano — substitui roxo → rosa
  deep:  ['#6D28D9', '#7C3AED'],
  calm:  ['#F3EBFF', '#E0F7FB'], // fundo de tela não autenticada, no tema claro
};
```

Escalas de forma e espaço, também compartilhadas e sem mudança nesta revisão:

```ts
export const radii = { sm: 8, md: 12, lg: 18, xl: 26, pill: 999 };
export const space = (n: number) => n * 4; // grade de 4px
```

**Regra prática**: todo produto novo importa o pacote de tema compartilhado em vez de
redeclarar essas cores. Hoje o pacote vive dentro de cada produto (`packages/theme` no
Nebula e no Atria) com um comentário no topo apontando este documento como origem; a
extração para um pacote único da organização, consumido por ambos, ainda está pendente. Um
valor mudado no pacote compartilhado muda em todos os produtos de uma vez — é a garantia de
que a paleta não diverge com o tempo.

**Alternância de tema**: `data-theme="light" | "dark"` no elemento raiz, **padrão `light`**,
`prefers-color-scheme` respeitado só quando o usuário nunca escolheu explicitamente.

### O truque de cor determinística por item

Onde o produto tem uma coleção de itens sem imagem própria (faixas sem capa, no Nebula —
mas o mesmo serve pra projetos sem ícone, entradas de diário sem humor definido, etc.), usa
um hash simples do id pra escolher sempre o mesmo par de cores daquele item, sem guardar
nada:

```ts
export const artPalettes: Array<[string, string]> = [
  ['#7C3AED', '#06B6D4'], ['#A855F7', '#22D3EE'], ['#6366F1', '#2DD4BF'],
  ['#8B5CF6', '#38BDF8'], ['#4C1D95', '#0E7490'], ['#9333EA', '#67E8F9'],
  ['#5B21B6', '#14B8A6'], ['#C084FC', '#0891B2'], ['#7E22CE', '#06B6D4'],
  ['#6D28D9', '#5EEAD4'],
];

export function paletteFor(seed: string): [string, string] {
  let h = 0;
  for (let i = 0; i < seed.length; i++) h = (h * 31 + seed.charCodeAt(i)) >>> 0;
  return artPalettes[h % artPalettes.length];
}
```

Mesmo id → mesma cor em todo cliente, sem round-trip ao servidor nem estado extra. Paleta
repaginada para a família roxo–ciano; o Nebula mantém a variante rosa até migrar.

## Tipografia

Par de fontes, não uma só — decidido durante o refinamento do Atria porque um produto com
blocos longos de texto (diário, notas, formulário) expôs que a Outfit foi desenhada para
display, não para parágrafo:

| Papel | Fonte | Regra |
|---|---|---|
| Títulos grandes, números grandes, logo | **Outfit** | peso 700–800, `letter-spacing` **negativo** (`-0.4px` a `-1.6px` conforme o tamanho sobe) — aperta o texto grande, evita o efeito "solto" |
| Rótulos pequenos em caixa alta ("eyebrow", badges, seções) | **Outfit** | peso 600, `letter-spacing` **positivo** (`0.9px` a `1.4px`) — abre o texto pequeno, mantém legibilidade em maiúsculas |
| Corpo, formulário, tabela, editor | **Inter** | peso 400–600, `letter-spacing` 0, `line-height` 1,6 em texto longo |

```css
--font-display: 'Outfit', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;
--font-body:    'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;

.page-title      { font-family: var(--font-display); font-size: 44px; font-weight: 800; letter-spacing: -1.6px; line-height: 1.05; }
.section-title   { font-family: var(--font-display); font-size: 21px; font-weight: 700; letter-spacing: -0.5px; }
.page-eyebrow    { font-family: var(--font-display); font-size: 12px; font-weight: 600; letter-spacing: 1.4px; text-transform: uppercase; }
.prose           { font-family: var(--font-body); font-size: 16px; line-height: 1.65; max-width: 68ch; }
```

Um produto sem texto longo (o Nebula, por exemplo) pode continuar só com Outfit — o par com
Inter é regra para quem tem prosa, não obrigação universal retroativa.

Fontes são **servidas pelo próprio app**, nunca por um CDN de fontes em runtime —
autohospedagem não faz requisição externa sem o usuário pedir.

## Bloco para colar em um novo prompt

```markdown
## Identidade do ecossistema Ishtar Sink

Este produto pertence ao ecossistema Ishtar Sink (github.com/ishtar-sink). Duas regras
não-negociáveis:

1. **Nome do produto**: já decidido como "<NOME>" — termo de astronomia cujo fenômeno real
   mapeia para a mecânica central do produto (ver
   github.com/Ishtar-Sink/.github/blob/main/docs/identidade-ecossistema.md para o precedente e
   o checklist, caso o nome ainda não esteja fechado).

2. **Identidade visual**: usar a paleta e os tokens do ecossistema tal como estão, sem criar
   uma paleta própria para este produto.
   - **Tema claro é o padrão**, dark é a alternativa — não o único modo. Fundo claro
     `#FAFAFC`, superfícies `#FFFFFF`/`#F4F3F8`, texto `#1B1630`/`#5C5478`/`#8B84A3`. Dark
     equivalente: fundo `#0A0713`, superfícies `#1A1130`/`#241740`, texto
     `#F6F2FF`/`#A99CC8`/`#6E6190`.
   - Marca: gradiente roxo → ciano (`#7C3AED` → `#06B6D4`). No tema claro, a cor de marca
     em **texto** é `#7C3AED` (não `#A855F7` — reprova contraste AA para texto); `#A855F7`
     é só para preenchimento e gradiente. O par correspondente em ciano é `#0E7490` para
     texto, `#06B6D4` para preenchimento.
   - Fonte **Outfit** para título/número grande/rótulo em caixa alta (letter-spacing
     negativo nos grandes, positivo nos pequenos); **Inter** para corpo, formulário e
     tabela, se o produto tiver texto longo.
   - Raios de borda: 8/12/18/26px, pill para badges e botões redondos.
   - Se houver itens sem imagem própria (cards, avatares, tags), gerar a cor a partir de
     um hash determinístico do id, não de estado salvo — ver "cor determinística por item"
     no doc de identidade.
```
