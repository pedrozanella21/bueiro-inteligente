# Bueiro Inteligente 🌧️

Protótipo de monitoramento de bueiros para ajudar a evitar alagamentos em Curitiba.

🔗 **Ver online:** https://pedrozanella21.github.io/bueiro-inteligente/

## O problema

Em dia de chuva forte, folhas e lixo entopem os bueiros e a água não escoa. Muitas vezes ninguém fica sabendo até a rua alagar.

## A ideia

- Uma grade tipo peneira no bueiro segura folha e sujeira, mas deixa a água passar
- Um sensor mede o quanto a grade está obstruída e avisa quando está enchendo
- Um mapa mostra a situação de cada ponto:
  - 🟢 **ok**: até 49% obstruído
  - 🟡 **atenção**: de 50% a 79%
  - 🔴 **crítico**: 80% ou mais
- A equipe de limpeza vê no mapa quais bueiros precisam de atendimento primeiro e marca como limpo depois do serviço

## Este protótipo

Os sensores são simulados: a cada 3 segundos o nível de cada bueiro sobe um pouco, como se a sujeira estivesse acumulando. A lista ao lado do mapa fica ordenada do mais crítico para o menos crítico.

Os pontos no mapa são exemplos com localização aproximada.

## Tecnologias

- HTML, CSS e JavaScript puro
- [Leaflet](https://leafletjs.com/) com mapa do OpenStreetMap

## Próximos passos

- Sensor físico com Arduino ou ESP32 (sensor ultrassônico) enviando os dados por Wi-Fi
- Guardar o histórico para saber quais bueiros entopem mais
- Avisar a equipe de limpeza automaticamente quando um ponto ficar crítico
