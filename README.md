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
  
  calcularGastoDePercurso(distancia, precoCombustivel) {
    return distancia * this.gastoMedioPorKm * precoCombustivel;
}

const uno = new Carro ('Fiat', 'Vermelho', 1/12);
console.log(uno.calcularGastoDePercurso(20,5));
