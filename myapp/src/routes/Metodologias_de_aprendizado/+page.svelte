<script>
    import Header from "../../lib/components/Header.svelte";
    import Button from "../../lib/components/Button.svelte";

</script>
<Header text={"Metodologia de Aprendizagem"}></Header>

<!-- Introdução -->
<div class="text-white p-4 text-justify bg-violet-500/50 mb-4 rounded-2xl">
    <div class="">
        <h2 class="text-4xl mb-4">
            Introdução
        </h2>

        <p>
            As metodologias de ensino permeam o trabalho de todo o educador e elas podem influenciar direta ou indiretamente a forma que o mesmo da aula. Com isso, dentro do conteúdo aprendido podemos ter contatos com algumas metodologias de ensino: como a tradicional e construtivista, que buscam engajar com o aluno de formas diferentes, principalmente através de estratégias de aprendizagem ativa ou passiva.
        </p>
    </div>

    <!-- Enunciado e alternativas -->
    <div class="my-4">
        <h2 class="text-2xl mb-4">
            Pergunta
        </h2>
        <p class="mb-4">Qual alternativa representa a aprendizagem baseada em problemas e uma atividade desenvolvendo pensamento computacional?</p>
        <ul class="list-[lower-latin] px-6 space-y-4">
            <li>
                O professor expõe todo o conteúdo durante o período da aula, transmitindo todo o conhecimento que ele possua para os alunos através dessa exposição, além disso, ele abre espaço para retirar as possiveis dúvidas que os alunos tenhas durante esse tempo. Como atividade, o professo faz um teste, presencial, sem consulta e avaliativo para entender quanto do conteúdo foi absorvido pelos alunos.
            </li>
            <li>
                O professor disponibliza textos, vídeos e outros conteúdo antes da aula, durante a sua aula ele realiza debates e discussões sobre o conteúdo previamente apresentado, além de responder a s dúvidas que surgiram durante o estudo prévio dos alunos. Durante a aula, ele propõe um quiz online que rankea os alunos através da através da velocidade que os alunos respondem a questão e a corretude da resposta.
            </li>
            <li>
                Metodologia que oferece um problema real para ensinar um tema com os alunos, apartir disso realiza atividades guiadas com o intuito de ensinar os alunos base do conteúdo para resolver o problema e promover discussões na sala para pensar sobre possiveis soluções. Para a atividade o professor propõe um problema através de uma pergunta e faz com que os alunos se dividam em grupos menores para discutir sobre o que os alunos pensam do problema, o que eles descobriram sobre, no caso podem ir pesquisar, e quais soluções eles pensaram. Ao fim, cada grupo elege um representante e essa pessoa trás os pontos do grupo.
    
            </li>

            <li>
                O professor explica um conteúdo sobre insetos e libera os alunos para que eles vejam alguns insetos, questionem sobre o professor se o que encontraram é um inseto e pesquisam mais sobre insetos. Como ativida, o professor faz com que os alunos documentem e montem uma mini enciclopédia com os insetos encontrados. 
            </li>

            <li>
                Metodologia que oferece um problema real para ensinar um tema com os alunos, apartir disso realiza atividades guiadas com o intuito de ensinar os alunos base do conteúdo para resolver o problema e promover discussões na sala para pensar sobre possiveis soluções. A atividade seria um projeto desenvolvido ao longo da matéria, onde são apresentado um ploblema e com base nisso eles elaboram uma ferramenta pra resolver o determinado problema, eles projetam, abstraindo partes de modelos ja construindos e aprende a construir os próprios, vão decompando o projeto em partes para melhor realizar os calculos e montar as peças e por fim, ele monta um fluxo para a montagem do equipamento e que pode ser escalável e também um roteiro de instruções como a peça funciona.
            </li>
        </ul>
    </div>

    <!-- Resposta -->
    <div>
        <h3 class="text-xl font-bold mb-4">Resposta:</h3>
        <ul class="px-6 list-[lower-latin] space-y-4">
            <li>
                <span class="text-red-600 uppercase font-bold">incorreta</span>, pois a metodologia de ensino é a tradicional e a sua atividade não envolve PC porque é apenas uma prova.<a class="text-orange-700"  href="https://andersongarrote.itch.io/garibot">link</a>
            </li>
            <li>
                <span class="text-red-600 uppercase font-bold">incorreta</span>, pois apesar de ser uma metodologia ativa, o método utilizado é sala de aula invertida. E apesar que pode ser argumentado o uso das habilidades do Pensamento computacional, a atividade é apenas uma uma forma de aprendizado baseado em jogos usando a tecnologia educacional <a class="text-orange-700" href="https://kahoot.it/">kahoot</a>.
            </li>
            
            <li>
                <span class="text-red-600 uppercase font-bold">incorreta</span>, apresenta metodologia baseada em problemas e atividade tem total relação com aprendizagem baseada em problemas, porém não trata do pensamento computacional e sim apenas um debate comum. Atividade foi retirada desse <a class="text-orange-700" href="https://www.youtube.com/watch?v=LwznGzpR0iQ">vídeo</a>.  
            </li>
            <li>
                <span class="text-red-600 uppercase font-bold">incorreta</span>, trata de uma forma de aprendizado ativa, mas sua base é metodologia construtivista pois foca na interação entre pessoas, interação com outros seres vivos e com tudo o que esta no meio ambiente, ou seja, interação do sujeito que conhece com o objeto do seu conhecimento. Isso envolve ação e reflexão, teoria e prática.<a class="text-orange-700" href="#id1">¹</a> Além disso, a própria construção de uma unidade de ensino reflete essa abordagem construtivista mencionada. Você consegue acessar o link dessa atividade clicando <a class="text-orange-700" href="https://tede2.pucrs.br/tede2/bitstream/tede/3335/1/347014.pdf">aqui</a>. 
            </li>
            <li>
                <span class="text-green-500 uppercase font-bold">correta</span>, , trata da metodologia baseada em problemas e atividade tratada é de uma oficina maker onde os pesquisadores fizeram a análise de como as habilidades do pensamento computacional são utilizados no contexto dessas oficinas. Informações detalhadas podem ser encontrados nesse <a class="text-orange-700" href="https://sol.sbc.org.br/index.php/wie/article/view/16448/16289">link</a>.
            </li>
        </ul>
    </div>
    
    <!--Referencias -->
    <div>
        <p>Referências: </p>
        <ul class="list-decimal px-8">
            <li><a  id="id1" class="text-orange-700" href="https://books.google.com.br/books/about/Construtivismo_e_ensino_de_ci%C3%AAncias_ref.html?id=r-WM04D8mJkC&redir_esc=y">BORGES, R. M. R. Repensando o Ensino de Ciências. In: MORAES, R. (Org.). Construtivismo e ensino de ciências: reflexões epistemológicas e metodológicas. Porto Alegre: EDIPUCRS, 2000</a></li>
        </ul>
    </div>

    <p class="font-bold mb-4">Ideia originalmente criada por: Luís Felipe Dobner Henriques</p>
    <Button/>
</div>
