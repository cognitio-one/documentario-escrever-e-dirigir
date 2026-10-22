---
tipo: modulo-skill
data: 2026-10-22
produzido-por: cognitio.one
versao-core: 1.0
---

# Dirigir o episódio (tela, plano visual e briefs para o gerador)

Códigos de origem como em `ESCREVER.md`: L1 a L8 são os livros listados no `SKILL.md`; "prática" é a experiência de produção do autor.

## 1. A gramática visual da série (vai na bíblia, uma vez)
1. **Os sete componentes** são declarados para a série: espaço, linha, forma, tom, cor, movimento e ritmo. Nenhum fica ao acaso: "Left uncontrolled, the visual components can inadvertently contradict the story telling, mislead the audience, or simply bore them". [L4]
2. **Fixos da série** (não mudam nunca): a voz, a tela final, a paleta de marca (as cores da identidade da série, usadas na tela final, nas marcas e nos cartões), a tipografia, a marca RECONSTITUIÇÃO e o cartão de fonte. **O estilo artístico varia por época**, pelo catálogo de estilos da bíblia (§ 5); dentro de um episódio, o estilo é um só. Estilo novo, só depois de protótipo aprovado. Estilo que evoca época (um jornal do século XIX, por exemplo) só emoldura documento real citado. [L4, a constante; prática]
3. **Progressão do arco** (muda de episódio a episódio, devagar): por exemplo, a cor dominante das cenas, da terra e do ouro da Antiguidade ao azul e ao cinza do Estado fiscal, **dentro** da identidade visual da marca da série, que prevalece em tipografia e cor. A paleta de marca não muda; o que progride é a cor das cenas. Decisão do responsável na bíblia. [L4, a progressão]
4. **Exposição visual no episódio 1:** cada convenção é ensinada uma vez, com a voz se precisar, e depois dispensa explicação (o documento real tem moldura e cartão; a reconstituição tem a marca; o conceito é diagrama, num estilo próprio fixado na bíblia). [L4; prática]
5. **Contra o estereótipo:** o sentido de uma cor ou de uma linha é o que a série fixa, não o de tabela. [L4]
6. **A função da imagem em cada plano:** substituir o que não foi filmado sem imitar foto (a cena histórica) ou evocar o que não tem aparência (um fundamento: consentimento, confisco, capacidade). Nas duas, o estilo visivelmente construído é virtude. Imitar a imagem fotográfica é o lado do engano, e a prova mora em outro lugar: a voz que nomeia a fonte, o documento real com cartão, a descrição. O estilizado aciona mais a emoção, e o realista, o intelecto (estudo citado pela autora, p. 108). [L7]

## 2. O plano visual do episódio
1. **Lista de sequências** com a função de cada uma: EX (exposição), CO (conflito), CX (clímax), R (resolução). [L4]
2. **Gráfico da história:** intensidade de 0 a 100 nos 20 minutos, tirado da escaleta. Embaixo, na mesma escala, **as curvas de um ou dois componentes** (por exemplo, saturação e espaço: plano e afinidade na exposição, profundo e contraste no clímax). [L4]
3. **Contraste e afinidade:** o contraste sobe a intensidade, a afinidade a baixa. Pico de contraste no clímax; afinidade na resolução e nas pausas. [L4]
4. ***Color script*** do episódio: uma faixa de quadros pequenos com a cor de cada sequência. [L4]
5. **Batidas da direção:** em cada mudança de intenção do texto, algo muda na tela (enquadramento, luz, cor). [L4]
6. **Para onde o olho vai:** a cada corte, saber onde está o ponto de atenção e se o corte o leva por afinidade (suave) ou por contraste (choque). [L4]

Formato do `PLANO-VISUAL.md`:
- a lista de sequências: `| Seq. | Blocos | Tempo | Função (EX, CO, CX, R) | Intensidade (0–100) | Componente 1 | Componente 2 | Cor dominante (código) |`;
- o gráfico da história, tirado dessa tabela (uma imagem, ou a própria coluna de intensidade);
- o *color script*: a coluna de cor dominante, na ordem das sequências, com uma amostra de cor por sequência se a ferramenta permitir;
- as batidas da direção e os cortes de contraste, marcados pelo número do bloco.

## 3. O roteiro em duas colunas
Formato fixo do `ROTEIRO.md`, bloco a bloco [L3]. A linha abaixo é só **exemplo de formato**: a frase da voz não foi conferida e não vai a roteiro nenhum assim. Na coluna Fonte, a fonte primária e, depois da seta, o id do fato na base de pesquisa.

| # | Tempo | TELA (direção) | VOZ (redator) | SOM | Fonte |
|---|---|---|---|---|---|
| 07 | 4:10–4:35 | Plano geral, espaço profundo, poente ocre; celeiro do Egito reconstituído (RECONSTITUIÇÃO); a câmera desce até um saco de grãos dividido em cinco | "Um quinto da colheita ia para o rei, e ninguém tinha votado por isso, porque naquela terra a parte do rei vinha antes da parte de quem plantava." | vento, grãos | Gênesis 47,24–26 (Vulgata) → F-001 |

Em cada bloco, as **quatro perguntas** [L3]: que ponto este bloco prova? o que a tela **mostra** para prová-lo? o que os elementos fazem? como o som e a voz ajudam?

