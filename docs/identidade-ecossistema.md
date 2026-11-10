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
| **Flare** | erupção solar: um clarão súbito, intenso e breve na superfície do Sol | soundpad pessoal — dispara sob demanda um som curto e marcante: aperta o botão, o som aparece de uma vez e some. Decidido no refinamento da SPEC-001, quando o projeto ainda se chamava "Soundpad" |
| **Translunar** | injeção translunar: a queima de motor que tira a nave da órbita da Terra e a manda para outro mundo | pipeline de legendas multilíngues — o corte em pt-BR sai do público de origem e é lançado para os públicos de outros idiomas, localizado em vez de traduzido literalmente; a manobra é literalmente uma *burn*, e a ferramenta queima a legenda no vídeo; *trans-* ecoa *translate* sem prometer tradução literal |
| **Synestia** | o anel de rocha vaporizada que se formou depois da colisão que criou a Lua, de onde ela se condensou aos poucos | ferramenta de estudos — o conhecimento de um tema, novo ou revisto, se forma em camadas pequenas, cada uma presa à anterior, com um tutor que pergunta em vez de entregar a resposta |
| **Vega** | α Lyrae, a referência de brilho da astronomia: o ponto zero da escala de magnitude, contra o qual o brilho das outras estrelas foi medido por séculos ("sistema Vega") | biblioteca de componentes do ecossistema — a referência visual contra a qual todos os produtos se medem; mudou a referência, muda a identidade de todos os produtos de uma vez |

