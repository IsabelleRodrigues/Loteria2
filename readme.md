# Simulador de Loteria

Esse projeto é um simulador da *megasenna* onde o usuário digita 6 números e selecionamos aleatoriamente e comparamos para verificar quantos números você acertou.

**Não é um simulador oficial / para jogos oficiais.**

## Tecnologias utilizadas:
1. **HTML**: (Abreviação para a expressão inglesa HyperText Markup Language), que significa Linguagem de Marcação de Hipertexto, e é uma linguagem de marcação utilizada na construção de páginas na Web;
2. **CSS**: (Cascading Style Sheets) é um mecanismo para adicionar estilo (cores, fontes, espaçamento, etc.) a um documento web;
3. **JS**: (frequentemente abreviado como JS) é uma linguagem de programação interpretada estruturada, de script em alto nível com tipagem dinâmica fraca e multiparadigma (protótipos, orientado a objeto, imperativo e, funcional);
4. ~~**Jquery**~~

## Funções principais
Aqui será apresentado as duas funções principais do site.

### Sorteio de números
Nessa função os números são sorteados aleatoriamente.
```
function sortearNumeros()
{
  numSort = [];
  let sort;

  for (var i = 0; i < 6; i++)
  {
  do
  {
   sort = Math.ceil(Math.random() * 60);
   sort = (sort==0) ? 1: sort;
 }while (numSort.includes(sort));

 numSort.push(sort);
   }
 }
```

### Lendo os números digitados
Lê as entradas de número digitadas pelo usuário.
```
function addToList(num, pos)
{
  if (num.length ==2 )
  {
    if (numEsco.includes(num))
    {
        alert2("Erro", "Número ja escolhido, informe outro número");
    }
    else if (parseInt(num) >  60)
    {
        alert2("Erro", "Numero digitado nao pode ser maior que 60");
    }
    else
    {
      numEsco[pos-1]=num;
    }
  }
}
```
## Como rodar o código
>Simplesmente baixe e abra o arquivo **_index.html_** no seu navegador;

## Exemplo de tabela
Exemplo   | Valor do Exemplo | Quantidade  |
----------|------------------|-------------|
Exemplo 1 |R$ 10,00          |5            |
Exemplo 2 |R$ 08,00          |4            |
Exemplo 3 |R$ 07,00          |34           |
Exemplo 4 |R$ 08,00          |23           |

## Imagens da tela
Tela 1: Tela de abertura
![Tela1](/imagens/tela1.png)

Tela 2: 6 números digitados e 2 acertos
![Tela2](/imagens/tela2.png)

## Referências
* HTML: [Wikipedia](https://pt.wikipedia.org/wiki/HTML)
* CSS: [w3schools](https://www.w3schools.com/css/)
* JS: [Wikipedia](https://pt.wikipedia.org/wiki/JavaScript)
