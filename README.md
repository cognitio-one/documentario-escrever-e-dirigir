---
tipo: readme
data: 2026-10-22
produzido-por: cognitio.one
versao-core: 1.0
---

# Documentário: escrever e dirigir

> Skill para assistentes de IA. Conduz a escrita e a direção de um episódio de
> série documental longa (de 15 a 25 minutos) para o YouTube, feito de narração
> sobre animação e imagem gerada, sem filmagem ao vivo nem entrevista.

Com imagem gerada, fazer um vídeo de 20 minutos ficou fácil. O difícil continua
sendo o resto: uma história que segura o espectador leigo até o fim e uma imagem
que não mente. O vídeo gerado falha de dois jeitos previsíveis. Vira **aula com
imagens**, em que a voz explica e a tela ilustra o que a voz já disse. Ou vira
**engano**, com a cena inventada passando por registro de época, o detalhe sem
fonte, o documento que nunca existiu.

Esta skill organiza o trabalho para evitar os dois. Ela não escreve a narração
nem gera imagem: **dirige** quem faz, em sete etapas, cada uma com um portão
que só o responsável pela série abre.

## As sete etapas

| # | Etapa | Entrega |
|---|---|---|
| 0 | Bíblia da série (uma vez) | voz, gramática visual, marcas, capa, convite, o que é proibido |
| 1 | Escaleta | a pergunta do episódio, as histórias A e B, os tempos, o gráfico de intensidade |
| 2 | Roteiro em duas colunas | TELA (direção) × VOZ (redator), bloco a bloco, com a fonte de cada fato |
| 3 | Plano visual | sequências, curvas dos componentes visuais, *color script* |
| 4 | Briefs de figura e de animação, a capa e a descrição | um brief por plano para o gerador de imagem; a descrição e os títulos do teste A/B |
| 5 | Conferência | os fatos contra a fonte primária; os direitos de cada imagem, som e música |
| 6 | Voz, cenas e corte | do *assembly* ao corte fino, e os cortes verticais |

Nenhuma imagem ou voz do episódio se gera antes de o roteiro inteiro passar pela
conferência de fontes: a voz e todo texto da tela, inclusive cartões, datas,
mapas e legendas. As amostras de estilo e de voz da bíblia, feitas com texto de
teste, vêm antes.

## As regras que seguram o método

**Uma pergunta por episódio.** Dita em uma frase, ela é o título, o fio
condutor e o que o fecho responde.

**Não é aula com imagens.** Toda escaleta tem uma história A, com alguém que quer
algo contra um obstáculo, e uma história B, com a ideia que nasce ou muda ali. O
conceito entra por dentro da história.

**Nada inventado; reconstituição dita como tal.** A cena imaginada tem estilo
visivelmente desenhado e a marca RECONSTITUIÇÃO. A imagem gerada nunca imita
foto, gravura ou documento de época. O documento real entra como documento
real, com a fonte na tela. É o teste de Jon Else: quando as luzes acendem, o que
o público acredita que é verdade?

**O uso de IA é revelado** ao público, na tela final e na descrição do vídeo.

**Direitos só por três vias:** obra gerada para o projeto, domínio público
verificado ou licença escrita. "Uso justo" não é plano.

**A voz acrescenta o que a tela não diz; a tela não repete a voz.**

## O que vem no pacote

| Arquivo | O que é |
|---|---|
| `SKILL.md` | as sete etapas, os papéis, as doze regras, a lista dos livros |
| `ESCREVER.md` | da matéria à pergunta, as histórias, a estrutura de 20 minutos, as diretrizes da voz |
| `DIRIGIR.md` | a gramática visual, o plano visual, o roteiro em duas colunas, o brief, a imagem parada e o som, a voz, as cenas e o corte |
| `CONTROLES.md` | as perguntas de controle de cada portão, o formato do `DIREITOS.md` e o mínimo de uma conferência de fontes |
| `MODELO-BIBLIA.md` | o molde da bíblia da série, com a direção de arte mínima |
| `MODELO-ESCALETA.md` | o molde da escaleta de cada episódio |

## Instalação

```bash
git clone https://github.com/cognitio-one/documentario-escrever-e-dirigir.git \
  ~/.claude/skills/documentario-escrever-e-dirigir
```

Skills seguem o padrão aberto [Agent Skills](https://agentskills.io).

## Como usar

`/documentario-escrever-e-dirigir`, e diga em que etapa está: "bíblia da série
documental", "escaleta do episódio 3", "roteiro do episódio 3", "plano visual
do episódio", "briefs de imagem do episódio".

A skill é chamada só pelo comando (`disable-model-invocation: true`): é um
trabalho longo e com custo, e não deve começar sozinho.

## O que você precisa ter

- **Uma base de pesquisa** com a fonte primária de cada fato. A skill não
  pesquisa: ela exige que a matéria já exista e seja conferível.
- **Um redator da narração**, pessoa ou o próprio assistente numa passada
  separada, só de escrita.
- **Uma conferência de fontes** feita por quem não escreveu. O `CONTROLES.md`
  traz o mínimo, se você não tiver uma etapa própria.
- **Ferramentas de produção à sua escolha:** gerador de imagem, voz sintética ou
  gravada, animação por código ou editor, transcrição com tempo por palavra,
  montagem. A skill não exige nenhuma marca de ferramenta.

## O que não faz

- Não escreve a narração nem gera imagem, voz ou trilha: dirige quem faz.
- Não pesquisa a matéria nem decide questão de mérito (tese jurídica, científica
  ou histórica controvertida).
- Não publica. A publicação é ato manual do responsável pela série.
- Não serve para vídeo curto, Reel ou aula em partes: é para o formato longo.

## Executa sozinha

Não depende de outra skill. Tudo o que o método pede está nos seis arquivos do
pacote.

## Os livros

O método vem de oito livros sobre roteiro, documentário, estrutura visual e
montagem: McKee, *Story*; Bernard, *Documentary Storytelling*; Rosenthal,
*Writing, Directing, and Producing Documentary Films and Videos*; Block, *The
Visual Story*; Bernard e Rabin, *Archival Storytelling*; Nichols e Baron,
*Introduction to Documentary*; Honess Roe, *Animated Documentary*; e Murch, *In
the Blink of an Eye*. As edições estão no `SKILL.md`. O pacote cita só frases
curtas, para comentário; o resto está nos livros.

## Exemplo

Os exemplos vêm de uma série sobre a história e os fundamentos da tributação: o
quinto da colheita entregue ao faraó, a pergunta "força ou consentimento?". São
exemplos de forma, não episódios aprovados.

## Licença

Licenciamento duplo, ambos copyleft, ambos com **atribuição nominal
obrigatória**: **[AGPL-3.0](LICENSE)** e **[CC BY-SA 4.0](LICENSE-DOCS)**. Uso
próprio não gera obrigação; distribuir ou servir a terceiros exige abrir o
código e manter a atribuição. O [NOTICE](NOTICE) é parte da licença.

## Autor

**cognitio.one**
[github.com/cognitio-one](https://github.com/cognitio-one)

Histórico de versões no [CHANGELOG](CHANGELOG.md).
