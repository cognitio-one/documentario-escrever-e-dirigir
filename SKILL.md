---
name: documentario-escrever-e-dirigir
description: >
  Método para ESCREVER e DIRIGIR um episódio de série documental longa (de 15
  a 25 min) para o YouTube, feito de narração sobre animação e imagem gerada,
  sem filmagem ao vivo nem entrevista. Conduz sete etapas com portões de
  aprovação do responsável pela série: bíblia da série, escaleta, roteiro em
  duas colunas (a VOZ vem do redator da narração; a TELA é da direção), plano
  visual, briefs de figura e a capa, conferência de fatos e de direitos, e voz,
  cenas e corte. Regra central: nada inventado, e a reconstituição é dita como
  tal. Chamar por "/documentario-escrever-e-dirigir" e dizer a etapa: "bíblia
  da série documental", "escaleta do episódio N", "roteiro do episódio N",
  "plano visual do episódio", "briefs de imagem do episódio". Por si, não
  escreve a narração, não gera imagem, voz nem trilha e não publica: dirige
  quem faz.
disable-model-invocation: true
# --- proveniência ---
tipo: skill
data: 2026-10-22
produzido-por: cognitio.one
versao-core: 1.0
---

# Documentário: escrever e dirigir um episódio de série

**Estado:** piloto. O método vem de oito livros sobre roteiro, documentário, estrutura visual e montagem (lista no fim) e da prática de produção do autor, e está em teste no primeiro episódio de uma série. Use, meça e corrija.

## Para que serve
Fazer o espectador leigo, que assiste uma vez, sair de 20 minutos sabendo **uma** coisa nova sobre o tema e lembrando dela, por uma história verdadeira bem contada e uma imagem que muda junto com a história.

## Quem é quem
- **Responsável:** a pessoa dona da série. Aprova cada portão e é a única que publica.
- **Diretor:** o agente que conduz esta skill. Escreve a bíblia, a escaleta, a coluna TELA, o plano visual e os briefs, e confere tudo contra os controles.
- **Redator da narração:** escreve a coluna VOZ a partir da bíblia, da escaleta e das diretrizes de `ESCREVER.md` § 5. Pode ser uma pessoa ou o próprio assistente numa passada separada, só de escrita. O que não pode é a direção reescrever a voz no meio da tabela.
- **Conferência de fontes:** etapa independente de quem escreveu, que confere cada afirmação contra a fonte primária. `CONTROLES.md` § G traz o mínimo, se você não tiver uma etapa própria.
- **Base de pesquisa:** o material de onde a série tira os fatos (texto-base, fichas de obra, acervo de fontes), com um id para cada fato (`F-001`, `F-002`...) e a fonte primária ao lado.

## Termos
- **Bíblia da série:** o documento que fixa, uma vez, o que vale para todos os episódios.
- **Escaleta:** o esqueleto do episódio, bloco a bloco, antes do texto.
- **História A e história B:** a A é alguém concreto que quer algo contra um obstáculo, numa época; a B é a ideia que nasce ou muda ali.
- **Linha de descida:** a frase que traz o assunto ao presente (o que ficou daquilo hoje).
- **Gancho:** a pergunta do episódio seguinte, deixada aberta em imagem.
- **Cartelas:** os quadros de texto na tela. A **tela final** é a cartela de encerramento (bíblia § 6); o **cartão de fonte** é a linha "OBRA · lugar · ano" sobre o documento real.
- **Ficha de obra:** a anotação sobre uma obra da base de pesquisa: o que ela diz, onde, com a página.
- **Folha de contato:** uma grade de quadros pequenos (de uma cena, ou de várias figuras) para conferir tudo de uma vez.
- ***Assembly*, corte bruto, corte fino:** a primeira junção de tudo, na ordem; a versão com estrutura, clímax e ritmo; a versão travada.

