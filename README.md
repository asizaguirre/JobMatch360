# JobMatch360

## Descrição
Sistema que busca vagas compatíveis com currículo enviado, calcula porcentagem de compatibilidade e permite candidatura automática ou exclusão da vaga.

## Tecnologias
- Node.js + Express
- Next.js (frontend)
- Prisma ORM
- Banco de dados (SQLite ou PostgreSQL)

## Funcionalidades
- Upload de currículo (PDF/Texto)
- Busca de vagas
- Compatibilidade calculada (%)
- Botão de candidatura
- Botão de exclusão
- Relatório de candidaturas

## Segurança
- Helmet para proteção de headers
- Rate limiting contra abuso
- Sanitização de inputs
- Criptografia de dados sensíveis
- Uso de HTTPS

## Deploy
- Compatível com Vercel
- Configuração via `vercel.json`

## Instalação

### Configuração Inicial
```bash
# Instalar dependências do projeto (raiz ou pastas separadas conforme setup)
npm install

# O arquivo .env foi criado automaticamente com DATABASE_URL e OPTIMIZE_API_KEY.
# Certifique-se de que ele não seja commitado (já está no .gitignore).

# Configurar Banco de Dados (SQLite por padrão)
npx prisma migrate dev --name init

# Gerar Cliente Prisma (necessário após atualizações)
npm run db:generate
