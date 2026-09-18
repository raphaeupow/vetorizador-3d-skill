# Referencia: Placa Chrysler

Este caso vem da conversa que originou a skill e deve ser usado como teste visual quando o usuario pedir o mesmo tipo de preparacao.

## Arquivos

- `assets/chrysler-reference-landscape.jpg`: foto principal em orientacao horizontal.
- `assets/chrysler-reference-portrait.jpg`: foto alternativa em orientacao vertical.
- `assets/known-issue-secondary-text-scale.png`: captura de um resultado anterior em que o texto secundario ficou com proporcao incorreta.

## Elementos Visiveis

- Base retangular preta com cantos arredondados.
- Borda externa e filetes/moldura em relevo ou baixo-relevo, pouco contrastantes na foto.
- Simbolo Chrysler a esquerda.
- Texto principal claro: `CHRYSLER`.
- Texto secundario claro: `do BRASIL S.A.`
- Texto em baixo-relevo/preto sobre preto: `12 VOLTS 75 AMP, HORA`.
- Texto em baixo-relevo/preto sobre preto: `PECA Nº 71304259`.
- Texto inferior em baixo-relevo/preto sobre preto: `ACUMULADORES VULCANIA S.A.`
- Circulo/furo na regiao inferior esquerda-central.

## Falhas Que Devem Ser Evitadas

- Reduzir demais `ACUMULADORES VULCANIA S.A.` em relacao a placa.
- Transformar borda, baixo-relevo ou texto preto sobre preto na mesma cor da base.
- Usar sombra, textura ou brilho para representar relevo.
- Inventar caracteres quando a foto nao permitir leitura segura.
- Entregar apenas um arquivo geral quando as partes precisam ser separadas.

## Cores Sugeridas Para Separacao

As cores podem mudar conforme a arte, mas devem ser claramente distintas. Uma paleta pratica:

- Base: branco ou cinza muito claro no PNG geral quando a base precisa contrastar.
- Borda/moldura: magenta.
- Simbolo Chrysler: ciano.
- Texto principal: azul.
- Texto `do BRASIL S.A.`: verde.
- Texto `12 VOLTS 75 AMP, HORA`: amarelo.
- Texto `PECA Nº 71304259`: laranja.
- Texto `ACUMULADORES VULCANIA S.A.`: vermelho.
- Circulo/furo: roxo.
- Ambiguidades: cinza com nomeacao explicita no arquivo.

Nao use essas cores para simular a aparencia final da peca. Elas sao uma mascara tecnica para separacao no Inkscape.
