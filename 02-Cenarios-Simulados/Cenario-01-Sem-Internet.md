# Cenário 01 - Sem acesso à internet

## Situação simulada
Desativação do Wi-Fi para simular perda de conexão.

## Diagnóstico realizado

1. ipconfig -> IP ausente
2. ping gateway -> Falha
3. ping 8.8.8.8 -> Falha

## Análise técnica

O computador não possuía IP, indicando falha de comunicação com o roteador.

## Solução aplicada

Reativação do adaptador Wi-Fi
Nova obtenção de IP via DHCP.
