# Teste prático

## Introdução

Parabéns, temos um pequeno teste prático para você botar a mão na massa. Os objetivos do teste serão descritos abaixo, assim como uma breve descrição do seu conteúdo.

### Informações preliminares

A aplicação deste repositório utiliza javascript, HTML e CSS para mostrar uma simples interface que simula um mapa e alguns pontos. Os arquivos possuem comentários úteis para que você entenda o código-fonte e suas funcionalidades. Se você tiver dúvidas que os comentários e estrutura do código-fonte não puderem elucidar, _não hesite em perguntar!_

Para que os módulos e componentes funcionem bem, você precisa de um ambiente `node.js` com `npm`. Instale as dependências do projeto contidas no arquivo package.json e use o comando `npm start` para servir os arquivos do projeto via http.

### Iniciando os trabalhos

Para começar a trabalhar no projeto, utilize o zip do respositório enviado por email, em seguida, crie e configure um repositório **no seu GitHub**. Para entregá-lo, suba suas modificações e siga as instruções da seção _Entregando o seu Teste_.

### Objetivo 1 OK

Se você conseguiu acessar a aplicação em [http://127.0.0.1:8081/](http://127.0.0.1:8081/), então o primeiro objetivo já está cumprido: **configuração do ambiente**. Se algo deu errado, confira as dependências instaladas e as permissões de acesso à porta 8081. _(não tem problema trocar a porta do servidor http, se você souber como e se for necessário)_

### Objetivo 2 OK

A aplicação utiliza uma classe chamada `Controller` para controlar a intercace. Nessa classe constam os métodos repsonsáveis por inicializar o SVG retangular na tela e desenhar a _bounding box_ do mapa. A classe `Map` corresponde a um mapa hipotético com algumas características e funções importantes. As duas classes podem ser encontradas no arquivo `models.js`. A documentação contida diretamente nos arquivos descrevem em detalhes as partes de cada uma das classes. _Dê uma lida._

Para que a aplicação funcione corretamente, **você precisa exibir todos os pontos contidos no arquivo `data.json` na tela**. A função `Map.getPoints()` pode carregá-los e a função `Controller.drawPoint()` está preparada para desenhar um ponto na tela. Escreva uma função `renderPoints()` na classe Map para resolver esse objetivo.

### Objetivo 3 OK

Agora que temos vários pontos sendo desenhados na tela, você precisa implementar os filtros correspondentes aos botões na tela. Os filtros são:

1. `Mostrar todos` - Exibir todos os pontos na tela;
2. `Mostrar pontos no mapa` - Exibir apenas os pontos contidos no mapa (representado pelo polígono colorido);
3. `Mostrar apenas pontos fora do mapa` - Exibir apenas os pontos que estão fora.

O método `addEvents()` já interliga uma função de clique para cada botão, e cada função já possui algumas linhas de _javascript_ para marcar os botões clicados como selecionados. Podem existir outros métodos úteis para resolver este objetivo que já estejam implementados.

Seu objetivo é completar as funções de clique para que executem os filtros corretamente. Fique a vontade para criar tantas funções e atributos quanto forem necessários para chegar ao objetivo. Lembre-se de manter a consistência dos dados nas classes conforme os manipula!

### Objetivo 4 OK

Como bem sabemos, um mesmo problema pode ser resolvido de diversas formas diferentes. Por isso, o quarto e último objetivo é **criar um arquivo `REPORT.md` na raiz do projeto e escrever brevemente qual foi a linha de raciocínio que você seguiu para resolver o Objetivo 3**.
