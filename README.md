# Laboratório de Prompts — Cucando TI

Playground didático para aprender a **estruturar, editar e revisar prompts**. O aluno experimenta quatro componentes, delimitadores e estratégias de solicitação, observa uma demonstração passo a passo e pode copiar seu próprio prompt ao final.

O ambiente funciona inteiramente no navegador. As demonstrações e a avaliação são **simulações locais para aprendizagem**: não enviam o prompt a uma IA.

## Começar

1. Coloque este `README.md` e o arquivo `playground-prompts-cucando-ti.html` na mesma pasta.
2. Abra o HTML em um navegador moderno, no computador ou no celular. Não é preciso instalar pacotes, configurar chave de API ou ter internet.
3. Edite os blocos de **Estrutura do prompt**. O painel **Prompt montado** atualiza o texto à medida que você escreve.

Se quiser usar o HTML como página inicial de um repositório, renomeie uma cópia para `index.html`. O arquivo continua autocontido.

## Estrutura do exercício

O editor começa com um exemplo fictício de atendimento em uma loja de eletrônicos, organizado em quatro partes:

1. **Instrução (A Ação Central):** o comando que define o que fazer.
2. **Contexto (O Cenário de Fundo):** informações e restrições da situação.
3. **Exemplos (Padrão Ouro de Entrada/Saída):** pares que ilustram a resposta esperada.
4. **Tarefa Final (O Gatilho Imediato):** o dado específico a processar agora.

O aluno pode escrever em cada campo, ativar ou desativar blocos, abrir e recolher exemplos pelo botão `?`, mudar a ordem pela alça ou pelas setas `↑` e `↓` e adicionar uma seção própria. A estrutura pronta pode ser carregada novamente pela caixa de ferramentas.

## Caixa de ferramentas

Clique em um delimitador para inseri-lo no último campo editado, ou arraste-o até um bloco:

| Delimitador | Uso apresentado no laboratório |
| --- | --- |
| `#` | Título principal |
| `---` | Separação entre seções |
| `###` | Subcabeçalho |
| `"""` | Delimitação de um trecho de conteúdo |
| `**` | Ênfase em Markdown |
| `[ ]` | Campo reservado para preenchimento |
| `{{ }}` | Variável a substituir manualmente ou por código |
| `<tag>` | Trecho identificado por uma tag nomeada |

Esses símbolos ajudam a tornar a estrutura legível. **Não garantem que um modelo siga as instruções, valide dados ou isole conteúdo inseguro.**

## Estratégias de prompt

Em **Laboratório de estratégias**, escolha uma opção e use **Carregar modelo** para trazê-la ao editor. A demonstração é controlada pelo aluno ou professor: **Executar demonstração**, **Próxima etapa**, **Voltar etapa** e **Recomeçar**.

| Modo | O que comparar |
| --- | --- |
| **Zero-shot** | Pedido direto sem exemplo resolvido |
| **Few-shot** | Pedido com exemplos de entrada e saída |
| **CoT** | Etapas explicativas observáveis e justificativa concisa |
| **ToT** | Alternativas, critérios de comparação e árvore de decisão ilustrativa |

As saídas e a árvore são **exemplos fixos**, não a resposta de uma IA nem uma exposição de raciocínio interno. O exercício permite discutir a diferença entre os formatos dos prompts sem exigir acesso a serviços externos.

## Avaliação orientativa

Ao terminar, clique em **Avaliar meu prompt** no fim de **Estrutura do prompt**. O sistema examina sinais observáveis do texto e apresenta uma tabela com **nota de 1 a 3 e justificativa breve** para cada critério:

| Critério | 1 | 2 | 3 |
| --- | --- | --- | --- |
| Clareza | Confuso | Parcialmente claro | Muito claro |
| Estrutura | Ausente | Parcial | Completa |
| Especificidade | Genérico | Moderado | Altamente específico |
| Criatividade | Pouco criativo | Criativo | Muito criativo |
| Aplicabilidade | Pouco útil | Útil | Altamente útil |
| Tom e Estilo | Não definido | Parcialmente definido | Bem definido |
| Engajamento | Pouco envolvente | Envolvente | Muito envolvente |
| Consistência | Inconsistente | Parcialmente consistente | Totalmente consistente |
| Autonomia | Muitas correções necessárias | Pequenos ajustes | Totalmente autônomo |

A devolutiva inclui **pontuação total de até 27 pontos**, percentual em uma régua do vermelho ao verde, **ponto forte** e **uma sugestão prática de melhoria**. O prompt **permanece no editor** depois da avaliação, para que o aluno o ajuste e envie novamente. O histórico mostra os últimos cinco envios e a variação em relação ao anterior. Quando o texto é alterado, a interface informa que a nota exibida pertence à versão anterior.

A nota é **heurística e orientativa**. Ela detecta características textuais, mas não consegue julgar plenamente criatividade, utilidade, engajamento ou coerência sem leitura humana. Por exemplo, uma contradição não detectada não equivale a uma garantia de consistência.

## Copiar, baixar e reiniciar

- **Copiar prompt** envia o texto montado para a área de transferência, quando o navegador permitir.
- **Baixar .txt** salva o texto em um arquivo local.
- **Reiniciar** restaura o exemplo inicial e limpa alterações, avaliação, histórico e andamento das demonstrações em um clique.
- O rascunho e os últimos resultados são guardados **somente no navegador usado**. Limpar os dados desse navegador pode apagá-los.

## Organização técnica

- Um único arquivo HTML com CSS e JavaScript incorporados, sem dependências externas.
- Layout adaptado a telas maiores e celulares; a tabela de avaliação vira uma sequência de cartões em telas estreitas.
- Os dados não são enviados a servidor; a análise funciona localmente.

## Créditos

Desenvolvido pela equipe **Cucando TI** para aprendizagem de engenharia de prompt.
