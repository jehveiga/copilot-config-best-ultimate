# Instruções do Copilot

- Todos os agentes de comportamento em `.github/agents/`
- Todos os arquivos de regras e instruções em `.github/instructions/`
- Todos os arquivos de prompt em `.github/skills/`
- Toda a documentação e comentários de código destinados aos contribuidores

## Documentação Viva do Projeto: CLAUDE.md

### O que é o CLAUDE.md

O `CLAUDE.md` é o **documento de onboarding técnico do projeto** — um arquivo vivo, escrito e mantido pelo Copilot, que concentra todo o conhecimento necessário para que qualquer sessão futura retome o contexto exatamente de onde parou. É o equivalente do _onboarding doc_ de uma equipe de engenharia.

> **Por que isso importa:** Documentação é investimento com retorno imediato. Cada hora documentando no `CLAUDE.md` economiza horas de contexto perdido em sessões futuras.

### Quando Criar e Atualizar

- **Criar** o `CLAUDE.md` na raiz do projeto ao iniciar qualquer novo projeto ou ao implementar a primeira funcionalidade relevante.
- **Atualizar** ao término de cada sessão que introduza mudanças significativas: novas features, refatorações, mudanças de arquitetura, novos serviços, variáveis de ambiente, etc.
- **Consultar** no início de cada sessão, antes de propor qualquer implementação, para garantir consistência com o que já foi decidido e construído.

### Estrutura Obrigatória do CLAUDE.md

O arquivo deve conter, no mínimo, as seguintes seções:

```markdown
# CLAUDE.md — Documento de Contexto do Projeto

## 1. Visão Geral da Arquitetura

Descrever o estilo arquitetural (DDD, Clean Architecture, CQRS, etc.), os principais limites de contexto e como os componentes se relacionam.

## 2. Stack Tecnológico Completo

Listar todas as tecnologias, frameworks, bibliotecas e versões relevantes utilizadas no projeto.

## 3. Variáveis de Ambiente

Documentar todas as variáveis de ambiente necessárias, com descrição e exemplo de valor (nunca valores reais de produção).

## 4. Estrutura de Diretórios

Mapa comentado da estrutura de pastas do projeto, explicando a responsabilidade de cada diretório principal.

## 5. Serviços, Jobs e Models

Catálogo dos principais serviços de domínio, jobs agendados e entidades/models, com uma linha descrevendo a responsabilidade de cada um.

## 6. Common Hurdles — Problemas Conhecidos e Soluções

Registro de obstáculos recorrentes já enfrentados no projeto e como foram resolvidos. Formato: problema → causa raiz → solução aplicada.

## 7. Design Patterns Adotados

Listar os padrões de projeto utilizados no codebase com uma breve justificativa de cada escolha.

## 8. Checklist Pós-Implementação

Lista de verificação a ser executada após cada entrega de funcionalidade, cobrindo testes, documentação, migrations, configurações e revisão de segurança.
```

### Regras de Manutenção

- O `CLAUDE.md` **nunca deve ficar desatualizado** em relação ao estado real do projeto.
- Decisões arquiteturais e técnicas relevantes **devem ser registradas imediatamente** após serem tomadas.
- A seção _Common Hurdles_ deve crescer organicamente: sempre que um problema for resolvido, adicionar o relato.
- O arquivo deve ser **legível por humanos e por agentes de IA** — escrever de forma clara, objetiva e sem ambiguidades.
- **Não remover** seções anteriores sem motivo explícito; prefira marcar itens como obsoletos com nota de contexto.
