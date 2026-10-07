# RULES.md

**Autor:** Ricardo Ceneviva  
**Versão:** 2026-04-10  
**Escopo do projeto:** execução técnico-operacional, analítica e documental do projeto Data Science

## Finalidade

Este repositório apoia a execução técnica de projetos de Data Science, econometria, avaliação de políticas públicas e estatística aplicada.

O agente deve reconhecer o tipo de tarefa antes de agir.

Este repositório pode apoiar, entre outras frentes:

1. especificação funcional;
2. modelagem de dados;
3. ingestão e curadoria de fontes;
4. marts analíticos e indicadores;
5. outputs prontos para dashboard e relatórios;
6. auditorias de qualidade de dados, lógica e consistência;
7. documentação técnica e handoff;
8. integração e reconciliação de materiais validados;
9. revisão metodológica, factual, editorial e de governança.

Não trate o projeto como simples repositório pedagógico.  
Não trate governança de dados como se fosse apenas tarefa de código.  
Não trate modelagem estatística como se fosse apenas automação operacional.  
Não tome decisões substantivas no lugar do Professor.

---

## Princípios centrais

1. Reprodutibilidade é mandatória.
2. Correção factual é mandatória.
3. Aderência à documentação canônica do projeto ou subprojeto é mandatória.
4. Confie no que foi validado. Seja cético com o que não foi validado.
5. Prefira fluxos simples, auditáveis e transparentes a soluções engenhosas, porém opacas.
6. Prefira ferramentas, pacotes e bibliotecas estáveis, comuns e bem documentados.
7. Toda entrega substantiva deve deixar rastro verificável por outro revisor.
8. Distinga claramente:
   - monitoramento operacional;
   - descrição;
   - associação;
   - previsão;
   - interpretação causal.
9. Nunca apresente uma alegação causal sem desenho compatível.
10. Preserve a lógica real do sistema, do processo analítico ou da regra de negócio sob análise.
11. Preserve privacidade por desenho, controle de acesso por perfil e rastreabilidade de uso.
12. Faça apenas o número mínimo de perguntas necessário para reduzir incerteza material.
13. **Programação Letrada é obrigatória.**
14. Código sem explicação humana suficiente não é entrega completa, salvo autorização explícita do Professor.
15. Arquiteturas multiagente são permitidas, mas não obrigatórias por padrão.
16. Prefira sempre a menor arquitetura capaz de cumprir a tarefa com segurança, rigor metodológico e auditabilidade.
17. Em tarefas complexas, a execução pode ser distribuída entre agentes especializados, desde que o plano explicite papéis, ferramentas, memórias, guardrails, critérios de validação e pontos de aprovação.
18. Memória persistente só pode incorporar conteúdo validado, aprovado ou explicitamente definido como canônico.
19. Histórico de sessão, logs, rascunhos e correções locais não equivalem a memória normativa do projeto.
20. Rastreamento de execução, observabilidade e documentação de decisões críticas são obrigatórios em fluxos agênticos complexos.

---

## Hierarquia de fontes e regras de evidência

Quando houver múltiplos arquivos, notas ou versões, use a seguinte ordem de prioridade:

1. instruções explícitas do Professor;
2. documentação canônica do projeto ou subprojeto;
3. planos, codebooks, decisões e materiais já validados;
4. fontes primárias de dados, exports, schemas, logs e código;
5. rascunhos internos e notas auxiliares;
6. documentação externa oficial e literatura técnica ou científica.

Regras adicionais:

1. Um resumo derivado nunca substitui uma fonte canônica.
2. Se uma nota interna conflitar com uma fonte canônica, prevalece a fonte canônica.
3. Se duas fontes validadas conflitam, interrompa a execução e reporte o conflito antes de continuar.
4. Regras de negócio, thresholds, datas, identificadores, parâmetros, métricas ou alegações empíricas devem ser conferidos na fonte primária ou canônica relevante antes de serem reutilizados.
5. Se faltar uma fonte obrigatória, interrompa e informe explicitamente o que está faltando.

---

## Classificação da tarefa

Antes de qualquer trabalho substantivo, classifique a tarefa em um modo principal:

1. **Especificação funcional**
   - requisitos;
   - regras de negócio;
   - definição de entidades;
   - regras de acesso;
   - definição de outputs.

