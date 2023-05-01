REACT === uma biblioteca javaScript para criar interfaces de usuário
é SPA 

---------------------------
extenção === jsx
todos os componentes devem começar com a letr maiuscula
sempre deve ter um return para mostrar a interface 

Um componente devolve sómente um elemento
mais dentro de um elemento pode ter mais elemento === exemplo ums div pu fragmento

============
CSS =>
Pré Processadores => quer dizer que você não vai utilizar esse arquivo em produção. Na verdade, ele será processado para utilização final no CSS da sua aplicação
CSS-in-Js => fazem  muito sentido, porque aproveitam métodos atuais de componentes perfirmáticos a prova de colisão 

 e tudo isso é extremamente automatizado

definir valores para componente 

=== se é texto ""
=== se é numeros {}

===========================================================
Map == tem como objetivo percorrer cada item dentro de uma lista, uma estrutura de repetição para cada item de existe ele fara uma determinada coisa


DIFERENÇA ENTRE FOREACH E MAP ------ o map retorna algo mais foreach não, map manipula e retorna um novo
-------------------------------------------

Bivlioteca AXIOS = CONSUMIR REQUISIÇÕES DO http

npm install axios

--------------------------------------------------

ESTADOS ===> permite que possamos amazenar dados de forma temporaria

Por que não utilizar variaveis comuns ?
= "../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (20).png
- varias comuns não percitem na segunda vez.( quando o valor sempre seja exibido ou queremos ultilizar o valor aualizado)

Atualiza um componente com novos dados "../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (21).png"
- salvar dados entre redenrizações
- acionar a re-rederização
=== quando indetidfica que um componente manteve seu estado e suas propriedades alteradas então ele aciona sua renderização para os componentes que tiveram alterção.

useEstate ../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (22).png

fornece duas coisas;
1 - reter dados 
2 - acionar rederização

function () {
    const [nomeDoEstado, funçãoQueAtualizaOEstado] = useState("")===> valor inicial
}

RECAPITULAR
1 - use um variavel de estado quando um componente precisar "lemnbrar" alguma informção entre renderização.

2 - as variaveis de estado são declaradas utilizando o useState.

3 - o useState retorna um par de valores: o estado atual e a função para atualiza-lo.

4 - o estado é privado para o componente. se voc~e renderizar em dois lugares, cada cópia terá seu proprio estado.

Anotação com a exibição protica 
 -  variaveis come não tem poder para iniciar uma renderização.

 - o estado não é alterado ele é substituido.

 - preserva o valor entre rederização , mas se recarregaro estado volta ao inicial.

 - não atuliza no mesmo instante.

 - projeto utilizado como exemplo ../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (24).png

-----------------------------------------------------------------------------------

LOCAL STORAGE ===> permite armazenar informações no navegador do usuario.

Voce pode garantir que mesmo que o usuario feche o navegador as informações continuaram.

forma de fazer ;../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (26).png

setItem ===> função parar amarzenar algo no navegador.

---------------------------------------------------------------------------------------------------

useEffect ===> voce diz ao React que o componente precisa fazer algo depois da renderização. Isto é depois que realizar as atualização do DOM.

colocando ele dentro do componente conseguimos usar os estados dentro co componente.

forma de fazer ;../../../stage08/estudo-08/apinew/image-estudo/Captura de Tela (27).png

primeiro parte ==> corpo
segundo parte ===> dependencias

Anotação com a exibição pratica 
 - primeiro ele recebe a logica de execucão.
 - no array ele recebeb as dependencias (estado).
 - clocando dependencias;
                        -  quando o estado muda o useEffect tambem eé executado.
                        - ele será renderizado.

RECAPITULANDO 
1 - O useEffect é executado após nosso componente ser renderizado.
2 - Dentro delel podemos colocar uma logica toda vez que nosso componente ser renderizado.
3 - Quando a depencia estiver vazia o useEffect ativado somente uma vez, após nosso componente ser renderizado. Caso contrario ele sera ativado toda vez que houver mudança nos estados.

---------------------------------------------------------------------------------------------------------------------------------------

RENDER

Explicaçoes em imagens na pasta "../../../stage08/estudo-08/apinew/image-estudo/render"

Render ===> 
Antes dos componentes serem exibidos na tela eles devem ser renderizados pelo React.
é o processo de desenhar/exibir/construir/vizualizar o componente na tela.

O Objetivo do React = construir interfaces.

ILUSTRAÇÃO
 - um restaurante é a plicação,
 - os componentes são os cozinheiros,
 - os ingredientes são as propriedades,
 - resct é o garçom,
 - 3 etapas
            - acionar
                    - iniciar
                    - atualizar
                                - re-render 
                                            - atualização do estado
                                            - gatilho
                                            - renderizar
                                                        - comfirmação
                                                        - alterar somente aqueles que tiveram alteração.
            - renderizar
            - comprometer-se
 - cliente ===> onde o componnet vai ser entregue




