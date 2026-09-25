# Preferências globais do usuário

## Superpowers e TDD

- Use a Superpowers em todas as sessões e chats do Codex, independentemente do projeto. Leia `using-superpowers/SKILL.md` e aplique as skills pertinentes à tarefa.
- Sempre que o usuário pedir para criar, implementar ou alterar código, leia e siga a skill `test-driven-development` da Superpowers antes de escrever a implementação.
- Siga RED → GREEN → REFACTOR: escreva um teste de comportamento, execute-o e confirme a falha esperada; implemente o mínimo para passar; execute os testes; refatore mantendo os testes passando. Para bugs, comece com um teste que reproduza o problema.
- Não substitua TDD por testes escritos depois da implementação. Informe os testes executados e seus resultados reais; se não puder executá-los, explique a limitação sem alegar sucesso.
- Use as skills do plugin Superpowers habilitado. Se não aparecerem no catálogo da sessão, localize e leia os arquivos instalados em `~/.codex/plugins/cache/*/superpowers/*/skills/`, escolhendo a versão ativa do plugin. Não dependa apenas da memória das instruções.
- Esta preferência persiste entre projetos e sessões, salvo orientação explícita posterior do usuário.

## Esclarecimento obrigatório de regras de negócio

- Use a skill `brainstorming` da Superpowers antes de criar funcionalidades ou alterar comportamentos. Consulte primeiro o contexto disponível (conversa, documentação, código e testes) para fazer perguntas informadas.
- Conduza ativamente o esclarecimento com o usuário, principalmente sobre regras de negócio. Faça uma pergunta objetiva por vez, preferindo alternativas com suas consequências quando isso facilitar a resposta. Continue perguntando enquanto houver lacunas ou contradições relevantes.
- Investigue, conforme a tarefa: objetivo e resultado esperado, atores e permissões, condições e validações, estados e transições, cálculos e limites, prazos, exceções, conflitos entre regras e critérios de aceitação. Use exemplos concretos e casos de borda para confirmar o significado das respostas.
- Não invente nem escolha silenciosamente regras de negócio. Se uma decisão de produto estiver indefinida, pergunte e aguarde a resposta antes de implementar a parte dependente dela; prossiga apenas com trabalho independente. Silêncio não é confirmação.
- Antes de implementar, apresente um resumo curto das regras entendidas e exemplos de aceitação para confirmação do usuário. Aproveite confirmações já dadas na conversa, sem exigir que sejam repetidas. Se surgir nova ambiguidade durante o trabalho, retome as perguntas.
- Converta as regras confirmadas e seus casos de borda em testes de comportamento, seguindo o TDD da Superpowers. Mantenha as decisões registradas no contexto ou na documentação pertinente do projeto.
- Evite perguntas repetidas ou sem impacto na solução; o objetivo é esclarecer o domínio continuamente. Decisões técnicas rotineiras podem ser resolvidas autonomamente quando não alterarem regras de negócio.

## Impeccable global

- A Impeccable está disponível globalmente em `~/.agents/skills/impeccable/SKILL.md`. Em todas as sessões e chats do Codex, use-a automaticamente sempre que a tarefa envolver criação, alteração, avaliação ou melhoria de interfaces, frontend, UX/UI ou design visual, sem exigir que o usuário a mencione novamente.
- Leia o `SKILL.md` instalado e as referências pertinentes antes do trabalho de interface. Siga seu carregamento de contexto por sessão no diretório do projeto e respeite o contexto de produto, a identidade visual existente e as preferências explícitas do usuário.
- Combine Impeccable para design e qualidade da interface com Superpowers para esclarecimento de regras de negócio, planejamento e TDD. As regras anteriores continuam valendo.
- Se a skill não aparecer no catálogo da sessão, leia diretamente o caminho global acima. A disponibilidade vale para qualquer projeto; aplique os fluxos de design quando forem pertinentes à tarefa, sem forçá-los em trabalhos exclusivamente de backend ou sem interface.

## Impeccable: perguntas, referências e paletas

- Ao iniciar uma nova direção visual, criar um site/interface ou propor mudanças de cores, conduza uma escolha visual com o usuário antes de implementar. Pergunte uma coisa por vez sobre preferências, público, sensação desejada, referências e restrições de marca; aproveite respostas já disponíveis e aprofunde as lacunas relevantes.
- Apresente pelo menos três referências de sites reais com direções cromáticas distintas e pertinentes ao projeto. Pesquise e abra os sites para verificar o visual atual, forneça links e explique o que cada referência ilustra. Não atribua cores ou características a um site sem verificá-las; se não houver acesso, declare a limitação e diferencie propostas próprias de referências verificadas.
- Ofereça pelo menos três paletas distintas, adequadas ao contexto, com amostras visuais comparáveis e códigos HEX. Identifique os papéis das cores (fundo, superfície, texto, principal e destaque), explique a sensação de cada opção e indique uma recomendação com justificativa. Diferencie paletas propostas de cores efetivamente extraídas das referências.
- Sempre que possível, mostre as paletas aplicadas ao mesmo pequeno exemplo de interface, como cabeçalho, botão e cartão, para facilitar a comparação. Verifique o contraste dos pares de texto/fundo e os estados de interação antes de aplicar; não afirme acessibilidade sem verificar.
- Pergunte qual direção/paleta o usuário prefere e aguarde sua escolha antes de implementar as decisões visuais dependentes. Permita combinar ou ajustar opções e retome as perguntas quando houver dúvidas. Uma escolha explícita já feita vale como confirmação; não repita a seleção em cada pequena alteração.
- Registre a direção aprovada na documentação visual pertinente do projeto. Em manutenção pontual que preserve a identidade aprovada, mantenha-a; se for necessário mudar a paleta ou a direção visual, reabra a escolha com referências e opções. Estas preferências orientam o uso da Impeccable mesmo após atualizações da skill.
