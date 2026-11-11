# 💍 Cofre dos Noivos — João & Anna Beatriz

Aplicativo web progressivo (PWA) e cofre de casamento inteligente, com mapa de envelopes, cotas de presente para padrinhos, sincronização em tempo real via Supabase e suporte offline.

---

## ✨ Principais Funcionalidades

### 💑 Modo Casal (Gestão dos Noivos)
- **Mapa dos Sonhos (283 Envelopes):** Toque nos envelopes para marcar valores já guardados (R$ 5 a R$ 1.000). Totaliza a meta de R$ 25.000.
- **Valores Livres:** Deposite valores fora do mapa com notas/observações.
- **Contagem Regressiva:** Contador automático de dias restantes rumo a novembro de 2027.
- **Gráfico de Evolução:** Curva diária de crescimento do fundo em relação à meta.
- **Celebração com Confetes:** Animação festiva ao preencher envelopes e atingir marcos.
- **Controle de Acesso Seguro:** Modo leitura público e modo edição protegido por código OTP por e-mail no Supabase (restrito ao João e Anna).
- **Backup & Ajustes:** Exportação/importação em JSON e configuração de nomes e meta.

### 🎁 Modo Padrinhos & Convidados (Presentes em Cotas)
- **Acesso direto via link:** Acesse adicionando `?modo=convidados` ou `?padrinhos` na URL.
- **Catálogo de Cotas de Presente:**
  - 🥂 Brinde dos Noivos — R$ 50
  - 🍰 Mesa de Doces & Bem-Casados — R$ 80
  - 📸 Álbum de Fotos do Grande Dia — R$ 120
  - 🍽️ Jantar Romântico na Lua de Mel — R$ 180
  - 🏖️ Passeio Inesquecível a Dois — R$ 250
  - 🛏️ Primeira Noite dos Recém-Casados — R$ 350
  - ✈️ Passagens da Lua de Mel — R$ 500
  - 💎 Presente do Coração (Valor Livre)
- **Pix com 1 Toque:** Chave Pix e QR Code para transferência bancária.
- **Mural de Recados & Felicitações:** O convidado envia o nome e uma mensagem de carinho aos noivos, que fica eternizada no mural do casal.

### 📲 Experiência Mobile & PWA
- **Instalável como App:** No Android e Chrome através do botão "Instalar", e no iPhone/Safari através de "Compartilhar > Adicionar à Tela de Início".
- **Compartilhamento Fácil no WhatsApp:** Botão para gerar um card de texto comemorativo e enviar direto no WhatsApp do casal ou dos amigos.
- **Cache Offline:** Funciona mesmo sem conexão com a internet graças ao Service Worker e LocalStorage.

---

## 🗄️ Configuração do Banco de Dados (Supabase)

Para garantir que o mural de recados dos convidados e a sincronização em tempo real funcionem perfeitamente:

1. Acesse o painel do seu projeto no [Supabase](https://supabase.com).
2. Abra a aba **SQL Editor**.
3. Copie e cole todo o conteúdo do arquivo [`supabase-setup.sql`](./supabase-setup.sql).
4. Clique em **Run** (Executar).

Pronto! Todas as tabelas, políticas de segurança e canais de Realtime estarão ativos.

---

## 🚀 Como Publicar Grátis na Web

Para que você e a Anna (e os convidados) possam acessar de qualquer lugar pelo celular com um link bonito:

1. **Vercel / Netlify / GitHub Pages:**
   - Basta subir esta pasta (`cofre-dos-noivos`) em um repositório no GitHub ou arrastar para o [Netlify Drop](https://app.netlify.com/drop).
2. O site terá HTTPS automático, o que ativa o PWA completo para instalação no celular!
