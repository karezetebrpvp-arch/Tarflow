[GUIA_INSTALACAO.md](https://github.com/user-attachments/files/27803936/GUIA_INSTALACAO.md)[Uploading# 🌊 TARFLOW — Versão 3.0

App pessoal que junta **gerenciamento financeiro** (gastos, metas, categorias, gráficos, Excel) com **gerenciamento de tarefas estilo Microsoft To Do** (listas, prioridades, lembretes, datas), além de **compartilhamento em casal/família** e **lembrete de fim de mês**.

---

## NOVIDADES DA VERSÃO 3.0

### 1. Novo nome: Tarflow 🌊
"Tar" de **tarefas** + "flow" de **fluxo financeiro**. Tudo o que você precisa para manter sua vida pessoal e financeira em ordem.

### 2. Aba de Tarefas (estilo Microsoft To Do)
- Crie múltiplas **listas de tarefas** (Trabalho, Casa, Compras, etc.).
- Cada tarefa tem **título, data de conclusão, lembrete (data/hora), prioridade** (alta/média/baixa) e **valor opcional**.
- Marque tarefas como **conta a pagar 💰** para que apareçam no lembrete de fim de mês.
- Visualização ordenada por prioridade, com indicadores de tarefas **atrasadas** e **para hoje**.
- Barra de progresso por lista mostrando % concluído.

### 3. Sistema de Compartilhamento 📤
Botão "Compartilhar" no cabeçalho com várias opções:
- **WhatsApp** (compartilhar com namorado(a), marido/esposa, família)
- **Telegram**
- **Email**
- **X / Twitter**
- **Facebook**
- **Copiar link**
- **Compartilhamento nativo** do sistema (Web Share API)

### 4. Modo Casal / Família 👨‍👩‍👧
- **Exportar dados**: gera um arquivo JSON com seus gastos, metas e tarefas.
- **Importar dados**: o parceiro carrega o arquivo dele e o app **mescla** (junta) os dados com os seus.
- Permite que casais ou famílias acompanhem juntos finanças e tarefas, mesmo sem servidor.

### 5. Lembrete de fim de mês ⏰
- Nos **últimos 5 dias do mês**, o app abre um modal mostrando:
  - 💰 **Contas a pagar pendentes** (tarefas marcadas como "É conta a pagar") com soma total.
  - 📝 **Tarefas pendentes** ainda não concluídas.
  - ⚠️ **Metas perto do limite** (acima de 80% do valor definido).
- Você pode dispensar ou clicar em "Lembrar mais tarde".
- Mostra no máximo **uma vez por dia**.

### 6. Notificações de lembretes de tarefas 🔔
- Se você definir um horário de lembrete em uma tarefa, o app dispara uma **notificação do navegador** no horário marcado.
- Também aparece como toast dentro do app.
- Verificação automática a cada 1 minuto enquanto o app está aberto.

### 7. Tudo do app de Finanças continua presente
20 categorias de gastos, metas mensais, gráfico de pizza, gráfico de barras mensal, exportação Excel (3 abas), modo escuro, login/cadastro, classificação social, perfil com insights e toast notifications.

---

## SOBRE A SINCRONIZAÇÃO ENTRE DISPOSITIVOS

Esta versão guarda os dados **no próprio aparelho** (localStorage do navegador). Para compartilhar com o parceiro:

1. **Modo casal via exportação JSON** (já funciona):
   - Você clica em "Exportar meus dados", recebe um arquivo .json.
   - Envia para o parceiro (WhatsApp, email, AirDrop, etc.).
   - Ele clica em "Importar dados" e os dados se mesclam com os dele.
   - Repita o processo quando quiser sincronizar.

2. **Sincronização automática em tempo real** (próxima evolução): requer backend (Firebase, Supabase). Me avise quando quiser fazer.

---

## COMO INSTALAR

### No celular (Android/iPhone)
1. Crie conta grátis no Netlify (netlify.com) ou Vercel.
2. Faça upload de `Tarflow.html` e `manifest.json`.
3. Abra o link no celular.
4. Android: Chrome > menu > "Instalar app".
5. iPhone: Safari > Compartilhar > "Adicionar à Tela de Início".

### No computador
1. Abra `Tarflow.html` no Chrome ou Edge.
2. Clique em "Instalar App" no topo (aparece quando hospedado em HTTPS).
3. Ou simplesmente abra o arquivo quando quiser usar.

---

## COMO USAR

### Cadastrar
1. Clique em "Entrar / Cadastrar" no topo.
2. Vá na aba "Cadastrar".
3. Preencha nome, email e senha (mínimo 4 caracteres).
4. Idade, salário e área são opcionais, mas dão acesso aos insights da aba Perfil.

### Adicionar gasto
1. Aba "Adicionar".
2. Escolha uma das 20 categorias.
3. Digite nome, valor e data.

### Criar lista e tarefas
1. Aba "✅ Tarefas".
2. Digite o nome da lista (ex: "Casa", "Trabalho") e clique em ➕ Criar.
3. Selecione a lista no dropdown.
4. Adicione tarefas com título, data de conclusão, lembrete, prioridade.
5. Se for conta a pagar, marque a caixinha "💰 É uma conta a pagar".

### Compartilhar com o parceiro
1. Clique em "📤 Compartilhar" no cabeçalho.
2. Para **convidar** alguém: clique em WhatsApp, Telegram, Email, etc.
3. Para **juntar dados** com o parceiro: clique em "Exportar meus dados" e envie o arquivo. Ele clica em "Importar dados" e seleciona o arquivo.

### Receber lembretes
1. Permita notificações quando o navegador perguntar.
2. Defina um horário de lembrete na tarefa.
3. Quando chegar o horário, o app mostra a notificação.
4. Nos últimos 5 dias do mês, o modal de fim de mês aparece automaticamente.

### Definir meta de gastos
1. Aba "Metas".
2. Escolha "Meta Geral" ou uma categoria específica.
3. Digite o valor limite mensal.

### Exportar Excel
1. Aba "Visualizar".
2. Clique em "Exportar para Excel".

### Modo escuro
1. Clique em "🌙 Modo Escuro" no cabeçalho.

---

## ARQUIVOS

- `Tarflow.html` — o app completo (HTML, CSS, JS em um único arquivo).
- `manifest.json` — configuração do PWA para instalação.
- `GUIA_INSTALACAO.md` — este guia.

---

## TESTE / REVISÃO

Funcionalidades testadas:
- Renomeação completa do app para Tarflow.
- Aba "Tarefas" com criação de listas, adição, conclusão, exclusão e ordenação por prioridade.
- Lembretes de tarefas (toast + Notification API) verificados a cada minuto.
- Modal de compartilhamento com WhatsApp, Telegram, Email, X, Facebook, Copiar link e compartilhamento nativo.
- Export/Import de JSON para modo casal (mescla gastos, metas e listas de tarefas sem duplicar IDs).
- Modal de fim de mês ativa quando faltam ≤ 5 dias e há pendências.
- Dados isolados por usuário (chave do localStorage inclui o email).

Sugestões para próximas versões:
- Sincronização real via Firebase ou Supabase.
- Recorrência (tarefa que se repete todo mês).
- Categorias customizáveis pelo usuário.
- Backup automático em nuvem.
- Modo família com convite por código.

Bom uso! 🌊
 GUIA_INSTALACAO.md…]()


