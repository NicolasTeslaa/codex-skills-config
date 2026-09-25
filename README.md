# Codex skills & configurações

Snapshot público da configuração pessoal do Codex, exportado em 24/09/2026.

## Conteúdo

- `config/AGENTS.md`: preferências globais completas — Superpowers, TDD, esclarecimento de regras de negócio e Impeccable com referências de sites e escolha de paletas.
- `config/config.example.toml`: modelo, esforço, nível de serviço, recursos, preferências do app e estados de plugins, exportados por lista explícita de campos permitidos.
- `skills/superpowers/`: 14 skills da instalação local Superpowers 6.3.0, cache `1dc19589`.
- `skills/impeccable/`: skill Impeccable 4.3.1, referências e scripts auxiliares instalados.
- `inventory/SKILLS.md` e `inventory/skills.json`: inventário completo dos SKILL.md encontrados nos diretórios globais e no cache, incluindo hashes para conferência.
- `inventory/mcp-servers.json`: nomes, ativação e campos de configuração dos servidores MCP, sem valores privados.

A presença no cache não garante que uma skill ou plugin esteja ativo. As skills internas do app podem exigir runtimes e ferramentas próprios e não são instalações independentes.

## Restaurar em outra máquina

1. Instale o Codex e autentique-se normalmente.
2. Faça backup das configurações existentes. Mescle `config/AGENTS.md` em `~/.codex/AGENTS.md` e os campos desejados de `config/config.example.toml` em `~/.codex/config.toml`.
3. Para Superpowers, prefira instalar o plugin original no Codex. Como alternativa, copie os diretórios individuais de `skills/superpowers/` para `~/.agents/skills/`. Use apenas uma dessas instalações para evitar skills duplicadas. Na alternativa por cópia, ajuste no AGENTS.md o caminho de fallback da Superpowers para `~/.agents/skills/`.
4. Copie `skills/impeccable/` para `~/.agents/skills/impeccable/`. O launcher pode baixar seu motor oficial no primeiro uso; hooks não foram instalados ou exportados aqui.
5. Reinstale os plugins oficiais necessários no Codex e configure seus MCPs localmente. Os estados em config.example.toml não instalam plugins nem restauram autenticações.
6. Inicie uma nova sessão e confirme que as skills e as instruções globais estão disponíveis.

## Limites deste backup público

Não é uma cópia integral de `~/.codex`. Foram excluídos credenciais, tokens, variáveis de ambiente, URLs privadas de MCP, histórico de conversas, memórias, bancos de dados, anexos, áudios, logs, caminhos de projetos e permissões locais de execução. Regras de aprovação acumuladas em `rules/default.rules`, registros de confiança, notificações com executáveis locais e caminhos de runtimes não são portáveis e não foram publicados.

As skills internas da OpenAI e templates aparecem no inventário, sem seus arquivos. A licença local de documentos proíbe redistribuição; para os demais componentes internos, não foi estabelecida permissão de redistribuição. Reinstale-os pelo produto ou marketplace correspondente. O inventário preserva a lista sem publicar conteúdo restrito.

Este backup inclui configurações acessíveis do usuário; não inclui instruções internas do serviço ou estado de sessões.

## Origens e licenças

- [Superpowers](https://github.com/obra/superpowers): MIT, licença preservada em `licenses/SUPERPOWERS-LICENSE`.
- [Impeccable](https://github.com/pbakaus/impeccable): Apache-2.0, licença preservada em `licenses/IMPECCABLE-LICENSE`. Os arquivos da skill foram copiados sem alterações.

Os componentes de terceiros mantêm suas licenças e avisos próprios. As configurações pessoais refletem preferências deste usuário e devem ser revisadas antes de uso em outro ambiente.
