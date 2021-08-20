# DOM-estudo

# Projeto de piano virtual para praticar a utilização do DOM.

# Comandos

## Gerais

- console.dir(document)
    - Exibe uma lista interativa das propriedades do objeto JavaScript especificado.
- document.URL/title/head/body/links/forms/images/...
    - Lista todos os elementos da propriedade específicada.

## Buscando e selecionando elementos

- .querySelector('elemento')
    - Seleciona o primeiro elemento daquele tipo no documento.
- .querySelectorAll('elemento')
    - Seleciona todos os elementos com aquela propriedade no documento.

## Manipulando conteúdo

- x.textContent / x.textContent = 'algo'
    - O primeiro pega o conteúdo e o segundo aplica o conteudo. Mostra todo o texto, até o oculto.
- .innerText
    - Retorna o texto puro apenas.
- .innerHTML
    - Retorna o texto e as tags aplicadas do elemento. - não recomendado para inserir texto puro.

[https://www.mundojs.com.br/2019/07/18/diferencas-entre-innerhtml-innertext-e-textcontent/](https://www.mundojs.com.br/2019/07/18/diferencas-entre-innerhtml-innertext-e-textcontent/)

## Alterando Estilo

- .style.algumaPropriedade( ex: backgroundColor)
    - Deve ser camelCase e aceita todas as propriedades do CSS
- .classList
    - Mostra as classes de um elemento
    - .add('propriedade') - adiciona a class propriedade no elemento
    - .remove('propriedade') - remove a class propriedade no elemento
    - .toggle('propriedade') - adiciona ou remove a class do elemento dependendo se ja tem ou não.

## Navegando pelos elementos

 - .parentNode
     - Mostra/seleciona o elemento pai
 - .children
     - Mostra/seleciona o elemento filho
 - .childElementCount
     - Conta quantos filhos o elemento tem
 - .firstChild
     - Mostra/seleciona o primeiro filho declarado do elemento
 - .lastChild
     - Mostra/seleciona o último filho declarado do elemento
 - .remove('elemento')
     - Remove um elemento
 - .nextSibling
    - Monstra/seleciona o próximo irmão do elemento
- .previousSibling
    - Monstra/seleciona o irmão anterior do elemento

## Criando elementos

- .createElemento( )
    - Cria novos elementos a serem adicionados na estrutura do HTML. Funciona como um commit do git, ou seja, para ser adicionado na estrutra é necessário fazer um push (.append())

## Trabalhando com propriedades dos elementos

- .setAttribute("nomeAtributo", "valorAtributo")
    - Adiciona um atributo e seu valor a uma variável
    - Ex.: h1.setAttribute("class", "teste")
- .getAttribute
    - retorna um atributo de uma variável
- .removeAttribute
    - remove um atributo de uma variável

## Eventos

- .addEventListener('tipo de escuta", function (evento) { lógica do evento}
    - escuta a execução de alguma ação dentro do html e executa uma função
