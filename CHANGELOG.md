---
tipo: changelog
data: 2026-10-22
produzido-por: cognitio.one
versao-core: 1.0
---

# Changelog

Todas as alterações relevantes deste projeto são documentadas neste arquivo.

O formato segue [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e o
versionamento adota [Semantic Versioning](https://semver.org/lang/pt-BR/).

---

## [1.0.0] — 2026-10-22

Versão inicial pública da skill, que segue em **piloto**: o método está em teste
no primeiro episódio de uma série.

### Higienização para uso público

- Tirados os dados de conta e de infraestrutura do autor (caminhos de disco,
  credenciais, nomes de máquina, orçamento), as decisões internas numeradas e
  datadas, os nomes de sistemas e de documentos internos, e a marca da série de
  origem. A série de exemplo ficou como "série sobre a história e os fundamentos
  da tributação".
- Toda remissão a documento que não está no pacote virou texto genérico dentro
  dele. A skill não remete a nada que o pacote não traga.
- Os oito livros do método são citados pelo título, autor, edição e ano, com
  frases curtas para comentário, conferidas no texto da edição indicada. O
  pacote não traz nenhum outro trecho, nem arquivo, ficha ou anotação dos livros.

### Acrescentado para a skill funcionar sozinha

- `SKILL.md`: os papéis ("Quem é quem"), um glossário curto ("Termos") e "O que
  você precisa ter".
- `CONTROLES.md` § G: o mínimo de uma conferência de fontes, para quem não tem
  uma etapa própria; § E: o formato do `DIREITOS.md` e os termos de uso dos
  geradores; § D, item 8: pessoa privada identificável.
- `DIRIGIR.md` § 2: o formato do `PLANO-VISUAL.md`; § 6: o método mínimo de voz,
  cenas e corte, em sete passos, com qualquer ferramenta.
- `MODELO-BIBLIA.md` § 5: a direção de arte mínima (os sete componentes, a
  paleta de marca, o catálogo de estilos por época, o orçamento de texto por
  quadro).
- Etapa 4: o `DESCRICAO.md` (descrição do vídeo e os três títulos do teste A/B),
  conferido na etapa 5.

### Corrigido na revisão antes de publicar

Revisão por leitor independente, que leu só este pacote, como um estranho.

- **Ordem do fecho** fixada num lugar só (`ESCREVER.md` § 3) e repetida igual na
  regra 8, na bíblia e nos controles: resposta, linha de descida, a frase única
  do convite e da referência final, o gancho em imagem (salvo o último episódio)
  e a tela final.
- **Paleta:** a paleta de marca é fixa; o que progride ao longo da série é a cor
  dominante das cenas. Antes, o texto dava a paleta como fixa e como exemplo de
  progressão.
- **Quando se confere o quê:** o roteiro e o texto da capa na etapa 2; o que
  mudou, as cartelas, a descrição e os títulos na etapa 5.
- **Amostras da bíblia:** as amostras de estilo e de voz da etapa 0, feitas com
  texto de teste, não esperam a conferência do roteiro; a imagem e a voz do
  episódio, sim.
- **Leituras de cada etapa:** `DIRIGIR.md` § 1 na etapa 0, `DIRIGIR.md` § 2 na
  etapa 1, `ESCREVER.md` § 5 na etapa 2.
- **Exibição a leigos:** o corte bruto, a duas pessoas que o responsável
  escolher, com ordem expressa dele, dito igual nos três lugares.
- **Palavras por minuto:** a conta foi refeita sobre os minutos de voz, já sem as
  pausas (cerca de 2.200 a 3.000 palavras num episódio de 20 min).
- **Citações:** atribuição explícita de "less can be more" (Rosenthal), "two
  things very fast" (Rosenthal, com o que são as duas coisas) e "Wild sound can
  be used to bring still images to life" (Bernard e Rabin); o *train* de Bernard
  definido na própria regra 1; a tradução dita como tradução.
- **Termos:** "trilha provisória" virou "voz provisória"; "diagrama de luz" virou
  diagrama "num estilo próprio fixado na bíblia"; "frase de valor e causa" e
  "sinopse em quatro peças" ligadas ao capítulo do McKee de onde vêm.
- **Disparo:** a descrição diz que a skill se chama pelo comando, coerente com
  `disable-model-invocation: true`.

### Licença

- Licenciada sob AGPL-3.0 (componente executável) e CC BY-SA 4.0 (obra textual),
  com termo adicional de atribuição pelo art. 7(b) da AGPL, nos termos do
  `NOTICE`.
