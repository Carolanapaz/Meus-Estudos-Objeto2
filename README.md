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
  if (imc < 18.5) {
    return ('Abaixo do peso');
} else if (imc >= 18.5 && imc < 25) {
   return ('Peso normal');
} else if (imc >= 25 && imc < 30) {
   return ('Acima do peso');
} else if (imc >= 30 && imc < 40) {
   return ('Obeso');
} else {
   return('Obesidade grave');
}
  
  }
}


const carol = new Pessoa('Carol', 69, 1.59);
console.log(carol.calcularImc());
console.log(carol.classificarImc());