## A série é obra própria
O arco, as perguntas e a dramaturgia são da série. A base de pesquisa serve de **matéria**: a série não adapta um texto pronto, capítulo por capítulo. Se a série remete a um projeto ou produto (um livro, um site, um curso), ele aparece num lugar só: a **referência final** de cada episódio (regra 8).

## Quando usar
Episódio de série documental longa, narrada, com imagem gerada. **Não usar** para vídeo curto, Reel, animação de um a dois minutos, filme de até 6 min ou aula em partes: esses formatos pedem roteiro curto, sem a estrutura de atos de 20 minutos.

## Como usar: as sete etapas
Ler o módulo da etapa antes de começá-la. Cada episódio tem a sua pasta (`<serie>-ep<N>/`). Cada etapa grava ali o seu arquivo e atualiza o `ESTADO.md` do episódio: o que foi feito, o que foi aprovado e por quem, o que falta e o próximo passo. Quem retoma o trabalho começa por ele.

| # | Etapa | Entrega | Quem | Ler | Portão |
|---|---|---|---|---|---|
| 0 | **Bíblia da série** (uma vez) | `BIBLIA.md` | diretor | `MODELO-BIBLIA.md`, `ESCREVER.md` § 5, `DIRIGIR.md` § 1 | responsável aprova |
| 1 | **Escaleta** | `ESCALETA.md` | diretor | `ESCREVER.md` §§ 1–4, `MODELO-ESCALETA.md`, `DIRIGIR.md` § 2, `CONTROLES.md` § A | responsável aprova |
| 2 | **Roteiro em duas colunas** | `ROTEIRO.md` | VOZ: redator da narração, com a bíblia, a escaleta e `ESCREVER.md` § 5 como entrada. A coluna VOZ é colada da versão aprovada da narração, e a conferência roda nessa versão, não na tabela. TELA: diretor | `DIRIGIR.md` § 3, `CONTROLES.md` § B | **conferência de fontes de todo o roteiro (a voz e todo texto da TELA: cartões, datas, mapas, legendas, diagramas) e do texto da capa** + ok do responsável, **antes** de gerar imagem e voz do episódio. As amostras de estilo e de voz da etapa 0, feitas com texto de teste, não contam |
| 3 | **Plano visual** | `PLANO-VISUAL.md` | diretor | `DIRIGIR.md` §§ 1–2, `CONTROLES.md` § C | junto com o roteiro |
| 4 | **Briefs de figura e de animação, a capa e a descrição** | `briefs/NN-*.md`, `briefs/00-capa.md` e `DESCRICAO.md` (a descrição do vídeo e os três títulos do teste A/B, pelo redator) | diretor; figuras por um gerador de imagem, **um gerador por vez**; o movimento é código (por exemplo, Manim) ou edição | `DIRIGIR.md` §§ 4–5, bíblia § 6-A | folha de contato de amostra e capa ao responsável |
| 5 | **Conferência** | reconferência do que mudou desde a etapa 2, das cartelas e do `DESCRICAO.md`; `DIREITOS.md` | conferência de fontes; direitos pelo diretor, com a lei de direitos autorais do país de publicação lida no texto oficial; a dúvida que o texto da lei não resolver vai ao responsável | `CONTROLES.md` §§ D, E e G | duas chaves, dadas nesta rodada: a conferência aprovada e o ok do responsável. Texto alterado depois volta à conferência |
| 6 | **Voz, cenas e corte** | voz, cenas, corte bruto → corte fino; cortes verticais | diretor, pelo método de `DIRIGIR.md` § 6: a voz da série (bíblia § 4), transcrição com tempo por palavra, cenas, render numa máquina própria, revisão independente, montagem | `DIRIGIR.md` §§ 5–6, `CONTROLES.md` § F | responsável aprova o corte fino |

**Custo:** antes das etapas 4 e 6, dar ao responsável a estimativa (número de figuras, minutos de render, cota de serviços pagos) e esperar o ok. Gasto não avisado é gasto não autorizado.

