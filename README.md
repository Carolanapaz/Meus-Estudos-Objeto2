# Meus-Estudos-Objeto2

class Carro {
  marca;
  cor;
  gastoMedioPorKm;
  
  construtor (marca, cor, gastoMedioPorKm) {
    this.marca = marca;
    this.cor = cor;
    this.gastoMedioPorKm = gastoMedioPorKm;
  }
  
  
}

const uno = new Carro ('Fiat', 'Vermelho', 1/12);
console.log(uno);
