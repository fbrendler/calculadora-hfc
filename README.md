# Calculadora G-PON

Versão 0.70 — by BRENDLER™.

Calculadora simples do trajeto entre a NAP e a ONT do cliente. Abra `index.html` em um navegador; o arquivo é autossuficiente e pode ser publicado no Cloudflare Pages.

## Uso

Informe a potência RX na origem do trecho e a distância da fibra em metros. A tecnologia é G-PON e o cálculo é fixo no sentido downstream, da NAP até a ONT. Potência e distância começam em zero; a atenuação é fixa em 0,00023 dB/m. Nenhum passivo é adicionado inicialmente. O divisor 1:2 aplica 3,5 dB fixos; o resultado inclui perdas mínima/máxima dos passivos adicionados. A faixa de potência é mostrada sempre do melhor sinal para o pior. O botão Limpar restaura potência e distância para zero e esvazia a lista de passivos.

Com os valores iniciais em zero e sem passivos, o resultado é 0,00 a 0,00 dBm.

O comprimento de onda é 1490 nm. Os padrões informados são NAP/DIO RX: -25 a 0 dBm e ONT RX: -27 a -8 dBm. A potência de origem fica vermelha em -25 dBm ou abaixo; cada extremo da faixa estimada na ONT fica vermelho individualmente em -27 dBm ou menos.

As perdas dos passivos são fixas e não editáveis: cordão óptico, 1,0–1,6 dB; conector óptico, 0,5–0,8 dB; divisor 1:2, 3,5 dB; PTO, 0 dB. O divisor pode ser adicionado pelo mesmo menu dos demais passivos; no máximo um divisor é permitido por instalação.

## Relatar problemas

Use o botão Relatar problema na calculadora ou abra uma issue em https://github.com/fbrendler/calculadora-hfc/issues.

## Versionamento

Incrementar o número exibido no rodapé em 0.01 a cada solicitação de alteração implementada.
A faixa fixa mínima/máxima dos passivos é apresentada lado a lado na mesma linha.

O layout prioriza celulares: campos compactos em duas colunas, rótulos alinhados acima dos respectivos campos, potência e instrução lado a lado, botão de passivo junto ao seletor, resultados agrupados e faixas GPON recolhidas inicialmente para reduzir a rolagem. Espaçamentos verticais também são reduzidos em telas de até 700 px, mantendo os textos e os alvos de toque confortáveis.

As colunas da tabela de referência GPON podem ser redimensionadas arrastando suas divisórias. Abra a seção de referência e use as alças verticais destacadas no cabeçalho; também é possível ajustar a coluna selecionada com as setas do teclado.
