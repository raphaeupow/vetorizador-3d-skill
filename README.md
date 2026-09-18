# Vetorizador 3D

Skill para preparar fotos de placas, logos e emblemas para vetorizacao 3D no Inkscape.

Ela orienta o Codex a produzir PNGs de alta resolucao, com perspectiva corrigida, cores solidas separadas por camada e sem inventar detalhes ilegíveis. O foco e facilitar a selecao por cor no Inkscape, inclusive em casos de relevo ou baixo-relevo preto sobre preto.

## Saidas esperadas

- PNG geral em alta resolucao, sem textura, sombra ou brilho.
- PNGs separados por camada/parte, preferencialmente com fundo transparente.
- Cores solidas distintas para base, borda, relevo, baixo-relevo, simbolo, textos e furos.
- ZIP quando houver muitos arquivos.
- Nota de ambiguidades para trechos pouco legiveis.

## Caso de teste

O caso de referencia e uma placa Chrysler do Brasil S.A. com textos em relevo e baixo-relevo, incluindo:

- `CHRYSLER`
- `do BRASIL S.A.`
- `12 VOLTS 75 AMP, HORA`
- `PECA Nº 71304259`
- `ACUMULADORES VULCANIA S.A.`

O texto `ACUMULADORES VULCANIA S.A.` e um ponto critico: ele nao deve ser reduzido ou redesenhado fora da proporcao original.

## Estrutura

- `SKILL.md`: instrucoes principais da skill.
- `references/chrysler-reference.md`: checklist especifico do caso Chrysler.
- `assets/`: imagens de referencia anexadas na conversa original.
