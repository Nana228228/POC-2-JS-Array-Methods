# POC-2-JS-Array-Methods


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


<!--índice-->
<p align="center">
  <a href="#descricao">Descrição</a> •
  <a href="#conceitos">Conceitos</a> •
  <a href="sort">Sort </a> •
  <a href="map">Map</a> •
  <a href="reduce">Reduce </a> •
  <a href="filter">Filter</a> •
  <a href="spread">Spread</a> •
  <a href="uso">Como usar?</a>
  <a href="autores">Autores</a>
</p>

<h2>Descrição do projeto</h2>
<p id="descricao"> Bem-vindo ao repositório JavaScript Array Methods! 🎉 Este projeto é dedicado a ensinar conceitos básicos de JavaScript abordando métodos para a manipulação de arrays dessa linguagem. O objetivo é oferecer à comunidade um recurso educativo gratuito e acessível para quem deseja aprender ou aprimorar suas habilidades em cinco métodos aplicados em arrays: sort, map, reduce, filter, e spread
</p>

<h2>Conceitos</h2>
Se deseja acompanhar as descrições usadas ao explicar o funcionamentos dos métodos selecionados mas ainda não domina alguns conceitos da linguagem JavaScript ou da programação, aqui há uma breve descrição.
<h3 id="est">Estrutura de dados</h2>
Estruturas de dados são maneiras organizadas de armazenar e manipular dados em um programa, permitindo que as operações necessárias sejam realizadas de forma eficiente. Elas oferecem formas de organizar dados para que possam ser acessados e manipulados de acordo com a necessidade. Dependendo da tarefa que o contexto demanda, uma estrutuda de dados é mais adequada e eficiente que a outra. Algumas conhecidas na proframação são: como arrays, listas, pilhas, filas, árvores e gráficos. Cada uma delas serve a diferentes propósitos e possui características específicas, como o tempo de acesso, inserção ou remoção de elementos. No JavaScript, as mais usadas são arrays e objetos. 



<h3 id="arrays"> Arrays</h2>

<p>
  Um array em JavaScript é uma estrutura de dados que permite armazenar uma coleção de elementos, como números, strings, objetos ou até outros arrays, em uma única variável. Cada elemento no array possui um índice, começando do zero, o que facilita a localização e manipulação dos itens.
<h3>Funcionamento</h3>
- São definidos usando colchetes ([]), com os elementos separados por vírgulas.<br>
- Podem conter diferentes tipos de dados ao mesmo tempo, ou seja, são heterogêneos.<br>
- Em JavaScript, os arrays são interpretados como objétos incluidos por padrão na linguagem, já que possuem propriedades e métodos próprios e previamente definidos. 
</p>
  
<h3 id="metodos"> Métodos </h2>
Métodos são funções associadas a objetos, ou seja, eles representam comportamentos que um objeto pode executar. Um método é invocado usando a sintaxe de ponto, e ele pode realizar operações como modificação, transformação ou consulta do estado do objeto. Ensinaremos métodos proprios para a manipulação dos arays, cada um acompanhado de exemplos simples para demonstrar como podem ser aplicados no dia a dia de desenvolvedores JavaScript para a resolução de problemas.


<h3>📚 Métodos Abordados</h3>
Sort - Retorna os elementos de um array em ordem alfabética. <br>
Map - Cria um novo array com os resultados da chamada de uma função para cada elemento. <br>
Reduce - Reduz um array a um único valor, executando uma função para cada elemento. <br>
Filter - Cria um novo array com todos os elementos que passam em um teste. <br>
Spread - Desconstrói arrays (ou objetos) em elementos individuais. <br>

Usaremos o array numeros = [44, 14, 200, 9, 18]

<h2 id="">Sort</h2>
O comportamento padrão do sort() pode não ser intuitivo, especialmente quando se trata de números, pois ordena os elementos como strings (texto), e não como números. Isso significa que ele compara os elementos com base na ordem lexicográfica, ou seja, na comparação de caracteres Unicode. 

 ```javascript
const arr = [1, 30, 4, 21, 100000];
arr.sort();
console.log(arr); // [1, 100000, 21, 30, 4]
 ```
