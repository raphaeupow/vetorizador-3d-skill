---
name: vetorizador-3d
description: Preparar fotos de placas, logos e emblemas para vetorizacao 3D no Inkscape, gerando PNG geral corrigido e PNGs separados por camada com cores solidas distintas.
metadata:
  short-description: PNGs separados para vetorizacao 3D
---

# Vetorizador 3D

Use esta skill quando o usuario enviar fotos de placas, logos, emblemas ou pecas com letras/simbolos em relevo ou baixo-relevo e quiser preparar imagens para separar por cor no Inkscape, corte, CNC, impressao 3D ou modelagem 3D.

O resultado principal e um conjunto de PNGs, nao SVG. O SVG so deve ser oferecido se o usuario pedir explicitamente.

## Resultado Esperado

Entregue:

- Um PNG geral em alta resolucao, com a placa/logo em vista frontal, perspectiva corrigida, sem textura, sem brilho, sem sombra e sem simulacao de relevo.
- Cores solidas e distintas para todos os elementos separaveis: base, simbolo, texto principal, cada grupo de texto secundario, borda, relevo, baixo-relevo, circulo/furo e qualquer detalhe preto sobre preto.
- PNGs separados por parte/camada, preferencialmente com fundo transparente.
- Um ZIP quando houver muitos PNGs ou quando isso deixar a entrega mais organizada.
- Uma nota curta de ambiguidades quando qualquer texto ou detalhe nao estiver legivel o suficiente.

Nao invente letras, numeros, marcas ou ornamentos ilegiveis. Preserve o que for visivel, isole o ambiguo como area/camada de revisao ou peca foto melhor.

## Regras Criticas

- Preserve proporcoes relativas reais. Nao redesenhe textos secundarios menores ou maiores por conveniencia.
- De atencao especial ao texto `ACUMULADORES VULCANIA S.A.`: no caso de referencia Chrysler, ele deve manter a largura, altura, espessura aparente e posicao proporcional observadas na placa, nao a versao reduzida do teste anterior.
- Toda borda deve ter cor propria e destacada. A borda nao deve sumir em preto sobre fundo preto.
- Todo relevo e baixo-relevo precisa de cor diferente da base, mesmo quando na foto original ele aparece preto sobre preto.
- Use cores chapadas, sem gradiente, textura, iluminacao, sombras ou highlights.
- Corrija a perspectiva antes de separar camadas, usando a geometria da placa como guia.
- Mantenha a orientacao final natural de leitura, salvo pedido contrario.
- Quando a foto tiver distorcao, sujeira, reflexo ou dedo cobrindo parte da peca, sinalize a limitacao.

## Camadas Recomendadas

Adapte os nomes as pecas reais, mas prefira separar:

- `00-geral`: composicao completa em alta resolucao.
- `01-base`: formato externo da placa ou fundo principal.
- `02-borda`: borda externa, filetes e molduras.
- `03-simbolo`: simbolo ou logomarca.
- `04-texto-principal`: nome/marca maior.
- `05-texto-secundario-grupo-1`, `06-texto-secundario-grupo-2`, etc.
- `relevo` e `baixo-relevo`: quando a peca tiver elementos tecnicamente diferentes.
- `circulo-furo`: furos, circulos ou marcas circulares.
- `ambiguidade`: areas ilegíveis ou que exigem confirmacao.

Use fundo transparente nos PNGs individuais sempre que possivel. No PNG geral, use fundo transparente ou branco neutro conforme for mais util para visualizacao; avise qual foi usado.

## Fluxo De Trabalho

1. Inspecione a foto original e identifique a area util da placa/logo.
2. Corrija perspectiva, rotacao e enquadramento sem mudar proporcoes internas.
3. Remova textura, sombra e reflexo do resultado final; mantenha apenas formas solidas.
4. Atribua uma cor distinta por parte/camada. Escolha cores com contraste forte entre si para facilitar selecao por cor no Inkscape.
5. Preserve tamanho relativo, alinhamento, espessura visual e espacamento dos textos.
6. Separe as camadas em PNGs individuais com nomes claros.
7. Gere um PNG geral em resolucao alta o bastante para vetorizacao, preferencialmente pelo menos 3000 px no maior lado quando a entrada permitir.
8. Se houver muitos arquivos, entregue tambem um ZIP.
9. Inclua uma lista breve de ambiguidades ou trechos que nao foram inferidos.

## Caso De Referencia Chrysler

Leia [references/chrysler-reference.md](references/chrysler-reference.md) quando o pedido mencionar Chrysler, placa de bateria, teste da conversa anterior, `ACUMULADORES VULCANIA S.A.` ou problemas com texto secundario/borda/relevo preto sobre preto.

As imagens de referencia ficam em `assets/` e servem para comparar proporcao, separacao por camadas e falhas que devem ser evitadas.