2. **Modelagem de dados**
   - esquema relacional;
   - modelagem dimensional;
   - desenho de metadados;
   - estratégia de chaves;
   - regras de versionamento.

3. **Ingestão e curadoria**
   - intake de arquivos brutos;
   - validação de tipos;
   - deduplicação;
   - reconciliação de identificadores;
   - padronização.

4. **Marts analíticos e indicadores**
   - marts;
   - KPIs;
   - funnels;
   - timelines;
   - agregados de monitoramento.

5. **Análise estatística e econométrica**
   - descrição analítica;
   - modelagem inferencial;
   - previsão;
   - avaliação causal;
   - heterogeneidade e sensibilidade.

6. **Dashboard e camada de reporting**
   - estruturas prontas para visualização;
   - filtros;
   - visões individuais e agregadas;
   - tabelas exportáveis;
   - outputs por perfil de uso.

7. **Auditoria e reconciliação**
   - conflitos de fonte;
   - reconciliação entre arquivos;
   - revisão de qualidade de dados;
   - validação de regras;
   - auditoria de outputs.

8. **Documentação técnica e handoff**
   - planos;
   - codebooks;
   - logs de decisão;
   - memorandos de validação;
   - notas de execução;
   - handoff.

Escolha um modo principal.  
Se a tarefa abranger vários modos, explicite a sequência antes da implementação.

---

## Regras metodológicas

1. Não confunda observação com explicação causal.
2. Não confunda monitoramento operacional com inferência estatística.
3. Não confunda associação com previsão.
4. Não confunda significância estatística com relevância substantiva.
5. Explicite suposições, limitações, riscos de viés e grau de incerteza.
6. Quando um indicador depender de regra de negócio, torne essa regra explícita e versionada.
7. Quando um resultado depender de filtro, recodificação, janela temporal, população-alvo ou transformação, documente isso em linguagem natural.
8. Se uma métrica desejada não for observável ou estiver apenas parcialmente observável, rotule-a como tal.
9. Não trate dado carregado sem erro como dado validado.
10. Não apresente resultados como definitivos quando dependerem de revisão de fonte, validação técnica ou decisão humana.

---

## Regras de interação e execução

1. Não faça perguntas evitáveis quando o repositório e as fontes validadas já responderem a dúvida.
2. Quando perguntas forem realmente necessárias, numere-as.
3. Antes de tarefa complexa, exija plano curto, revisável e auditável.
4. Tarefas complexas devem ser executadas em fases curtas, com checkpoints claros.
5. Não reabra decisão já validada sem nova evidência, nova fonte canônica ou mudança de escopo aprovada.
6. Preserve continuidade com decisões previamente validadas.
7. Prefira um artefato integrado, limpo e validado a múltiplos rascunhos parcialmente sobrepostos.

---

## Execução agêntica

1. O projeto pode usar arquitetura multiagente hierárquica quando a complexidade justificar.
2. O uso de MAS deve sempre partir de um agente orquestrador responsável por:
   - classificar a tarefa;
   - definir os agentes ativos;
   - controlar a ordem de execução;
   - consolidar outputs;
   - respeitar os gates definidos pelo workflow.
3. Em tarefas simples, prefira agente único com ferramentas.
4. Em tarefas complexas, o plano deve declarar:
   - quais agentes serão ativados;
   - por que serão ativados;
   - quais ferramentas cada agente poderá usar;
   - quais guardrails se aplicam;
   - quais critérios determinam aprovação, rejeição, bloqueio ou interrupção.
5. Nenhum agente pode alterar silenciosamente fonte canônica, regra validada, artefato aprovado ou memória persistente do projeto.
6. O uso de múltiplos agentes não elimina a obrigação de simplicidade, rastreabilidade, Programação Letrada, validação e documentação.
7. Se o uso de MAS aumentar custo, latência ou retrabalho sem ganho claro de qualidade, a arquitetura deve ser simplificada.

--- 

## Memória, RAG e proveniência

1. Distinga explicitamente:
   - memória operacional de sessão;
   - memória canônica do projeto;
   - memória de padrões validados;
   - recuperação via RAG.
2. Memória operacional serve para continuidade da execução, não para redefinir a verdade do projeto.
3. A memória canônica do projeto deve ser composta apenas por:
   - instruções explícitas do Professor;
   - documentação canônica;
   - decisões aprovadas;
   - handoffs e artefatos validados.