## Regras que não se dobram
1. **Uma pergunta por episódio**, dita em uma frase, que a narração faz de fato e o fecho responde. Ela é o título, o *train* (em Bernard, "the single thread [...] that drives your film forward") e o fio condutor (Rosenthal). O nome da série fica fora do título.
2. **De onde vem o fato:** a matéria sai da base de pesquisa, que serve para **achar**; a conferência vai à **fonte primária**, pela cadeia de evidências (cada fato com o seu id na base e a fonte primária ao lado). Trecho da base que ainda não foi conferido só entra depois de conferido. Fato sem fonte nessa base fica de fora. Ninguém estima.
3. **Nada inventado; reconstituição dita como tal.** A cena imaginada tem estilo visivelmente desenhado e leva a marca fixa RECONSTITUIÇÃO. A imagem gerada nunca imita foto, gravura ou documento de época: hachura e traço de gravura como estilo de desenho visível são permitidos; gravura de época simulada, não. O documento real entra como documento real, com a fonte na tela. É o teste de Jon Else, em Bernard e Rabin: "When the lights come on in the theater, what does the audience believe to be true?". Estilo que evoca época (um jornal do século XIX, por exemplo) só emoldura documento real citado, com a fonte na tela; nunca manchete, jornal ou documento inventado. **Pessoa histórica real** pode ser nomeada com o que a fonte diz dela, mas sem diálogo, pensamento ou rosto inventado como retrato. **Pessoa privada de hoje** (um cliente, um paciente, um conhecido) entra sem nome, cidade nem data que a identifiquem; fato histórico público entra com os dados da fonte. **Revelar ao público o uso de IA** na imagem e na voz (Nichols e Baron: "The question of disclosure [...] is key"); onde e como, pela prática: na tela final e na descrição do vídeo, com a redação fixada na bíblia. A imagem estilizada mostra que é construída e por isso não engana quanto à natureza da imagem (Honess Roe); o detalhe de época sem fonte continua vedado (`DIRIGIR.md` § 5, item 6).
4. **A voz acrescenta o que a tela não diz; a tela não repete a voz.**
5. **Direitos só por três vias:** obra gerada para o projeto (dentro dos termos de uso do gerador), domínio público verificado no acervo de origem, ou licença escrita. "Uso justo" não é plano. Nenhum dado pessoal de cliente ou de terceiro nos briefs. Trecho dos livros que você usou para estudar o método não entra no vídeo nem na descrição.
6. **Lote pesado numa máquina própria:** render e geração em lote rodam numa máquina feita para isso, um trabalho de GPU por vez, e não na máquina de uso diário.
7. **Não é aula com imagens.** Se a escaleta não tem história A com alguém que quer algo contra um obstáculo, ela volta. Os fundamentos do tema (filosóficos, jurídicos, científicos, conforme a série) entram como a **história B** dos episódios, por dentro da história, e não como episódios de conceito.
8. **Marca, capa, convite e referência final:** a série tem dono declarado na bíblia (pessoa, canal ou marca). Cada episódio tem capa própria. No fecho (a ordem completa está em `ESCREVER.md` § 3), depois da resposta e da linha de descida, vem **uma frase só**, que convida a se inscrever e curtir e, se houver, faz a referência final ao projeto ou produto a que a série remete, sem endereço falado: produto só no fecho, e em uma frase. O endereço vai na descrição do vídeo, e só quando estiver no ar (confira antes que o link responde). Se a profissão do dono tem regras de publicidade (advocacia e medicina, por exemplo), a referência passa por elas na conferência. Bíblia §§ 6, 6-A e 6-B.
9. **Estilo artístico pela direção de arte da série** (bíblia § 5): o estilo varia por época; ficam fixos a voz, a tela final, a paleta de marca, a tipografia e as marcas. Estilo novo só depois de protótipo aprovado pelo responsável (uma página HTML com amostras, por exemplo).
10. **A voz é prosa contínua de professor,** com as frases ligadas por conectivos. Frase curta demais e pausa em excesso soam picotadas, como quem fala e para, fala e para (`ESCREVER.md` § 5).
11. **Piloto e medida:** o episódio 1 é piloto. 28 dias depois de publicado, ler nas métricas da plataforma a curva de retenção, a duração média de visualização e a taxa de cliques da capa (CTR), comparando com os vídeos longos do canal, e só então fixar duração e cadência. Antes de publicar, o corte bruto vai a duas pessoas leigas que o responsável escolher, com a ordem expressa do responsável, porque é material não publicado (`CONTROLES.md` § F). Cada episódio rende cortes verticais de 1 a 2 min para Reels e Shorts.
12. **Os controles não atestam a si mesmos:** o `CONTROLES.md` respondido é instrumento do autor; não substitui a conferência de fontes nem prova nada.