<img src="imgs cod/sort.png">
 
No entanto, é possível personalizar o modo de ordenação com uma função de comparação (callback) para o sort().

 ```javascript
const numeros = [44, 14, 200, 9, 18];
// Usando sort em ordem crescente
const crescente = [...numeros].sort((a, b) => a - b);
// Em ordem decrescente
const decrescente = [...numeros].sort((a, b) => b - a); 
 ```

<h2 id="">Map</h2>
A função map() cria um novo array aplicando uma função a cada elemento do array original. Não modifica o array original.

```
const numeros = [44, 14, 200, 9, 18];
// Usando map para multiplicar cada número por 2
const multiplicados = numeros.map(num => num * 2);
// Usando map para transformar cada número em string
const comoStrings = numeros.map(num => num.toString());
```
<img src="imgs cod/map.png">

<h2 id="">Reduce</h2>
A função reduce() executa uma função redutora (callback) em cada elemento do array, resultando em um único valor. Pode ser usada para somar, concatenar, ou transformar arrays em outros tipos de dados.


 ```javascript
 const numerosReduce = [1, 2, 3, 4, 5];
 const soma = numerosReduce.reduce((acumulador, atual) => acumulador + atual, 0);
 ```
<img src="imgs cod/reduce.png">

<h2 id="">Filter</h2>
A função filter() cria um novo array com todos os elementos que passam em um teste implementado pela função fornecida.

```javascript
const idades = [15, 25, 35, 45, 55];
const maioresDeIdade = idades.filter(idade => idade >= 18);

 ```
<img src="imgs cod/filter.png">
<h2 id="">Spread</h2>
O operador spread é usado para expandir elementos de um array ou propriedades de um objeto. Ele pode ser utilizado para copiar, combinar arrays, ou passar elementos individuais.

```javascript
const numeros1 = [1, 2, 3];
        const resultadonumeros = [...numeros1, 8, 23, 72];
        console.log(resultadonumeros); // [1, 2, 3, 4, 5]
 ```
<img src="imgs cod/spread.png">

<h2 id="uso">🛠 Como Usar </h2>

Este repositório consiste em pequenos trechos de código que exploram apenas um conceito por vez. Você pode clonar o repositório e executar os exemplos no seu ambiente local.

Clonando o Repositório bash Copiar código git clone https://github.com/seu-usuario/js-array-methods.git cd js-array-methods Executando os Exemplos Você pode abrir cada arquivo .js individualmente em seu editor de código favorito e testar os métodos diretamente em seu console JavaScript ou ambiente Node.js.

<h2 id="autores"> Autores </h2>

<a href="">
 <img style="border-radius: 50%;" src="" width="100px;" alt=""/>
 <br />
<h3>Naomi Arakaki</h3>
<img src="imgs cod/E919DE67-90A4-433E-93BA-9FBC40BB2CF1.jpeg">


[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/naomi-suguimoto-57436b290/)](https://www.linkedin.com/in/naomi-suguimoto-57436b290)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:arakakinaomi228@gmail.com)](mailto:arakakinaomi228@gmail.com)


<a href="">
 <br />
<h3>Gabriel Aboboreira</h3>
<img style="border-radius: 50%;" width="350px;" height= "500px;"  alt="" src="imgs cod/2023-05-26at08.21.20.jpeg">


[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriel-aboboreira/)](https://www.linkedin.com/in/gabriel-aboboreira/)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:masterkillbr007@gmail.com)](mailto:masterkillbr007@gmail.com)

<a href="">
 <br />
<h3>Ana Julia Blande</h3>
<img style="border-radius: 50%;" width="350px;" height= "500px;"  alt="" src="ana.jpeg">


[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/ana-julia-blande-silva-348612286/)](https://www.linkedin.com/in/ana-julia-blande-silva-348612286/)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:anajblande04@gmail.com)](mailto:anajblande04@gmail.com)

