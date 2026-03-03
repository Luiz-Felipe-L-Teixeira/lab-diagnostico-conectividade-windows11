# Fluxo de Diagnóstico de Conectividade

Usuário relata: "Estou sem internet"

1. Executar ipconfig
   - Possui IP válido?
     - Não -> Problema de DHCP/Wi-Fi
     - Sim -> Prosseguir

2. Testar comunicação local
   - ping 127.0.0.1 (loopback IPv4 Address)
   - ping gateway

3. Testar comunicação externa
   - ping 8.8.8.8

4. Testar resolução de nome
   - ping google.com
   - nslookup google.com

5. Analisar rota
   - tracert 8.8.8.8

