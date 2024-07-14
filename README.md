
## Sistema de Controle de Acesso com RFID

**Funcionalidades**

- **Identificação por RFID:** Utiliza um leitor RFID para ler os cartões.
- **Controle de Acesso:** Determina se o acesso deve ser concedido ou negado com base na identificação do cartão.
- **Feedback Visual:** Fornece feedback visual através de um dispositivo indicando se o acesso foi permitido ou negado.

**Explicação das Tags no Código C++ da Classe LeitorRFID**
```markdown
### Declaração da Classe e Funções:

class LeitorRFID {
public:
  // Construtor
  LeitorRFID(int inicioMemoria, int fimMemoria, int tamanhoCartao);

  // Função para ler dados do cartão RFID
  std::string lerCartaoRFID(int enderecoMemoria);

  // Função para consultar o banco de dados
  bool consultarBancoDados(const std::string& dadosCartao);

  // Função para adicionar um cartão ao banco de dados
  void adicionarCartaoAoBancoDados(const std::string& dadosCartao);
};
```

**1. `class`:**

- Define o início de uma declaração de classe. O nome da classe é `LeitorRFID`.
- As funções e variáveis dentro da classe são consideradas membros da classe.

**2. `public`:**

- Especifica que os membros da classe a seguir (funções) são acessíveis de fora da classe.

**3. Construtor:**

- Uma função especial que é chamada para inicializar um objeto da classe.
- O nome do construtor é o mesmo nome da classe.
- A lista entre parênteses (`int inicioMemoria, int fimMemoria, int tamanhoCartao`) define os parâmetros do construtor.

**4. Declaração de Funções:**

- Declara as funções membro da classe.
- Especifica o tipo de retorno da função (por exemplo, `std::string` para `lerCartaoRFID`), o nome da função, a lista de parâmetros entre parênteses e o tipo de valor de cada parâmetro.
- A função `consultarBancoDados` recebe um parâmetro constante `std::string` chamado `dadosCartao`.
- A função `adicionarCartaoAoBancoDados` recebe um parâmetro constante `std::string` chamado `dadosCartao`.

**5. Definição de Funções:**

```cpp
// Definição da função lerCartaoRFID
std::string LeitorRFID::lerCartaoRFID(int enderecoMemoria) {
  // ...
}

// Definição da função consultarBancoDados
bool LeitorRFID::consultarBancoDados(const std::string& dadosCartao) {
  // ...
}

// Definição da função adicionarCartaoAoBancoDados
void LeitorRFID::adicionarCartaoAoBancoDados(const std::string& dadosCartao) {
  // ...
}
```

- As definições das funções fornecem o código que será executado quando as funções forem chamadas.
- O operador de escopo `::` separa o nome da função do nome da classe.
- O conteúdo das funções está entre chaves `{}`.

**6. Tipos de Dados:**

- `int`: Tipo de dado inteiro para armazenar números inteiros (por exemplo, `inicioMemoria`, `fimMemoria`, `tamanhoCartao`).
- `std::string`: Tipo de dado string para armazenar strings de texto (por exemplo, `dadosCartao`).
- `bool`: Tipo de dado booleano para armazenar valores true ou false (por exemplo, `cartaoValido`).
- `vector<std::string>`: Tipo de dado container `vector` para armazenar uma lista de strings (por exemplo, `bancoDados`).

**7. Palavras-chave:**

- `class`: Define uma classe.
- `public`: Especifica acesso público aos membros da classe.
- `const`: Indica que um parâmetro ou variável não pode ser modificado.
- `return`: Retorna um valor da função.
- `if`: Executa um bloco de código se uma condição for verdadeira.
- `else`: Executa um bloco de código se a condição do `if` for falsa.
- `for`: Repete um bloco de código um número específico de vezes.
- `push_back`: Adiciona um elemento ao final de um container `vector`.

**8. Operadores:**

- `==`: Operador de comparação para verificar se dois valores são iguais.
- `!=`: Operador de comparação para verificar se dois valores são diferentes.
- `+`: Operador de adição para somar dois números.
```
