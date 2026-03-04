# Cenário 03 - Site acessível por IP, mas não por nome

## Situação simulada
Simulação de falha na resolução de nomes mantendo conectividade ativa.

## Diagnóstico Realizado

1. ipconfig -> IP válido
2. ping gateway -> Sucesso
3. ping 8.8.8.8
4. ping google.com -> Falha
5. nslokuup google.com -> Retorna IP válido
6. ping (IP retornado pelo nslookup) -> Sucesso

## Análise Técnica

A conectividade com a internet estava operacional.
O acesso ao servidor externo por IP funcionava normalmente.

A falha ocorria apenas na conversão de nome para IP, caracterizando problema de DNS.

Este tipo de ocorrência é comum quando:
- DNS está configurado incorretamente
- Cache DNS está corrompido
- Servidor DNS está indisponível

## Solução Aplicada

Correção da configuração de DNS
Execução do comando:

ipconfig/flushdns

Validação final com:

- ping google.com -> Sucesso
- Navegação normalizada
