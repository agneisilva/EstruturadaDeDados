# Repositório de Códigos das Aulas de Estruturas de Dados

Bem-vindo(a) ao repositório oficial da disciplina de Estruturas de Dados!

Este espaço foi criado para centralizar todos os códigos-fonte, exemplos e algoritmos desenvolvidos durante nossas aulas. O objetivo é que sirva como um material de apoio confiável para consulta, estudo e aprofundamento nos conceitos abordados.

## 📚 Tópicos Abordados

Navegue pelos principais temas que exploramos. Cada seção contém uma breve explicação teórica que serve como referência para o código-fonte correspondente.

### 1. Árvores (Trees)
As árvores são estruturas de dados não lineares e hierárquicas, fundamentais na computação para representar informações com relações de parentesco, como sistemas de arquivos, organogramas ou o DOM de uma página web.

* **Terminologia Essencial**:
    * **Nó (Node)**: O elemento que armazena a informação.
    * **Raiz (Root)**: O nó do topo da árvore.
    * **Filho (Child)**: Um nó conectado diretamente a outro nó (seu pai) em um nível inferior.
    * **Pai (Parent)**: O nó predecessor de um filho.
    * **Folha (Leaf)**: Um nó que não possui filhos.
    * **Altura (Height)**: O comprimento do caminho mais longo da raiz até uma folha.
    * **Profundidade (Depth)**: O comprimento do caminho da raiz até um nó específico.

### 2. Árvores Binárias de Busca (BST - Binary Search Tree)
Uma BST é uma árvore binária com uma propriedade de ordenação fundamental que torna as operações de busca, inserção e remoção extremamente eficientes.

* **Propriedade da BST**: Para qualquer nó `N`, todos os valores em sua subárvore esquerda são **menores** que `N`, e todos os valores em sua subárvore direita são **maiores** que `N`.

* **Operações e Desempenho**:
    * **Busca, Inserção e Remoção**: O código implementa os algoritmos recursivos para essas operações.
    * **Complexidade**: No caso médio, as operações têm complexidade **O(log n)**. No pior caso (árvore desbalanceada), a complexidade degenera para **O(n)**.

### 3. Travessias em Árvores (Tree Traversal)
Travessia é o processo de visitar cada nó da árvore exatamente uma vez. As estratégias definem a ordem em que os nós são processados.

* **In-Order (Em Ordem)**: `Esquerda → Raiz → Direita`. Em uma BST, essa travessia visita os nós em ordem crescente.
* **Pre-Order (Pré-Ordem)**: `Raiz → Esquerda → Direita`. Útil para criar cópias de árvores.
* **Post-Order (Pós-Ordem)**: `Esquerda → Direita → Raiz`. Usado para deletar nós da árvore com segurança.

### 4. Árvores Balanceadas (AVL)
Para resolver o problema do pior caso da BST, utilizamos árvores de busca auto-balanceadas. A árvore AVL é um exemplo clássico.

* **Fator de Balanceamento**: A principal regra da AVL é que, para qualquer nó, a diferença de altura entre suas subárvores esquerda e direita não pode ser maior que 1.
* **Rotações**: Quando uma inserção ou remoção quebra a regra do balanceamento, a árvore executa **rotações** (simples ou duplas) para se reorganizar e manter a altura logarítmica, garantindo o desempenho **O(log n)** em todas as operações.

### 5. Aplicação Prática: Árvore de Expressão Aritmética
Uma aplicação poderosa das árvores é a representação de expressões matemáticas.

* **Estrutura**: Os nós internos são os **operadores** (+, -, \*, /) e os nós folha são os **operandos** (números e variáveis).
* **Funcionamento**: A estrutura da árvore respeita nativamente a precedência de operadores e o uso de parênteses, permitindo a avaliação de expressões complexas. O código-fonte demonstra como construir essa árvore a partir de uma string.

## 📂 Estrutura do Repositório

Os códigos estão organizados em pastas, seguindo a ordem das aulas para facilitar a localização do material:

```
.
├── Aula-01-Conceitos-BST/
│   └── bst_completa.py
├── Aula-02-Travessias-AVL/
│   └── arvore_avl.py
├── Aula-03-Arvores-de-Expressao/
│   └── expressao_aritmetica.py
└── README.md
```

## ⚙️ Como Executar o Código

### Pré-requisitos
* **Python 3.x** instalado.
* **Graphviz**: Muitos exemplos utilizam a biblioteca `graphviz` para gerar visualizações das árvores. É uma ferramenta poderosa para entender o que o código está fazendo.

### Instalação
1.  **Instale o software Graphviz no seu sistema:**
    * **Linux (Ubuntu/Debian)**: `sudo apt-get install graphviz`
    * **macOS (usando Homebrew)**: `brew install graphviz`
    * **Windows**: Baixe o instalador no [site oficial](https://graphviz.org/download/) e adicione o diretório `bin` ao PATH do sistema.

2.  **Instale a biblioteca Python:**
    ```bash
    pip install graphviz
    ```

### Execução de um Exemplo
Para rodar um dos arquivos, navegue até a pasta correspondente e execute o script Python:
```bash
# Exemplo para rodar o código da BST
cd Aula-01-Conceitos-BST/
python bst_completa.py
```

## 💬 Contribuições

Encontrou um bug, tem alguma dúvida ou uma sugestão para melhorar um código? Sinta-se à vontade para abrir uma **Issue** neste repositório! O feedback é sempre bem-vindo.

---
*Desenvolvido por **[Seu Nome]***