## Exemplo
Série sobre a história e os fundamentos da tributação. Episódio 1: história A, o vencido e a quota do rei na Antiguidade oriental; história B, o que separa o tributo do saque; fecho, a pergunta que atravessa a série (força ou consentimento?). É exemplo de forma, não episódio aprovado: a pergunta e os fatos saem da bíblia, conferidos na fonte primária. Os exemplos dos módulos (o quinto da colheita entregue ao faraó, no Gênesis) vêm da mesma série.

## O que você precisa ter
- **A base de pesquisa** da série, com a fonte primária de cada fato. Sem ela, a etapa 1 não começa.
- **Um redator da narração** e **uma conferência de fontes** independentes da direção (veja "Quem é quem").
- **A direção de arte** da série: o mínimo vai na bíblia, § 5.
- **Ferramentas de produção, à sua escolha:** um gerador de imagem (um por vez); uma voz sintética ou gravada (nunca a imitação da voz de uma pessoa real); animação por código ou um editor; transcrição com tempo por palavra; um programa de montagem. A skill não exige nenhuma marca de ferramenta. Leia os termos de uso de cada gerador quanto a uso comercial e registre-os no `DIREITOS.md`.

## Os oito livros
O método cita os livros pelo código entre colchetes (L1 a L8); "prática" marca a regra que vem da experiência de produção do autor, e não dos livros. As frases curtas em inglês são citações para comentário, conferidas no texto destas edições; os capítulos e as páginas citados nos módulos também são destas edições. O pacote não traz nenhum outro trecho: para o resto, leia os livros.

- **L1** Robert McKee, *Story: substância, estrutura, estilo e os princípios da escrita de roteiro*, trad. Chico Marés (Arte & Letra, 2006).
- **L2** Sheila Curran Bernard, *Documentary Storytelling: Creative Nonfiction on Screen*, 3.ª ed. (Focal Press, 2011).
- **L3** Alan Rosenthal, *Writing, Directing, and Producing Documentary Films and Videos*, 3.ª ed. (Southern Illinois University Press, 2002).
- **L4** Bruce Block, *The Visual Story: Creating the Visual Structure of Film, TV, and Digital Media*, 3.ª ed. (Routledge, 2021).
- **L5** Sheila Curran Bernard e Kenn Rabin, *Archival Storytelling: A Filmmaker's Guide to Finding, Using, and Licensing Third-Party Visuals and Music* (Focal Press, 2009).
- **L6** Bill Nichols e Jaimie Baron, *Introduction to Documentary*, 4.ª ed. (Indiana University Press, 2024).
- **L7** Annabelle Honess Roe, *Animated Documentary* (Palgrave Macmillan, 2013).
- **L8** Walter Murch, *In the Blink of an Eye: A Perspective on Film Editing*, 2.ª ed. (Silman-James Press, 2001).

## O que esta skill não faz
Não escreve a narração: dirige quem escreve. Não decide questão de mérito da matéria (tese jurídica, científica ou histórica controvertida): a matéria vem da base de pesquisa, e a controvérsia é dita como controvérsia. Não gera imagem, voz nem trilha por si: dirige quem gera. Não publica: **a publicação na plataforma é ato manual do responsável**. Não altera a base de pesquisa. Não mostra material não publicado a terceiros sem ordem expressa do responsável.
