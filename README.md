# PAM Segurança: Assistente de Segurança Pessoal (MIT App Inventor)

App que simula uma central de segurança pessoal: botão SOS com confirmação e contagem regressiva, localização por GPS, sirene, vibração, lanterna de tela, checklist de segurança, contatos de confiança e histórico de eventos da sessão.

## Conteúdo

| Arquivo | O que é |
|---|---|
| `guia/guia-pam-seguranca.html` | Guia passo a passo com imagens de todos os blocos e maquetes de cada tela. Abra no navegador. |
| `assets/sirene.wav` | Som de sirene (2 s, toca em loop) para enviar em **Media → Upload File** no App Inventor. |

## Telas

1. `Screen1`: menu de navegação e resumo
2. `TelaSOS`: botão de emergência com confirmação, contagem de 5 s e estados com cores
3. `TelaLocalizacao`: latitude e longitude, abertura no mapa, tratamento de GPS desligado, sem sinal e permissão negada
4. `TelaAlertas`: sirene, piscar, vibração, lanterna de tela e botão para parar tudo
5. `TelaChecklist`: 6 itens, barra de progresso calculada por programação e botão de reiniciar
6. `TelaContatos`: cadastro validado de até 5 contatos de confiança
7. `TelaHistorico`: lista de eventos (data, hora e tipo), totais e limpeza

O histórico fica em uma lista global em cada tela e é compartilhado entre as telas pelo TinyDB (Namespace `PAM`). Ele é apagado sempre que o app abre, então vale só para a sessão.
