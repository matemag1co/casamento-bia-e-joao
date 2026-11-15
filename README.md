# 💍 Casamento de João Miguel & Anna Beatriz · Convite Oficial & Lista de Presentes

Site oficial e convite digital interativo de casamento de **João Miguel & Anna Beatriz**, rumo a **Novembro de 2027**.

O projeto conta com confirmação de presença (RSVP) em tempo real, integração direta com WhatsApp dos noivos, lista completa de presentes para montagem do novo lar (com contribuição via Pix e links para Amazon e Mercado Livre), galeria com fotos reais do casal e painel administrativo para gestão dos noivos.

---

## ✨ Principais Funcionalidades

### 💌 1. Confirmação de Presença (RSVP)
- **Formulário Completo e Inteligente:**
  - Nome completo e WhatsApp com formatação e máscara.
  - Seletor de presença (*"Sim, com certeza!"* ou *"Infelizmente não"*).
  - Quantidade de pessoas e nomes dos acompanhantes.
  - Mensagem carinhosa de bênção/felicitações.
- **Sincronização em Tempo Real (Supabase):**
  - Salva instantaneamente na tabela `cofre_rsvp`.
  - Contador dinâmico em tempo real exibindo quantas pessoas já confirmaram presença.
- **Confirmação Direta no WhatsApp com Mensagem Programada:**
  - Fluxo: `Nome > Telefone > Acompanhantes > Escolha do Destinatário`.
  - Botão interativo para escolher enviar para o **Noivo (João)** ou para a **Noiva (Bia)**.
  - Gera a mensagem perfeitamente formatada com nome, acompanhantes e recado.

### 🎁 2. Lista de Presentes para o Novo Lar
- **Categorias Organizadas:**
  - 🍳 **Cozinha:** Panelas de cerâmica, aparelho de jantar, faqueiro, taças, potes herméticos, facas chef.
  - ⚡ **Eletrodomésticos:** Air Fryer, cafeteira, liquidificador potente, sanduicheira grill, aspirador vertical, micro-ondas espelhado.
  - 🛋️ **Sala & Casa:** Cota para Smart TV, caixa de som Bluetooth, tapete geométrico, mantas e almofadas.
  - 🛏️ **Quarto:** Jogo de cama 400 fios, edredom dupla face toque de pluma, travesseiros NASA.
  - 🛁 **Banheiro:** Jogo de toalhas banhão 5 peças, kit cerâmica & bambu, roupões de casal.
  - ❤️ **Presentes do Coração & Experiências:** Jantar romântico na lua de mel, passeio de barco na Urca, brinde de champanhe, cota para reforma do ninho de amor e **Presente com Valor Livre** (onde o convidado escolhe qualquer valor).
- **Modelo Duplo de Presente:**
  1. **Presentear via Pix:** Abre modal com valor sugerido, QR Code Pix gerado na hora, Chave Pix com cópia em 1 toque (`jmsantos108@gmail.com`), campo para deixar recado e botão de avisar no WhatsApp.
  2. **Comprar na Loja:** Botões diretos para buscar e comprar o produto exato na **Amazon** ou **Mercado Livre**.

### 📷 3. Nossa História & Galeria de Fotos
- Galeria com fotos reais do casal:
  - O pedido de noivado inesquecível no Pão de Açúcar com o anel de noivado.
  - Passeio de barco na Urca com o Pão de Açúcar ao fundo.
  - Sob a luz das estrelas e iluminação suspensa.
  - Momentos no Maracanã torcendo pelo Mengão.
  - Píer e caminhadas na praia.
  - A caminhada de fé na Igreja Batista Reviver em Cristo.
- **Lightbox Interativo:** Toque em qualquer foto para visualizá-la em tela cheia com legenda.

### 💬 4. Mural de Recados & Felicitações
- Conectado em tempo real ao Supabase (`cofre_guest_messages`).
- Os convidados podem deixar homenagens que aparecem na hora no mural.

### 🔒 5. Painel de Gestão dos Noivos (Admin)
- Acesso com senha (`casamento2027`) ou no topo pelo ícone 🔒.
- Contagem total de pessoas confirmadas e famílias cadastradas.
- Tabela com lista completa de convidados, telefones, acompanhantes e mensagens.
- **Exportar para CSV (Excel)** com 1 clique para a cerimonialista.
- **Copiar Resumo para WhatsApp** com a lista formatada.
- Configuração e edição dos números de WhatsApp de João e Bia.

---

## 🗄️ Configuração do Banco de Dados (Supabase)

1. Acesse o seu projeto no [Supabase](https://supabase.com).
2. Abra a aba **SQL Editor**.
3. Execute o script contido em [`supabase-setup.sql`](./supabase-setup.sql).
4. O script cria automaticamente a tabela `cofre_rsvp` e configura as políticas de RLS e o Realtime!

---

## 🚀 Publicação & GitHub Pages

O site é 100% estático (Single Page Application com HTML5, CSS3 e JS moderno), podendo ser hospedado diretamente no **GitHub Pages**:
- Repositório: `https://github.com/matemag1co/cofre-dos-noivos.git`
- Branch: `main`
- Raiz: `/` (root)
