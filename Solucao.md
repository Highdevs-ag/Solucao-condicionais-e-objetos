//Exercício 1: Verificando a Idade

const idade = parseInt(prompt("Digite sua idade: "));

if (idade >= 18) {
  console.log("Você é maior de idade");
} else {
  console.log("Você é menor de idade");
}

//Exercício 2: Cumprimentando com Base no Turno

const turno = prompt("Digite o turno em que você estuda (M, V ou N): ");

if (turno === "M") {
  console.log("Bom Dia!");
} else if (turno === "V") {
  console.log("Boa Tarde!");
} else if (turno === "N") {
  console.log("Boa Noite!");
} else {
  console.log("Turno não reconhecido.");
}

//Exercício 3: Cumprimentando com Base no Turno (Switch Case)

const turno = prompt("Digite o turno em que você estuda (M, V ou N): ");

function cumprimentar(turno) {
  switch (turno) {
    case "M":
      return "Bom Dia!";
    case "V":
      return "Boa Tarde!";
    case "N":
      return "Boa Noite!";
    default:
      return "Turno não reconhecido.";
  }
}

console.log(cumprimentar(turno));

//Exercício 4: Verificando Filme Favorito

const filme = {
  nome: prompt("Digite o nome do seu filme favorito: "),
  genero: prompt("Digite o gênero do filme: "),
};

if (filme.genero.toLowerCase() === "fantasia" && prompt("O ingresso custa R$20 ou menos? (S/N): ").toLowerCase() === "s") {
  console.log("Bom filme!");
} else {
  console.log("Escolha outro filme :(");
}

//Exercício 5: Candidatura a Bolsa de Estudos

const aluno = {
  nome: "João",
  idade: 25,
  curso: "Engenharia",
  temBolsa: false,
};

if (aluno.idade < 30 && aluno.curso === "Engenharia" && !aluno.temBolsa) {
  console.log("Você pode se candidatar a uma bolsa de estudos!");
} else {
  console.log("Desculpe, você não atende aos requisitos para a bolsa.");
}

//Exercício 6: Calculando Preço Final do Produto

const produto = {
  nome: "Notebook",
  preco: 1500,
  desconto: 200,
  freteGratis: true,
};

const precoFinal = produto.preco - produto.desconto;

if (produto.freteGratis) {
  console.log(`Preço final: R$${precoFinal} (Frete Grátis)`);
} else {
  console.log(`Preço final: R$${precoFinal}`);
}

//Essas são as versões em JavaScript dos exercícios
