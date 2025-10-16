# Instruções para Importação no GitBook

Este documento fornece orientações para importar a documentação do curso para o GitBook.

## 📁 Estrutura de Arquivos

A documentação está organizada no diretório `gitbook/` com a seguinte estrutura:

```
gitbook/
├── README.md              # Página inicial
├── SUMMARY.md             # Índice de navegação
├── ementa.md              # Ementa completa do curso
├── professor.md           # Informações sobre o professor
├── modulo1/               # Conteúdo do Módulo 1
├── modulo2/               # Conteúdo do Módulo 2
├── modulo3/               # Conteúdo do Módulo 3
├── modulo4/               # Conteúdo do Módulo 4
├── materiais/             # Materiais de apoio
└── referencias/           # Referências e glossário
```

## 🔄 Métodos de Importação

### Método 1: Integração com GitHub (Recomendado)

O GitBook pode ser integrado diretamente ao repositório GitHub para sincronização automática.

**Passos:**

1. Acesse o GitBook: https://app.gitbook.com/
2. Faça login na sua conta
3. Crie um novo espaço ou selecione o espaço existente
4. Vá em **Settings** > **Integrations**
5. Selecione **GitHub**
6. Autorize a conexão com o GitHub
7. Selecione o repositório: `ErisonBarros/Fiscaliza-o-de-Obras-com-Drones`
8. Configure o branch: `erison.barros`
9. Defina o diretório raiz: `gitbook/`
10. Ative a sincronização bidirecional (opcional)

**Vantagens:**
- Sincronização automática entre GitHub e GitBook
- Controle de versão integrado
- Colaboração facilitada

### Método 2: Importação Manual

Se preferir importar manualmente os arquivos:

**Passos:**

1. Acesse o GitBook: https://app.gitbook.com/
2. Crie um novo espaço ou selecione o espaço existente
3. Clique em **Import** no menu
4. Selecione **Markdown files**
5. Faça upload do arquivo `SUMMARY.md` primeiro
6. Faça upload dos demais arquivos `.md` respeitando a estrutura

**Nota:** A importação manual requer que você mantenha a estrutura de diretórios conforme definida no `SUMMARY.md`.

### Método 3: Git Sync

Para sincronização via Git:

**Passos:**

1. No GitBook, vá em **Settings** > **Git Sync**
2. Configure a URL do repositório
3. Defina as credenciais de acesso
4. Configure o branch e o diretório
5. Ative a sincronização

## 📝 Arquivo SUMMARY.md

O arquivo `SUMMARY.md` define a estrutura de navegação do GitBook. Ele já está configurado com todos os capítulos e seções do curso.

**Estrutura atual:**

- Introdução
  - Apresentação do Curso
  - Ementa Completa
  - Sobre o Professor
- Módulos do Curso (1 a 4)
- Materiais de Apoio
- Referências

## ✅ Checklist de Importação

Antes de importar, verifique:

- [ ] Todos os arquivos `.md` estão no formato correto
- [ ] O arquivo `SUMMARY.md` está completo
- [ ] As imagens (se houver) estão no diretório correto
- [ ] Os links internos estão funcionando
- [ ] A estrutura de diretórios está correta

## 🔧 Configurações Recomendadas

Após a importação, configure:

### Aparência
- **Tema:** Claro ou Escuro (conforme preferência)
- **Logo:** Adicione o logo da UFPE ou do curso
- **Cores:** Personalize conforme identidade visual

### Navegação
- Ative o **índice lateral** para facilitar navegação
- Configure **breadcrumbs** para mostrar caminho
- Ative a **busca** para localização rápida de conteúdo

### Acesso
- **Público:** Se o curso for aberto
- **Privado:** Se restrito aos participantes
- **Com senha:** Para controle de acesso

### Domínio Personalizado (Opcional)
- Configure um domínio personalizado se disponível
- Exemplo: `curso-drones.ufpe.br`

## 🔗 Links Importantes

- **GitBook Docs:** https://docs.gitbook.com/
- **GitHub Integration:** https://docs.gitbook.com/integrations/git-sync
- **Markdown Guide:** https://docs.gitbook.com/content-editor/markdown

## 📧 Suporte

Para dúvidas sobre a importação:

- **Professor:** erison.barros@ufpe.br
- **Departamento:** decart.ctg@ufpe.br
- **Suporte GitBook:** support@gitbook.com

---

## 🎨 Personalização Adicional

Após a importação, você pode:

1. **Adicionar imagens e diagramas** aos módulos
2. **Inserir vídeos** de demonstração
3. **Criar páginas interativas** com quizzes
4. **Adicionar arquivos para download** (PDFs, checklists)
5. **Configurar comentários** para interação dos alunos

## 📊 Monitoramento

O GitBook oferece analytics para acompanhar:

- Número de visualizações
- Páginas mais acessadas
- Tempo de leitura
- Origem dos acessos

Use essas métricas para melhorar continuamente o conteúdo do curso.

---

**Última atualização:** Outubro de 2025  
**Versão da documentação:** 1.0

