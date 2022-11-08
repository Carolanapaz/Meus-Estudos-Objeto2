# Meus-Estudos-Objeto2

class Carro {
  marca;
  cor;
  gastoMedioPorKm;
  
  constructor(marca, cor, gastoMedioPorKm) {
    this.marca = marca;
    this.cor = cor;
    this.gastoMedioPorKm = gastoMedioPorKm;
  }
  
  calcularGastoDePercurso(distancia, precoCombustivel) {
    return distancia * this.gastoMedioPorKm * precoCombustivel;
  }
}

const uno = new Carro('Fiat', 'Vermelho', 1 / 12);
console.log(uno);
console.log(uno.calcularGastoDePercurso(70, 5));

-----------------------------------------------------------

class Pessoa {
  nome;
  peso;
  altura;
  
  constructor(nome, peso, altura) {
  this.nome = nome;
  this.peso = peso;
  this.altura = altura;
  }
  
  calcularImc() {
  return this.peso / Math.pow(this.altura, 2);
  }
  
  classificarImc(){
  const imc - this.calcularImc();
  
  }
}

const jose = new Pessoa('Jose', 60, 1.59);
console.log(jose.calcularImc());

const carol = new Pessoa('Carol', 69, 1.59);
console.log(carol.calcularImc());