## 4. O brief de figura e de animação
O gerador de imagem (um por vez, nunca dois em paralelo) entrega figuras e cenários; o movimento é código (por exemplo, Manim) ou edição, pelos §§ 5 e 6. Numa série em teatro de sombras, o gerador fez silhuetas isoladas, preto sobre branco, e o céu e a luz saíram do código. Toda figura gerada é conferida com os olhos antes de entrar. [prática]

Um arquivo por plano, ou por grupo de planos com o mesmo cenário, com estes campos:
1. **Bloco e tempo**, e a frase da voz que corre por cima (para a imagem **não** repeti-la).
2. **O que se vê**, em uma frase, e **o que muda** durante o plano (movimento de objeto, de câmera ou de atenção). [L4]
3. **Componentes:** espaço (plano, profundo, limitado), linha dominante, forma, faixa de tom, paleta (os códigos da bíblia), movimento e ritmo. [L4]
4. **Natureza:** RECONSTITUIÇÃO (estilizada, nunca fotorrealista de época), DOCUMENTO REAL (o arquivo de origem, com a licença ou o domínio público verificado) ou DIAGRAMA (conceito). [L3, L5; prática]
5. **Proibido neste plano:** rosto de pessoa real inventado como retrato; documento falso com ar de autêntico; texto ilegível; qualquer marca, pessoa ou empresa atual. [L5, ética; prática]
6. **Texto na tela**, se houver: no máximo quatro elementos legíveis por quadro, fora da faixa inferior de 15% da tela. [prática]
7. **Duração e tamanho:** 16:9, 1080p ou 4K; a duração tirada da voz gravada ou da voz provisória (a leitura de trabalho). [L4: "find the verbal rhythm first"]

O brief da capa (`briefs/00-capa.md`) usa os mesmos campos, mais as regras da bíblia § 6-A.

## 5. Imagem parada, documento e som
1. **Movimento sobre a imagem** (pan e zoom lentos), camadas separadas com paralaxe e **movimento ambiente**, para nenhuma tela ficar parada mais de 3 s com a voz andando. [L5; prática]
2. **Som de ambiente sobre a imagem parada** dá vida; nas palavras de Bernard e Rabin, "Wild sound can be used to bring still images to life". [L5]
3. **Música** sem competir com a voz; nunca uma frase musical bonita sob a narração. [L3; L2]
4. O ritmo da voz manda: grava-se a voz (ou a voz provisória) e a imagem se corta pela voz. [L4]
5. **Animar é animar a imagem aprovada, sem redesenhar o cenário.** A regra veio de um teste reprovado, em que a animação trocou o cenário inteiro. Vídeo gerado, só em poucos momentos-chave: o mínimo possível. Método [prática]: recortar em camadas a própria imagem aprovada (máscara, preenchimento, ou edição do gerador com ela como referência) e comparar o quadro 0 com a imagem aprovada antes de seguir, porque a edição do gerador pode redesenhar o cenário.
6. **Imagem gerada inventa detalhe de época** (num teste, lingotes com cara de modernos numa cena antiga): objeto de época vai genérico ou com fonte; detalhe específico sem fonte é o mesmo engano do fotorrealismo. [prática, com base em L7]

## 6. Voz, cenas e corte
O método mínimo, com qualquer ferramenta:
1. **Voz por cena:** a voz da série (bíblia § 4), um arquivo por cena, a partir da coluna VOZ conferida.
2. **Tempos por palavra:** transcrição automática do áudio com tempo por palavra (por exemplo, Whisper), sem passar o texto do roteiro ao transcritor. Os tempos marcam onde cada imagem entra e onde o corte cai.
3. **Cenas** (animação por código ou editor), conferidas em folhas de contato (uma grade de quadros de cada cena) antes do render final.
4. **Render numa máquina própria**, um trabalho de GPU por vez; nada pesado na máquina de uso diário.
5. **Revisão independente** das cenas, por outra pessoa ou outro modelo, antes da montagem.
6. **Montagem:** música e efeitos sincronizados pela voz, normalização de volume, legendas tiradas da transcrição, e o pacote de publicação (vídeo, legendas, capa, e o título e a descrição do `DESCRICAO.md` conferido).
7. **Cortes verticais** de 1 a 2 min para Reels e Shorts, tirados do corte fino.

**Onde e como cortar** [L8]: a ordem do corte é emoção, história, ritmo, rastro do olho, plano da tela e continuidade do espaço; se for preciso sacrificar, sacrifica-se de baixo para cima. O corte cai quando o espectador "pegou" a ideia da frase, nem antes nem depois: na série, no fim de uma ideia da voz, marcado pela sincronia por palavra. Murch trata a televisão como tela de "olhar para" ("a 'look-at' medium") e o cinema como tela de "olhar dentro" ("a 'look-into' medium"). Aplicado ao YouTube, pela prática: a mudança está no movimento e no enquadramento dentro da imagem aprovada, e não em mais imagens nem em mais vídeo gerado. A regra de Murch de montar primeiro sem som não vale aqui: a voz vem antes (L4).

*Assembly* → corte bruto (estrutura, clímax, ritmo) → corte fino (travado). Entrar no bloco o mais tarde e sair o mais cedo possível. Exibir o corte bruto a quem não conhece o assunto, **só com ordem expressa do responsável e para pessoas que o responsável escolher** (é material não publicado); se a mensagem recebida não for a enviada, há problema. [L3; L2]
