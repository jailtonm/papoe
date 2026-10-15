# PAPOE — projeto inicial

Protótipo web em Next.js com identidade visual verde e amarela.

## Antes de começar

Instale:
1. Node.js (versão LTS) em https://nodejs.org/
2. Visual Studio Code em https://code.visualstudio.com/

## Como abrir no Windows

1. Extraia o arquivo ZIP para uma pasta fácil de encontrar, por exemplo `C:\PAPOE`.
2. Abra essa pasta no Visual Studio Code.
3. No menu do VS Code, selecione **Terminal > Novo Terminal**.
4. Digite:

```powershell
npm install
```

5. Depois que terminar, digite:

```powershell
npm run dev
```

6. Abra o navegador e visite:

http://localhost:3000

Para parar o servidor, volte ao terminal e pressione `Ctrl + C`.

## O que funciona nesta primeira versão

- Navegação entre Feed, Amigos, Mensagens, Vídeos, Comunidades e Perfil.
- Criar publicações de texto e curtir posts.
- Enviar mensagens locais de demonstração.
- Criar grupos de demonstração.
- Editar o nome do perfil na sessão atual.
- Layout adaptável a telas menores.

## Limitações importantes

Este é o primeiro esqueleto do projeto, não uma rede social pública pronta:
- Ainda não há cadastro/login real.
- Publicações e mensagens não são persistidas num banco de dados.
- Mensagens não chegam a outros usuários ou dispositivos.
- Upload e armazenamento de fotos/vídeos ainda não estão conectados.
- Não publique informações pessoais reais nesta versão.

## Arquitetura sugerida para a próxima etapa

- **Interface:** Next.js + React + TypeScript.
- **Banco, autenticação, armazenamento e tempo real:** Supabase.
- **Hospedagem futura:** Vercel para o site e Supabase para dados/arquivos.

Antes de abrir para o público, implementar políticas de segurança (RLS), validação de uploads, moderação, recuperação de conta, privacidade e testes.

## Estrutura

```text
papoe-inicial/
├── app/
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── package.json
├── tsconfig.json
├── next.config.ts
├── eslint.config.mjs
└── README.md
```
