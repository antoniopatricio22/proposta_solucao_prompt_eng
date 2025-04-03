# proposta_solucao_prompt_eng


## Questão 1:

**Técnica utilizada: Context, instructions, details, Input (CIDI)**

**Prompt:**
```
Explique passo a passo como o algoritmo de Ray Tracing calcula a cor de um pixel em uma imagem renderizada. Inclua os conceitos matemáticos e físicos envolvidos, as etapas principais do processo, e como são calculadas as interações com diferentes materiais. Use exemplos concretos quando possível.
```

- A estrutura passo a passo força a IA a organizar informações complexas sequencialmente

## Questão 2:

**Técnica utilizada: Chain-of-Thought Prompting (CoT)**

**Prompt:**
```
Realize a decomposição numérica completa do número 142.981. Por favor:
1. Detalhe cada etapa do processo
2. Mostre a decomposição em fatores primos
3. Identifique todos os divisores do número
4. Apresente a representação do número em diferentes bases (decimal, binária, octal, hexadecimal)
5. Calcule a soma dos dígitos

Explique cada passo do seu raciocínio antes de fornecer a resposta final.
```

- Solicitar explicitamente que a IA mostre seu raciocínio reduz erros matemáticos
- A estrutura numerada define claramente as partes da decomposição desejada
- Solicitar a explicação de cada passo torna o conteúdo mais didático

## Questão 3: 

**Técnica utilizada: Zero-shot Prompting + Chain-of-Thought Prompting (CoT)**

**Prompt:**
```
Analise detalhadamente quais personagens da saga "As Crônicas de Gelo e Fogo" de George R.R. Martin possuem características inspiradas na filosofia política de Nicolau Maquiavel, especialmente aquelas encontradas em "O Príncipe".

Para cada personagem identificado:
1. Cite evidências específicas de seus comportamentos nos livros
2. Compare diretamente com os princípios maquiavélicos correspondentes
3. Explique como esses personagens demonstram pragmatismo político, separação entre moralidade e governança, ou a ideia de que "os fins justificam os meios"

Baseie sua análise apenas nos livros da série, não na adaptação para TV "Game of Thrones".
```


- Estabelece contexto claro (livros, não série de TV)
- Define parâmetros específicos para a análise (princípios maquiavélicos específicos)
- A estrutura comparativa força a IA a fazer conexões significativas entre a filosofia e os personagens

## Questão 4:

**Técnica utilizada: Tree of Thoughts**

**Prompt:**
```
Crie um endpoint completo usando FastAPI que valide e processe a entrada de um objeto do tipo `Item` com as seguintes especificações:

Estrutura do Item:
- nome: string com tamanho máximo de 25 caracteres
- valor: float
- data: valor do tipo date, que não pode ser superior à data atual

Requisitos:
- O endpoint deve validar todos os valores recebidos
- Após validação, retornar o corpo da requisição com um campo adicional "uuid" contendo um identificador único gerado dinamicamente

Por favor:
1. Forneça o código Python completo e funcional
2. Inclua todas as importações necessárias
3. Adicione comentários explicando cada parte importante do código
4. Explique como o Pydantic é usado para validação
5. Mostre um exemplo de como testar o endpoint
```


- As especificações são claras e completas
- Pedir explicações sobre Pydantic garante que a validação seja implementada corretamente
- Solicitar um exemplo de teste ajuda a verificar a funcionalidade
- A estrutura numerada garante que todos os requisitos sejam atendidos