4. Correções locais, histórico de chat, outputs transitórios e logs não devem ser promovidos automaticamente a memória longa.
5. Toda recuperação via RAG deve indicar sua fonte e respeitar a hierarquia de evidência do projeto.
6. Quando houver conflito entre memória recuperada e fonte canônica, prevalece a fonte canônica.
7. Conteúdo metodológico, técnico ou substantivo recuperado via RAG deve ser tratado como insumo verificável, não como verdade autoevidente.

---

## Guardrails e isolamento

1. Toda arquitetura agêntica deve usar, quando aplicável:
   - guardrails de input;
   - guardrails de output;
   - guardrails de tool;
   - guardrails de workflow.
2. Código, edição de arquivos, acesso a conectores e manipulação de dados sensíveis devem ocorrer em ambiente isolado quando houver risco de efeito colateral.
3. Alterações em arquivos canônicos, exportações externas, operações destrutivas e gravações em memória persistente devem exigir aprovação quando o risco justificar.
4. O princípio de menor privilégio deve orientar o acesso de cada agente a arquivos, ferramentas, conectores e fontes.
5. Nenhum agente deve receber mais contexto, memória ou permissão do que o estritamente necessário para sua função.

--- 

## Tracing, avaliação e desempenho

1. Fluxos agênticos complexos devem registrar:
   - identificador de execução;
   - agentes acionados;
   - ferramentas usadas;
   - outputs críticos;
   - rejeições, bloqueios, interrupções e retomadas;
   - artefatos produzidos.
2. Toda fase deve ter critérios explícitos de aprovação.
3. O uso de múltiplos agentes deve ser reavaliado sempre que aumentar custo, latência ou retrabalho sem ganho proporcional.
4. Benchmarks, testes, logs, pareceres e auditorias devem ser usados para ajustar prompts, handoffs, ferramentas e guardrails.
5. Se nenhuma entidade for claramente responsável por um check crítico, esse check deve ser considerado inexistente e a fase não deve ser aprovada.


--- 
## Programação Letrada e padrões de implementação

1. **Programação Letrada é obrigatória em qualquer linguagem usada no projeto**, incluindo R, Python, SQL, Quarto, R Markdown, Jupyter e outras.
2. Toda implementação com código deve intercalar código com explicação clara em linguagem natural.
3. A explicação deve cobrir, no mínimo:
   - objetivo do bloco;
   - inputs;
   - outputs;
   - regras de negócio aplicadas;
   - premissas;
   - transformações realizadas;
   - validações executadas;
   - interpretação do resultado.
4. Entrega apenas com código não é suficiente, salvo autorização explícita do Professor.
5. Formatos preferenciais incluem:
   - `.qmd`;
   - `.Rmd`;
   - notebooks Jupyter;
   - notas de execução em `.md`;
   - scripts acompanhados de documentação equivalente.
6. Se scripts planos forem usados, eles ainda devem conter:
   - cabeçalhos de seção claros;
   - comentários úteis;
   - documentação suficiente para auditoria humana;
   - referência explícita à documentação explicativa associada.
7. Use nomes significativos e específicos para variáveis, funções, objetos, tabelas e arquivos.
8. Mantenha convenção de nomenclatura consistente dentro de cada linguagem e componente.
9. Use comentários e espaços em branco para melhorar legibilidade, não para compensar má estrutura.
10. Mantenha formatação e indentação consistentes.
11. Separe, sempre que possível:
    - ingestão;
    - transformação;
    - aplicação de regra de negócio;
    - validação;
    - geração de output.
12. Evite efeitos colaterais ocultos.
13. Salve outputs intermediários relevantes quando isso melhorar rastreabilidade.
14. Teste caminhos críticos com exemplos controlados, dados sintéticos ou testes formais, quando aplicável.
15. Use tratamento explícito de erros quando falhas forem previsíveis.
16. Prefira eficiência quando ela não sacrificar clareza, auditabilidade ou segurança.

---

## Convenções gerais de repositório

Use a estrutura documentada do repositório.  
Na ausência de convenção específica, adote as seguintes diretrizes:

1. preserve arquivos brutos exatamente como recebidos;
2. não sobrescreva dados brutos;
3. use caminhos relativos à raiz do projeto;
4. organize outputs para que outro revisor consiga identificar sua origem;
5. use nomes de arquivo descritivos, com tema, versão e data quando útil;
6. não inclua dados identificáveis em outputs analíticos, salvo domínio seguro explicitamente documentado;
7. quando exemplos forem necessários, prefira registros mascarados ou sintéticos.

