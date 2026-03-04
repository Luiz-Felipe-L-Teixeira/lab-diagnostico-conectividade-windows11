# Cenário 04 - Conectado ao Wi-Fi, mas sem navegação

## Situação Simulada
Manutenção da conexão Wi-Fi ativa com simulçao de falha na saída para internet.

## Diagnóstico Realizado

1. ipconfig -> IP válido
2. ping gateway -> Sucesso
3. ping 8.8.8.8
4. tracert 8.8.8.8 -> Interrupção após primeiro salto (roteador)

## Análise Técnica

O computador estava corretamente conectado à rede local.
A comunicação com o roteador era funcional.

Entretando, não havia resposta de servidores externos.

O teste com tracert indicou que a falha ocorria após o roteador, sugerindo:

- Problema no provedor de internet
- Instabilidade no modem
- Bloqueio externo de tráfego

## Solução Aplicada

Reinicialização do roteador/modem.
Aguardar restabelecimento do link com o provedor.
Validação com:

- ping
- 8.8.8.8 -> Sucesso
- Navegação normalizada
