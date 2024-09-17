
#**Introdução à Programação Orientada a Objetos (POO) com Javascript**

*IMPORTANTE: Esta é uma atividade prática de estudo-dirigido. Somente inicie-a usando o VSCode e praticando no editor de códigos.*

A Programação Orientada a Objetos (POO) visa ampliar o conceito de variáveis compostas, como os vetores (ou matrizes), introduzindo uma maneira mais complexa de estruturar e organizar dados.

### Vetores:

Vetores são estruturas que permitem armazenar múltiplos valores sob uma única variável, acessados por seus índices. Um exemplo simples é o vetor de `Strings`:

```js
let frutas = ["Maçã", "Banana", "Laranja"];
```

Cada valor é referenciado por seu índice no vetor.

### Objetos:

Na POO, os objetos também podem ser vistos como variáveis, mas com uma diferença crucial: eles podem conter múltiplos valores (ou propriedades) que são armazenados e acessados como pares chave-valor. Esses valores compostos são frequentemente organizados em um formato mais legível:

```js
let carro = {
  marca: "Volvo",
  modelo: "Volvo 360",
  cor: "branco",
  ano: 2019
};
```

Aqui, `carro` é um objeto com quatro propriedades (`marca`, `modelo`, `cor`, `ano`), cada uma com seu valor correspondente.

### Classes:

Uma classe pode ser entendida como um "molde" para criar objetos. A classe define as propriedades e comportamentos que seus objetos terão, mas não atribui valores diretamente. Para isso, usamos *instâncias*.

### Inicialização de Objetos: Instâncias

Assim como variáveis precisam ser inicializadas com um valor, por exemplo:

```js
int notaAluno = 7;
```

Os vetores são inicializados com valores entre colchetes `[]`, e cada valor é acessado por seu índice:

```js
int[] notas = {7, 8, 9};
```

De forma similar, objetos de uma classe precisam ser instanciados, ou seja, receber valores. Ao criar um objeto de uma classe, usamos o *construtor*, que é uma função especial que inicializa as propriedades do objeto.

#### Exemplo de Classe:

```js
class Carro {
  constructor(marca, modelo, cor, ano) {
	this.marca = marca;
	this.modelo = modelo;
	this.cor = cor;
	this.ano = ano;
  }
}
```

Aqui, `Carro` é uma classe com um construtor que define suas propriedades (`marca`, `modelo`, `cor`, `ano`). O operador `this` é utilizado para referenciar a instância atual da classe.

### Instanciando Objetos:

Para criar um objeto (instância) da classe `Carro`, fazemos o seguinte:

```js
let meuCarro = new Carro("Volvo", "Volvo 360", "branco", 2019);
```

Agora, `meuCarro` é uma instância da classe `Carro`, e podemos acessar suas propriedades da seguinte forma:

```js
console.log(meuCarro.marca); // Saída: "Volvo"
```

### Templates de Classes:

Classes funcionam como templates para criar múltiplos objetos, com propriedades e métodos compartilhados. Ao criar um novo objeto a partir de uma classe, é possível visualizar as propriedades disponíveis no VSCode ao passar o mouse sobre a classe ou o objeto.

### Propriedades da Classe:

As propriedades de uma classe são variáveis associadas a objetos instanciados dessa classe. Essas propriedades podem ser acessadas e modificadas após a criação do objeto. Exemplo:

```js
let pessoa1 = new Pessoa("João", 25);
let pessoa2 = new Pessoa("Maria", 30);

console.log(pessoa1.name); // Saída: "João"
console.log(pessoa2.age);  // Saída: 30
```