---

## Governança de dados e segurança

1. Trate como sensíveis dados pessoais, identificáveis, confidenciais, contratuais, financeiros, institucionais ou protegidos por regra específica.
2. Separe o domínio analítico do domínio identificável sempre que a arquitetura permitir.
3. Audite exportações.
4. Prefira chaves substitutas nas camadas analíticas.
5. Não exponha dados identificáveis além do estritamente necessário para uso autorizado.
6. Recomende controles de acesso por perfil quando houver múltiplos usuários ou diferentes níveis de sensibilidade.
7. Registre riscos de privacidade, segurança e uso indevido quando a tarefa tocar dados sensíveis.
8. Se o projeto tiver regras específicas de domínio, siga as fontes canônicas do subprojeto correspondente.

---

## Validação e qualidade

1. Não assuma que dados estão limpos porque carregaram com sucesso.
2. Valide schema, campos obrigatórios, tipos, datas, chaves e valores incompatíveis.
3. Documente explicitamente:
   - filtros;
   - exclusões;
   - recodificações;
   - joins;
   - transformações;
   - variáveis derivadas.
4. Valide:
   - correção computacional;
   - plausibilidade de negócio;
   - coerência metodológica.
5. Salve outputs verificáveis quando aplicável:
   - tabelas;
   - resumos de modelo;
   - diagnósticos;
   - logs;
   - notas de validação.
6. Verifique se código e outputs são compreensíveis para um revisor humano, não apenas executáveis por máquina.
7. Em entregas com Programação Letrada, valide a coerência entre:
   - código;
   - explicação;
   - regra aplicada;
   - output resultante.
8. Se uma transformação, filtro, indicador derivado ou decisão analítica não estiver explicada em linguagem natural, a tarefa não está plenamente documentada.

---

## Tratamento de erros

1. Quando uma etapa falhar, não apenas repita o mesmo comando.
2. Diagnostique primeiro.
3. Aja com base no diagnóstico.
4. Se o problema persistir, registre:
   - o erro exato;
   - o que foi testado;
   - o que permanece bloqueado.
5. Se o bloqueio decorrer de conflito entre fontes, documente o conflito explicitamente.
6. Se o bloqueio decorrer de ausência de fonte canônica obrigatória, interrompa e reporte a dependência ausente.
7. Não contorne silenciosamente um erro que altere regra de negócio, integridade analítica ou segurança.

---

## Documentação e handoff

Toda tarefa substantiva deve deixar rastro suficiente para revisão e retomada.

Documente:

1. o que foi feito;
2. por que foi feito;
3. quais fontes foram usadas;
4. quais regras de negócio foram implementadas ou respeitadas;
5. o que foi validado;
6. como rerodar, continuar ou auditar o trabalho;
7. quais outputs foram gerados;
8. o que permanece pendente;
9. o que exige aprovação do Professor;
10. o que cada script, notebook, consulta ou artefato executável faz;
11. quais inputs ele espera;
12. quais outputs ele gera;
13. quais regras, thresholds ou transformações aplica;
14. onde está a explicação humana da lógica implementada.

O handoff deve permitir retomada sem reconstrução de contexto a partir do histórico do chat.

---

## Checklist de conclusão

Antes de marcar qualquer tarefa substantiva como concluída, verifique:

1. o modo principal da tarefa foi identificado corretamente;
2. as fontes canônicas apropriadas foram usadas;
3. o output respeita o escopo aprovado;
4. regras de negócio e restrições relevantes foram preservadas;
5. alegações factuais foram validadas;
6. restrições de segurança e acesso foram respeitadas, quando aplicáveis;
7. outputs estão salvos, prontos para salvar ou claramente descritos;
8. documentação foi atualizada;
9. pendências e incertezas remanescentes estão listadas;
10. os requisitos de Programação Letrada foram satisfeitos quando houve código;
11. a lógica implementada é compreensível para um revisor humano sem reconstrução a partir da execução;
12. a implementação atende aos padrões de legibilidade, nomenclatura, documentação, validação, tratamento de erros e auditabilidade do projeto.

Se qualquer item falhar, a tarefa não está concluída.