[manifest.json](https://github.com/user-attachments/files/27803942/manifest.json){
  "name": "Tarflow — Finanças & Tarefas",
  "short_name": "Tarflow",
  "description": "Tarflow: gerenciamento de finanças e tarefas pessoais, com compartilhamento em casal, lembretes e metas mensais",
  "start_url": "/Tarflow.html",
  "display": "standalone",
  "background_color": "#1a1a2e",
  "theme_color": "#2C5F7C",
  "orientation": "portrait-primary",
  "icons": [
    {
      "src": "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200'%3E%3Crect fill='%232C5F7C' width='200' height='200' rx='40'/%3E%3Ctext x='100' y='135' font-size='110' text-anchor='middle' fill='white'%3E🌊%3C/text%3E%3C/svg%3E",
      "sizes": "192x192",
      "type": "image/svg+xml"
    },
    {
      "src": "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Crect fill='%232C5F7C' width='512' height='512' rx='100'/%3E%3Ctext x='256' y='360' font-size='300' text-anchor='middle' fill='white'%3E🌊%3C/text%3E%3C/svg%3E",
      "sizes": "512x512",
      "type": "image/svg+xml",
      "purpose": "any maskable"
    }
  ],
  "categories": ["finance", "productivity", "utilities", "lifestyle"],
  "screenshots": [
    {
      "src": "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 540 720'%3E%3Crect fill='%23667eea' width='540' height='720'/%3E%3Ctext x='270' y='360' font-size='48' text-anchor='middle' fill='white'%3ETarflow%3C/text%3E%3C/svg%3E",
      "sizes": "540x720",
      "type": "image/svg+xml",
      "form_factor": "narrow"
    }
  ]
}



[Tarflow_Estrutura_Site.docx](https://github.com/user-attachments/files/27803949/Tarflow_Estrutura_Site.docx)




<img width="1254" height="1254" alt="tarflow_logo" src="https://github.com/user-attachments/assets/7ac84a8b-fdce-41d3-967c-10b3586203f8" />
<img width="1254" height="1254" alt="tarflow_icon" src="https://github.com/user-attachments/assets/51a7fe39-4f73-43aa-b0a2-a778bf1c2167" />
