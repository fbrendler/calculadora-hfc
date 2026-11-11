# Calculadora HFC

Versão 0.20 — by BRENDLER™.

Calculadora de atenuação para cabos RG6 e RG11, divisores e DCs.

## Uso

Abra `index.html` em um navegador. Selecione onde o sinal foi medido (TAP/DG ou Ponto), preencha os sinais disponíveis, informe a metragem e adicione os passivos com as saídas utilizadas. O cálculo ocorre automaticamente no sentido correspondente.

Os sinais são opcionais. Metragem vazia equivale a zero metro. Os coeficientes dos cabos são fixos; a atenuação dos passivos é somada em série. As cores e avisos seguem os limites definidos para cada destino.

## Publicação

O arquivo `index.html` é autossuficiente e pode ser enviado ao Cloudflare Pages. Manter este repositório privado preserva o acesso ao histórico no GitHub; um site público ainda entrega seu HTML e JavaScript ao navegador dos visitantes.

## Versionamento

Incrementar o número exibido no rodapé em 0.01 a cada solicitação de alteração implementada.
