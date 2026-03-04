# cenário 02 - Falha de DNS

## Situação Simulada
Alteração manual do DNS para um endereço inválido (10.10.10.10), mantendo a conexão Wi-Fi ativa.

## Diagnóstico Realizado

1. ipconfig -> IP válido obtido via DHCP
2. ping gateway -> Sucesso
3. ping 8.8.8.8 -> Sucesso
4. ping google.com -> Falha
5. nslookup google.com -> DNS request timed out

## Análise Técnica

A conectividade com o roteador e com a internet estava funcional. Entretando, o sistema não conseguia resolver nomes de domínio.

Isso caracteriza falha na resolução DNS.

O problema não estava na conexão física ou no provedor, mas na configuração incorreta do servidor DNS.

## Solução Aplicada

Configuração do DNS revertida para automático.
Nova validação com:

- ping google.com -> Sucesso
- nslookup google.com -> Resolução correta


