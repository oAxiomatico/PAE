# Didática na matemática e computação

Versão inicial para discussão e ensaio do grupo. Público: pós-graduandos em preparação para a docência no ensino superior. São 20 slides de conteúdo, sem capa separada, e duas páginas de referências. Inserir nomes no campo `author` do arquivo LaTeX.

## Arquivos e compilação

- `apresentacao.tex`: fonte Beamer, formato 16:9, editável também no Overleaf.
- `apresentacao.pdf`: versão compilada.
- `roteiro.md`: divisão de tempo, notas para falar e ensaiar.
- `fontes.md`: correspondência entre as oito referências e seus usos.

Com uma distribuição TeX Live contendo Beamer e Latin Modern:

```sh
cd /workspace/PAE/seminario
mkdir -p /tmp/pae-beamer
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp/pae-beamer apresentacao.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp/pae-beamer apresentacao.tex
cp /tmp/pae-beamer/apresentacao.pdf .
```

A versão foi compilada com pdfLaTeX. Não requer shell-escape, imagens externas ou BibTeX. O texto usa UTF-8 e fontes T1; a hifenização automática está desativada para não depender do pacote de idioma português indisponível nesta máquina.

## Recorte e limites

Tese: ensinar envolve organizar condições para compreender, justificar e transferir conhecimentos, articulando objetivos, conteúdo, mediação e avaliação. As fontes fundamentam a discussão; as tarefas e a rubrica são propostas do grupo, não resultados experimentais dos autores. Não foram usadas referências externas às oito fornecidas. A síntese não substitui a leitura integral dos livros e relatórios.

Os documentos curriculares são tratados como documentos fornecidos para análise, sem afirmar que representam toda a legislação vigente. Alves discute também educação básica: a aplicação ao ensino superior é uma adaptação explícita. Borba (2021) não é usado como evidência de eficácia de IA generativa. O relatório da SBC é uma agenda de desafios, não uma revisão de eficácia de métodos.