Translunar, decidido em 2026-10-28 a partir da SPEC-001 ("Pipeline de legendas
multilíngues"). Disponibilidade na data: npm e PyPI livres, `translunar.dev` e
`translunar.app` sem registro aparente; `.com`, `.io` e o usuário `translunar` no GitHub
ocupados, o que não afeta `Ishtar-Sink/Translunar`. Ressalva aceita: 10 letras, mais longo
que Nebula e Atria. Termos avaliados e descartados para esse produto:

- **Rosetta** (sonda da ESA, nomeada pela Pedra de Roseta, um texto em três escritas):
  metáfora quase perfeita, mas colide com Apple Rosetta e Rosetta Stone, e npm, PyPI e
  `.dev` estão ocupados.
- **Refracta** (refração: a luz se curva ao entrar num meio novo): npm e PyPI livres, mas já
  existe uma ferramenta Linux chamada Refracta, e `.com` e `.io` estão ocupados.
- **Radiant** (o ponto de onde os meteoros de uma chuva parecem sair): npm e PyPI ocupados,
  e o projeto `radiant/radiant` já existe.
- **Doppler** (o mesmo sinal percebido de forma diferente por cada observador): colide com a
  empresa Doppler, e npm e PyPI estão ocupados.
- **Parallax**, **Perseid** e **Lensing**: ocupados, ou com a metáfora mais fraca.

Synestia, decidido em 2026-11-10. O primeiro uso é a preparação para um vestibular, mas o
nome descreve a ferramenta genérica — aprender um tema do zero ou revisar um esquecido —, não
esse caso. Disponibilidade na data: npm, PyPI, `synestia.dev` e `synestia.app` livres;
`synestia.com` registrado; no GitHub, só um sistema operacional pequeno com o termo.
Ressalva aceita: o termo é de 2017 e pouco conhecido, então o README precisa explicar a
metáfora. Termos avaliados e descartados para esse produto:

- **Nomes presos ao caso de uso**: Encke (o cometa que volta com mais frequência), Saros (o
  ciclo que prevê eclipses), Cepheid (a estrela que pulsa num período regular), Ceres (o
  asteroide perdido e reencontrado por cálculo), Spica e Alcor. Todos descreviam revisão ou
  prova, e a ferramenta também serve para aprender algo novo. Saros, Cepheid e Encke também
  não agradaram pelo som.
- **Maia** (a estrela das Plêiades que deu origem a *maiêutica*, o método socrático): a
  metáfora é genérica e boa, mas npm, PyPI e domínios estão ocupados, e o nome não agradou.
- **Accretion** (acreção, crescer grão por grão): agradou, mas os domínios estão ocupados e
  há um gerenciador de conhecimento pessoal com o mesmo nome no GitHub.
- **Planetesimal**: livre, mas longo e técnico.
- **Accrete**, **Protostar**, **Regolith**, **Moonlet**, **Crescent**, **Ephemeris**,
  **Halley**, **Mira**, **Astra**, **Vesper**, **Selene**: ocupados, colidem com projetos
  conhecidos ou têm a metáfora fraca.

Vega, decidido em 2026-11-10. Não é um produto para o usuário final, e sim a biblioteca de
componentes React que nasce do `@atria/ui` (botões, campos, diálogos, toasts, abas, cartões,
estados de vazio e de erro, sobre os tokens do pacote de tema) e passa a ser consumida por
todos os produtos. Publicada sob o escopo `@ishtar-sink`, livre no npm na data
(`@ishtar-sink/vega`). Ressalva aceita: a gramática de visualização Vega (`vega/vega`, cerca de
12 mil estrelas, dona do nome sem escopo no npm) usa o termo no mesmo ecossistema JavaScript,
então buscas e discussões de frontend vão misturar as duas; o escopo evita a colisão no
pacote. Termos avaliados e descartados:

- **Asterism** (desenho de estrelas de constelações diferentes, como o Triângulo de Verão) e
  **Barycenter** (o centro de massa que todos os corpos orbitam): metáforas boas, mas não
  agradaram pelo som.
- **Albireo** (estrela dupla dourada e azul): livre, mas descreve só os dois temas, não as
  peças compartilhadas.
- **Photosphere**, **Corona**, **Lyra** e **Cassini**: longos, ocupados ou sem mecânica.

## Sistema visual: tema padrão do ecossistema

A paleta desta seção é o **tema padrão do Ishtar Sink**, exportado pela
[Vega](https://github.com/Ishtar-Sink/Vega) junto com os componentes. É o ponto de partida de
todo produto, e um produto pode trocá-la por uma paleta própria (ver a subseção `2026-11`
logo abaixo). Até 2026-11 a regra era outra: todo produto usava exatamente a mesma paleta,
priorizando o reconhecimento da marca pela cor.

### 2026-11 — o tema sai da Vega, e cada produto pode ter paleta própria

> Decidido em 2026-11-10, junto com a criação da Vega, a biblioteca de componentes do
> ecossistema.

A Vega exporta **componentes e temas**. O tema Ishtar Sink, com os tokens desta seção, é o
padrão, e cada produto pode substituí-lo por uma paleta própria.

Por que a regra mudou: a Vega é uma biblioteca aberta, que qualquer pessoa pode usar fora do
ecossistema, e por isso precisa ser tematizável de verdade. Com essa capacidade pronta, os
produtos do ecossistema ganham a mesma liberdade.

**O que continua compartilhado** entre todos os produtos, com ou sem paleta própria:

- os componentes da Vega;
- a tipografia, os raios, o espaço e o movimento;
- a **estrutura** dos tokens: os mesmos nomes (`bg`, `surface`, `primary`, `success`, os
  `*Soft`, as camadas de elevação), nos temas claro e escuro;
- a alternância de tema, com o claro como padrão;
- as regras de contraste.

A identidade "isto é Ishtar Sink" passa a vir da forma dos componentes, da tipografia e da
convenção de nomes, mais do que da cor. É uma troca consciente: um produto com paleta própria
se reconhece menos pela cor como parte da família.

**Regras para um produto com paleta própria:**

- **O tema é criado com a API de tema da Vega** e passado para os componentes. Nenhum
  componente redeclara cor, nem no produto nem na Vega.
- **Todos os tokens nos dois temas.** Uma paleta própria cobre claro e escuro, com o mesmo
  conjunto de tokens do tema padrão.
- **Contraste AA verificado.** O tema passa pelas mesmas verificações de contraste do tema
  padrão (texto normal em 4,5:1, `textFaint` em 3:1), feitas por teste e não estimadas.
- **Estados continuam distinguíveis.** Sucesso, aviso, erro e informação seguem diferentes
  entre si e não dependem só do matiz: o fundo `*Soft`, o ícone e a palavra dizem o mesmo.
- **A decisão fica registrada no produto**, com o motivo, na documentação de identidade dele.
  Um produto sem motivo para paleta própria usa o tema padrão.

### 2026-10 — nova paleta com profundidade (Flare)

> Origem: refinamento da SPEC-002 do Flare (`Ishtar-Sink/Flare`, "Melhorias no Backoffice"),
> com a paleta aprovada em 25/10/2026. O bloco de tokens da subseção de 2026, logo abaixo, já
> traz estes valores.

A paleta continua única em todo o ecossistema, e o roxo continua sendo a cor da marca. A
mudança é de **estrutura**, não de identidade: o tema anterior era plano, com fundo, cartão e
borda quase na mesma luminosidade e sem sombra, e as cores de estado só existiam como cor de
texto. Nada se destacava do fundo, e sucesso, aviso e erro só se distinguiam lendo a palavra.

O que muda:

- **Fundo com matiz roxo.** O fundo claro deixa de ser o branco levemente frio (`#FAFAFC`) e
  passa a lavanda claro (`#F3F0FA`); os cartões continuam brancos. A diferença de luminosidade
  entre página e cartão cria a primeira camada de profundidade sem precisar de borda grossa. No
  escuro, o fundo segue violeta quase preto (`#0B0816`).
- **Camadas de elevação.** Três níveis (`elevation1` a `elevation3`) para cartão, menu e
  diálogo. No claro, todas as camadas são brancas e a diferença vem da sombra (`shadows.sm`,
  `md` e `lg`), tingida de roxo escuro em vez de preto para não sujar o fundo lavanda. No
  escuro, a sombra quase não aparece, então cada nível sobe de luminosidade e a sombra só
  reforça.
- **Roxo de texto um degrau mais escuro no claro.** `#6D28D9` substitui `#7C3AED` como roxo de
  texto. Sobre o fundo lavanda e sobre `primarySoft`, o roxo anterior ficava perto do limite de
  4,5:1; o novo tem folga. `#A855F7` continua só para preenchimento e gradiente. No escuro, o
  roxo de texto sobe para `#A78BFA`.
- **Cores de status com fundo suave.** `successSoft`, `warningSoft`, `dangerSoft` e `infoSoft`
  dão a cada estado um fundo de baixa saturação, com texto e ícone na cor cheia do estado.
  Estado deixa de depender só do matiz: o fundo, o ícone e a palavra dizem o mesmo. O aviso
  escurece de `#B45309` para `#92400E` no claro, para passar em AA sobre o seu fundo suave. A
  informação deixa de repetir o ciano do destaque e vira azul (`#0369A1` no claro, `#38BDF8` no
  escuro), para que "informação" não se confunda com "destaque de dado".
- **Texto com mais contraste.** `text` e `textMuted` escurecem um pouco no claro e clareiam no
  escuro, para que o texto secundário passe em AA também sobre `surfaceMuted` e sobre os fundos
  suaves.
- **Movimento com tokens.** Durações (`motion.fast` 120 ms, `motion.base` 200 ms,
  `motion.slow` 320 ms) e curvas (`motion.ease.*`) viram tokens, para que a animação seja igual
  em todos os produtos. Nenhuma transição passa de 320 ms.

**Consequência prática que todo produto herda**: no tema claro a cor de marca em texto é
`#6D28D9`, e o fundo de um estado é sempre o `*Soft` correspondente, nunca a cor cheia.

#### Valores que mudam

Os tokens que não aparecem nas tabelas mantêm o valor anterior (por exemplo, `surface` no claro,
`primaryBright`, `accent`, `accentFill`, `success` e `danger`). Os valores anteriores ficam
registrados aqui como legado.

**Tema claro**

| Token | Antes | Depois |
|---|---|---|
| `bg` | `#FAFAFC` | `#F3F0FA` |
| `bgElevated` | `#FFFFFF` | `#FAF8FE` |
| `surfaceMuted` | `#F4F3F8` | `#EAE5F6` |
| `surfaceHover` | `#EFEDF6` | `#E1DAF2` |
| `border` | `#E6E3EF` | `#D9D1EC` |
| `borderStrong` | `#D5D0E3` | `#BFB3DD` |
| `primary` | `#7C3AED` | `#6D28D9` |
| `primaryHover` | `#6D28D9` | `#5B21B6` |
| `primarySoft` | `#F3EBFF` | `#EBE0FD` |
| `accentSoft` | `#E0F7FB` | `#D8F1F6` |
| `text` | `#1B1630` | `#1A1230` |
| `textMuted` | `#5C5478` | `#4F4469` |
| `warning` | `#B45309` | `#92400E` |
| `info` | `#0E7490` | `#0369A1` |

**Tema escuro**

| Token | Antes | Depois |
|---|---|---|
| `bg` | `#0A0713` | `#0B0816` |
| `bgElevated` | `#120C22` | `#110B21` |
| `surface` | `#1A1130` | `#181028` |
| `surfaceMuted` | `#150F28` | `#130D22` |
| `surfaceHover` | `#241740` | `#241A3D` |
| `border` | `#2E1F52` | `#2F2250` |
| `borderStrong` | `#3D2A6B` | `#45337A` |
| `primary` | `#A855F7` | `#A78BFA` |
| `primaryHover` | `#C084FC` | `#C4B5FD` |
| `primarySoft` | `#241740` | `#2B1D52` |
| `primaryOn` | `#0A0713` | `#12082B` |
| `accentSoft` | `#0E3A44` | `#0F3342` |
| `text` | `#F6F2FF` | `#F5F1FF` |
| `textMuted` | `#A99CC8` | `#B1A5CF` |
| `textFaint` | `#6E6190` | `#7A6C9E` |
| `info` | `#22D3EE` | `#38BDF8` |

Os tokens de estado `*Soft`, as camadas `elevation1` a `elevation3` e `shadows` são novos nos
dois temas e aparecem no bloco de tokens abaixo.

#### Contraste medido

Texto normal exige 4,5:1 (WCAG AA). A razão é a luminância relativa do WCAG 2, calculada por
script e não estimada. Pares principais:

| Tema | Texto | Fundo | Razão | Resultado |
|---|---|---|---|---|
| Claro | `text` #1A1230 | `bg` #F3F0FA | 15,90:1 | AA |
| Claro | `text` #1A1230 | `surface` #FFFFFF | 17,90:1 | AA |
| Claro | `textMuted` #4F4469 | `bg` #F3F0FA | 7,89:1 | AA |
| Claro | `textMuted` #4F4469 | `surface` #FFFFFF | 8,89:1 | AA |
| Claro | `primary` #6D28D9 | `bg` #F3F0FA | 6,31:1 | AA |
| Claro | `primary` #6D28D9 | `surface` #FFFFFF | 7,10:1 | AA |
| Claro | `primary` #6D28D9 | `primarySoft` #EBE0FD | 5,62:1 | AA |
| Claro | `accent` #0E7490 | `bg` #F3F0FA | 4,76:1 | AA |
| Claro | `accent` #0E7490 | `accentSoft` #D8F1F6 | 4,55:1 | AA (pior par do claro) |
| Claro | `success` #047857 | `successSoft` #D9F3E7 | 4,68:1 | AA |
| Claro | `warning` #92400E | `warningSoft` #FCEFCF | 6,21:1 | AA |
| Claro | `danger` #BE123C | `dangerSoft` #FDE2E9 | 5,16:1 | AA |
| Claro | `info` #0369A1 | `infoSoft` #DAEEFB | 4,97:1 | AA |
| Claro | `primaryOn` #FFFFFF | `primary` #6D28D9 | 7,10:1 | AA |
| Escuro | `text` #F5F1FF | `bg` #0B0816 | 17,83:1 | AA |
| Escuro | `text` #F5F1FF | `surface` #181028 | 16,53:1 | AA |
| Escuro | `textMuted` #B1A5CF | `bg` #0B0816 | 8,63:1 | AA |
| Escuro | `textMuted` #B1A5CF | `surface` #181028 | 8,00:1 | AA |
| Escuro | `primary` #A78BFA | `bg` #0B0816 | 7,28:1 | AA |
| Escuro | `primary` #A78BFA | `surface` #181028 | 6,75:1 | AA |
| Escuro | `primary` #A78BFA | `primarySoft` #2B1D52 | 5,51:1 | AA (pior par do escuro) |
| Escuro | `accent` #22D3EE | `surface` #181028 | 10,16:1 | AA |
| Escuro | `success` #34D399 | `successSoft` #0E2E27 | 7,59:1 | AA |
| Escuro | `warning` #FBBF24 | `warningSoft` #33260B | 8,84:1 | AA |
| Escuro | `danger` #FB7185 | `dangerSoft` #3A1222 | 6,05:1 | AA |
| Escuro | `info` #38BDF8 | `infoSoft` #0C2C42 | 6,74:1 | AA |
| Escuro | `primaryOn` #12082B | `primary` #A78BFA | 7,04:1 | AA |

#### textFaint: só decorativo ou texto grande

`textFaint` não passa em 4,5:1 e por isso **não é texto de leitura**. Serve a ícone inerte,
divisor e dica não essencial, ou a texto grande e componente, com exigência de 3:1. Medido:
no claro, `#8B84A3` tem 3,15:1 sobre `bg` e 3,54:1 sobre `surface`; no escuro, `#7A6C9E` tem
4,21:1 sobre `bg` e 3,91:1 sobre `surface`.

#### Legado e migração

**Rosa vira legado, não erro, e roxo antigo também.** Nebula e Atria migram para esta paleta nos
próprios projetos quando for conveniente. Até lá continuam com os valores anteriores, e nada
quebra por causa desta mudança: os valores de antes ficam nas tabelas desta subseção e valem
como legado.

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

> A partir de 2026-10, esta tabela vale como registro dos valores anteriores. No tema claro o
> roxo de texto passa a ser `#6D28D9` (ver a subseção `2026-10` acima).

Consequência prática que todo produto novo herda: **no tema claro a cor de marca visível em
texto é `#7C3AED`, não `#A855F7`.** O `#A855F7` sobrevive em fundo de área, gradiente e
ilustração, onde contraste de texto não se aplica.

#### Tokens

> Valores atualizados em 2026-10 (ver a subseção acima), com `motion` novo. Os valores
> anteriores estão nas tabelas dela. `gradients` e as escalas de forma e espaço não mudam.

```ts
// Vega: src/theme/tokens.ts (@ishtar-sink/vega) — fonte única; nenhum app redeclara cor.
// Fonte de verdade da identidade visual do ecossistema Ishtar Sink (DEC-001, [project/theme-08]).
// tokens.css espelha estes valores; mudança aqui é levada para Ishtar-Sink/.github docs/identidade-ecossistema.md.

export const light = {
  bg:            '#F3F0FA', // lavanda claro: a diferença para o cartão branco cria a primeira camada
  bgElevated:    '#FAF8FE', // barra lateral e cabeçalho, entre a página e os cartões
  surface:       '#FFFFFF', // cartões e painéis (camada 1)
  surfaceMuted:  '#EAE5F6',
  surfaceHover:  '#E1DAF2',
  border:        '#D9D1EC',
  borderStrong:  '#BFB3DD',

  elevation1:    '#FFFFFF', // cartão em repouso
  elevation2:    '#FFFFFF', // menu, popover, item arrastado (a sombra faz a diferença)
  elevation3:    '#FFFFFF', // diálogo modal e toast

  primary:       '#6D28D9', // texto, link, ícone, botão primário
  primaryHover:  '#5B21B6',
  primaryBright: '#A855F7', // só preenchimento e gradiente
  primarySoft:   '#EBE0FD', // item ativo da sidebar, chip e selo de marca
  primaryOn:     '#FFFFFF',

  accent:        '#0E7490', // ciano de texto e link
  accentFill:    '#06B6D4', // ciano de gráfico e barra
  accentBright:  '#22D3EE', // destaque e gradiente
  accentSoft:    '#D8F1F6', // fundo do selo e do destaque ciano

  text:          '#1A1230', // texto principal
  textMuted:     '#4F4469', // texto secundário e rótulo
  textFaint:     '#8B84A3', // só decorativo e texto grande (3:1)

  success:       '#047857', // texto e ícone de sucesso
  successSoft:   '#D9F3E7', // fundo de toast, selo e alerta de sucesso
  warning:       '#92400E', // escurecido para passar em AA sobre warningSoft
  warningSoft:   '#FCEFCF', // fundo de toast, selo e alerta de aviso
  danger:        '#BE123C', // texto, ícone e botão de perigo
  dangerSoft:    '#FDE2E9', // fundo de toast, selo e alerta de erro
  info:          '#0369A1', // azul, separado do ciano do destaque
  infoSoft:      '#DAEEFB', // fundo de toast, selo e alerta informativo

  shadows: {
    sm: '0 1px 2px rgba(42, 24, 96, 0.08)',                                       // botão, campo e chip
    md: '0 4px 12px rgba(42, 24, 96, 0.10), 0 1px 3px rgba(42, 24, 96, 0.06)',    // cartão elevado, menu e toast
    lg: '0 18px 44px rgba(42, 24, 96, 0.20), 0 4px 12px rgba(42, 24, 96, 0.08)',  // diálogo modal
  },
};

export const dark = {
  bg:            '#0B0816', // violeta quase preto
  bgElevated:    '#110B21', // barra lateral e cabeçalho
  surface:       '#181028', // cartões e painéis (camada 1)
  surfaceMuted:  '#130D22',
  surfaceHover:  '#241A3D',
  border:        '#2F2250',
  borderStrong:  '#45337A',

  elevation1:    '#181028', // cartão em repouso (igual a surface)
  elevation2:    '#201638', // menu, popover, item arrastado
  elevation3:    '#2A1D4A', // diálogo modal e toast

  primary:       '#A78BFA', // texto, link, ícone, botão primário
  primaryHover:  '#C4B5FD',
  primaryBright: '#C084FC', // só preenchimento e gradiente
  primarySoft:   '#2B1D52', // item ativo da sidebar, chip e selo de marca
  primaryOn:     '#12082B',

  accent:        '#22D3EE', // ciano de texto e link
  accentFill:    '#06B6D4', // ciano de gráfico e barra
  accentBright:  '#67E8F9', // destaque e gradiente
  accentSoft:    '#0F3342', // fundo do selo e do destaque ciano

  text:          '#F5F1FF', // texto principal
  textMuted:     '#B1A5CF', // texto secundário e rótulo
  textFaint:     '#7A6C9E', // só decorativo e texto grande (3:1)

  success:       '#34D399', // texto e ícone de sucesso
  successSoft:   '#0E2E27', // fundo de toast, selo e alerta de sucesso
  warning:       '#FBBF24', // texto e ícone de aviso
  warningSoft:   '#33260B', // fundo de toast, selo e alerta de aviso
  danger:        '#FB7185', // texto, ícone e botão de perigo
  dangerSoft:    '#3A1222', // fundo de toast, selo e alerta de erro
  info:          '#38BDF8', // texto e ícone de informação
  infoSoft:      '#0C2C42', // fundo de toast, selo e alerta informativo

  shadows: {
    sm: '0 1px 2px rgba(0, 0, 0, 0.45)',                                                                // botão, campo e chip
    md: '0 6px 16px rgba(0, 0, 0, 0.50), 0 0 0 1px rgba(167, 139, 250, 0.08)',                          // cartão elevado, menu e toast
    lg: '0 22px 52px rgba(0, 0, 0, 0.65), 0 0 0 1px rgba(167, 139, 250, 0.14)',                         // diálogo modal
  },
};

export const gradients = {
  brand: ['#7C3AED', '#06B6D4'], // roxo → ciano — substitui roxo → rosa
  deep:  ['#6D28D9', '#7C3AED'],
  calm:  ['#F3EBFF', '#E0F7FB'], // fundo de tela não autenticada, no tema claro
};

export const motion = {
  fast: 120, // ms: hover, foco, pressão, entrada de tooltip
  base: 200, // ms: diálogo, toast, aba, expandir linha
  slow: 320, // ms: troca de tela, preenchimento de barra (teto)
  ease: {
    standard: 'cubic-bezier(0.4, 0, 0.2, 1)', // mudança de estado do que já está na tela
    enter:    'cubic-bezier(0, 0, 0.2, 1)',   // elemento que entra
    exit:     'cubic-bezier(0.4, 0, 1, 1)',   // elemento que sai
    linear:   'linear',                        // só laços contínuos
  },
};
```

Escalas de forma e espaço, também compartilhadas e sem mudança nesta revisão:

```ts
export const radii = { sm: 8, md: 12, lg: 18, xl: 26, pill: 999 };
export const space = (n: number) => n * 4; // grade de 4px
```

Tokens acrescentados na Vega 0.1.0 (2026-11-10), para que nenhum componente tenha peso de
fonte, entrelinha, camada ou cor de item literais:

```ts
export const fontWeights = { semibold: 600, bold: 700, extrabold: 800 };
export const lineHeights = { tight: 1.1, relaxed: 1.6 };
export const zIndices = { dropdown: 40, popover: 45, toast: 200 }; // dropdown, popover e toast

// Pares de cor dos itens sem imagem própria; o ItemSwatch escolhe o par pelo hash do id.
// Substitui paletteFor/artPalettes do @atria/theme, com os mesmos valores.
export const itemPalette = [
  ['#7C3AED', '#06B6D4'],
  ['#A855F7', '#22D3EE'],
  ['#6366F1', '#2DD4BF'],
  ['#8B5CF6', '#38BDF8'],
  ['#4C1D95', '#0E7490'],
  ['#9333EA', '#67E8F9'],
  ['#5B21B6', '#14B8A6'],
  ['#C084FC', '#0891B2'],
  ['#7E22CE', '#06B6D4'],
  ['#6D28D9', '#5EEAD4'],
];
```

No `tokens.css`, eles viram `--font-weight-*`, `--line-height-*`, `--z-*` e
`--item-palette-N-from`/`--item-palette-N-to`, e o gradiente `deep` ganha a variável
`--deep-gradient` (`linear-gradient(135deg, #6d28d9, #7c3aed)`).

**Raio dos controles**: botões, grupos de botões e seletores usam `radii.md` (12px), o mesmo
dos campos de formulário, para que botão e campo lado a lado tenham a mesma forma.
`radii.pill` fica só para badges, chips, barras de progresso e elementos circulares (botão
só de ícone, avatar). Botões em pill que já existem nos produtos são legado e migram quando
for conveniente. Decidido no Atria em 2026-10-30, quando os componentes começaram a ser
preparados para virar a biblioteca compartilhada.

**Regra prática**: todo produto novo importa o pacote de tema compartilhado em vez de
redeclarar essas cores. Desde 2026-11-10 o pacote é o `@ishtar-sink/vega` (0.1.0), extraído do `@atria/ui` e do
`@atria/theme`: os tokens ficam em `src/theme/tokens.ts` da [Vega](https://github.com/Ishtar-Sink/Vega),
com um comentário no topo apontando este documento como origem, e saem junto com os
componentes. O `packages/theme` do Nebula e do Atria é legado e migra para a Vega. Nenhum produto novo deve recriar um componente que já
existe nela. Um valor mudado no tema padrão da Vega muda em todos os produtos que o usam de
uma vez — é a garantia de que a paleta não diverge com o tempo. Um produto com paleta própria
(ver a subseção `2026-11`) continua importando a Vega e substitui só os valores do tema.

**Alternância de tema**: `data-theme="light" | "dark"` no elemento raiz, **padrão `light`**,
`prefers-color-scheme` respeitado só quando o usuário nunca escolheu explicitamente.

### White label: troca de marca por instância

> Decidida em 2026-11-10, no estudo de escopo do Synestia (`Ishtar-Sink/Synestia`,
> `docs/estudos/ESTUDO-001-plataforma-de-estudos.md`), o primeiro produto com white label.

Um produto pode permitir que **a instância de um terceiro** troque a marca, para que uma
escola ou um coletivo apareça para o próprio público com o próprio nome. O produto em si
continua com o próprio nome e o próprio tema (o padrão do Ishtar Sink, ou a paleta própria
do produto), que é o que aparece numa instalação sem configuração. O tema é uma escolha do
produto; o white label é uma escolha de quem hospeda.

O que a instância pode trocar, sempre pelo backoffice e sem mexer no código:

- nome, logo e ícone, inclusive o nome e o ícone do aplicativo instalado (manifesto do PWA
  gerado por instância);
- a **camada de marca**: `primary`, `primaryHover`, `primaryBright`, `primarySoft`,
  `primaryOn` e o gradiente `brand`, nos temas claro e escuro;
- textos institucionais (boas-vindas, rodapé, aviso de privacidade), domínio e contato.

O que **não** muda: fundos, superfícies, bordas, cores de estado (`success`, `warning`,
`danger`, `info` e os `*Soft`), sombras, raios, espaços, movimento e tipografia. Eles
continuam vindo do pacote de tema, e a troca acontece em tempo de execução, por variáveis CSS
que sobrescrevem só os tokens de marca.

Regras para qualquer produto que ofereça white label:

- **Contraste validado no backoffice.** A cor de marca que não passar em 4,5:1 (WCAG AA)
  sobre `bg` e `surface` é recusada para texto e aceita só como preenchimento, como já
  acontece com `#A855F7`. O backoffice calcula a razão e mostra o motivo da recusa; a marca
  de terceiros nunca deixa a interface ilegível.
- **O link para o código-fonte não pode ser removido.** A AGPL-3.0 garante a quem usa pela
  rede o acesso ao código da versão em uso, e isso continua valendo com a marca trocada. O
  crédito "feito com <produto>" vem ligado por padrão, mas é opcional.
- **Conteúdo exportado não carrega a marca da instância.** Pacotes trocados entre
  instâncias levam só o conteúdo.
- **Sem white label por padrão.** Um produto só oferece white label quando o uso por
  terceiros fizer parte do escopo dele, com esta seção como referência.

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

2. **Identidade visual**: montar a interface com a Vega (componentes e tema). Usar o tema
   padrão do Ishtar Sink, descrito abaixo, a menos que este produto tenha decidido uma paleta
   própria; nesse caso, criá-la com a API de tema da Vega, nos dois temas, com contraste AA
   verificado e o motivo registrado (ver a subseção `2026-11` do documento de identidade).
   - Valores vigentes desde 2026-10 (Flare): ver a subseção `2026-10` deste documento. Onde
     esta lista diverge, a subseção nova vale.
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
   - Raios de borda: 8/12/18/26px. Botões e seletores com 12px, o mesmo dos campos;
     pill só para badges, chips, progresso e elementos circulares.
   - Se houver itens sem imagem própria (cards, avatares, tags), gerar a cor a partir de
     um hash determinístico do id, não de estado salvo — ver "cor determinística por item"
     no doc de identidade.
```
