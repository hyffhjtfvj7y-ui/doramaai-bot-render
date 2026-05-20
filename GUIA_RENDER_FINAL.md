# 🚀 Guia de Implantação DoramaAI no Render

Seu bot foi otimizado para vozes sensuais realistas, carregamento rápido e botões 100% funcionais. Siga os passos abaixo para rodar 24/7 no Render.

## 🛠️ O que foi melhorado:
1.  **Vozes Realistas:** Configurado o estilo `Sensual` da Microsoft Neural no D-ID, com tom mais grave e cadência sedutora.
2.  **Carregamento Rápido:** Otimizado o intervalo de polling do D-ID e reduzido o tempo de processamento de áudio para entrega imediata.
3.  **Botões Corrigidos:** Toda a lógica de navegação do catálogo, favoritos e episódios foi revisada.
4.  **Persistência de Dados:** Configurado o `render.yaml` para usar um Disco Persistente, garantindo que seus usuários VIP e favoritos não sumam ao reiniciar.

## 📦 Como Implantar no Render:
1.  Crie uma conta em [render.com](https://render.com).
2.  Crie um novo **Blueprint** (ou conecte seu repositório GitHub com estes arquivos).
3.  O Render lerá o arquivo `render.yaml` automaticamente.
4.  **Configure as Variáveis de Ambiente no Painel do Render:**
    *   `TELEGRAM_BOT_TOKEN`: Seu token do @BotFather.
    *   `TELEGRAM_ADMIN_ID`: Seu ID do Telegram para comandos de admin.
    *   `DID_API_KEY`: Sua chave de API do D-ID.
    *   `PIX_KEY`: Sua chave PIX para pagamentos VIP.
    *   `TONCOIN_ADDRESS`: Seu endereço Toncoin (opcional).

## 💾 Persistência:
O bot salvará os dados na pasta `/data`. No Render, configuramos um volume de 1GB para que esses dados sejam permanentes.

---
**Dica:** Para rodar 24/7 de forma estável, o plano "Worker" do Render é o ideal, pois não entra em suspensão.
