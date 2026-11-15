# 💍 Casamento de Beatriz & João · Convite Oficial & Lista de Presentes

Site oficial e convite digital interativo de casamento de **Beatriz & João**, rumo ao grande dia em **13 de Novembro de 2027 às 15h30** no **Espaço Paradayse** (Nova Iguaçu - RJ).

---

## 🌐 Acesso Online

👉 **Site Oficial:** [https://matemag1co.github.io/casamento-bia-e-joao/](https://matemag1co.github.io/casamento-bia-e-joao/)

---

## ✨ Principais Funcionalidades

### 💌 1. Confirmação de Presença (RSVP Individual)
- **Convite Individual:** Sem campo de acompanhantes; cada confirmação é única e pessoal.
- **Formulário Dinâmico:** Nome completo, WhatsApp com máscara, confirmação de presença (*"Sim, confirmo!"* ou *"Infelizmente não"*) e recado carinhoso opcional.
- **Sincronização em Tempo Real (Supabase):** Salva instantaneamente na tabela `cofre_rsvp` e atualiza o contador de presenças em tempo real.
- **Confirmação no WhatsApp com Mensagem Programada:**
  - Botão interativo com escolha do destinatário: **Enviar para a Noiva (Beatriz)** ou **Enviar para o Noivo (João)**.
  - Abre diretamente a conversa com mensagem personalizada pré-preenchida para a data de **13/11/2027 às 15h30**.

### 📖 2. Manual do Convidado
- **Horário & Pontualidade:** 15h30 pontualmente (chegada recomendada entre 15h00 e 15h15).
- **Local & Recepção:** Espaço Paradayse (Estrada Mato Grosso, 80 - Campo Alegre, Nova Iguaçu - RJ).
- **Rotas GPS com 1 Toque:** Botões diretos para Google Maps e Waze.
- **Dress Code:** Passeio Completo / Esporte Fino Elegante.
- **Bênção dos Pais:** Marcela de Mello Rosa & Wilde dos Santos Rosa | Vanessa dos Santos Barbosa Souza & Alexandre Soares da Silva Souza.

### 🎁 3. Lista de Presentes & Pix Oficial C6 Bank
- **Pix Oficial em Destaque:**
  - QR Code do C6 Bank em alta resolução.
  - Chave Pix E-mail: `jmdias1317@icloud.com`.
  - Beneficiário: **João Miguel Dias (C6 Bank)**.
  - Botão de **Copiar Pix Copia e Cola** (código EMV completo).
  - Botão de **Copiar Chave E-mail**.
- **Presentes do Coração:** Sem links externos, focados na contribuição com amor via Pix.
- **Itens para o Novo Lar:** Cozinha, Eletrodomésticos, Sala, Quarto e Banheiro, com links diretos para Amazon e Mercado Livre.

### 🔒 4. Painel de Administração dos Noivos (Admin)
- Acesse pelo ícone 🔒 no topo da página.
- **Login seguro:** cada noivo entra com o próprio e-mail e senha (Supabase Auth). Cadastro público desativado.
- **Tudo sincronizado:** alterações feitas no painel ficam salvas no Supabase e aparecem em qualquer aparelho (PC e celular).
- **Gestão de Convidados:** busca, contagem de presenças, exclusão e exportação para CSV (Excel) e cópia para o WhatsApp. A lista de convidados só é visível para os noivos.
- **Gerenciador de Imagens:** edição da foto de capa, fotos da história do casal e fotos de cada presente, com envio de fotos direto do celular ou PC.
- **Configurações:** troca de senha, dados do Pix e telefones de WhatsApp dos noivos.

---

## 🚀 Publicação & GitHub Pages

- Repositório: `https://github.com/matemag1co/casamento-bia-e-joao.git`
- Branch: `main`
- Site no ar: [matemag1co.github.io/casamento-bia-e-joao](https://matemag1co.github.io/casamento-bia-e-joao/)
- Banco de dados: Supabase — script de configuração em `supabase-setup.sql` (pode ser executado mais de uma vez).
