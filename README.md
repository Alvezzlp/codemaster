# Projeto CodeMaster Dev 💻

## O Estado Inicial

<p>Recebi o HTML e CSS prontos. O layout renderiza perfeitamente, mas
o menu mobile não abre, o formulário recarrega a página e o carrossel não se movimenta.</p>

---

## Checklist de tarefas ✅
- [✅] 1. Menu Mobile

<p> Primeiro, foram selecionados dois elementos da página: o ícone do menu e a lista de links de navegação
Depois, é criado um evento para que quando o usuário clique no ícone, o menu abra ou feche.

Quando isso acontece, o ícone muda de aparência (☰ vira ✖) e o menu aparece ou desaparece. Além disso, quando o menu está aberto, a rolagem da página é bloqueada.

O código também faz o menu fechar automaticamente quando o usuário clica em um link ou rola a página. Assim, o ícone volta ao normal e o scroll é liberado novamente. </p>

- [✅] 2. Links de navegação

<p> Quando o usuário clica em um link, o código primeiro remove o destaque de todos os links. Em seguida, adiciona o destaque apenas no link que foi clicado.

Por fim, o script adiciona um evento de clique em cada link do menu, para que esse destaque funcione sempre que o usuário selecionar uma opção da navegação. Assim, fica mais fácil visualizar qual seção do site foi escolhida. </p>

- [✅] 3. Modo Claro/Escuro

<p> O código cria uma função responsável por alternar entre o tema claro e o tema escuro do site.

Quando essa função é executada, ela adiciona ou remove a classe “light” no elemento principal da página. Essa classe normalmente é usada no CSS para mudar cores do site, como fundo, textos e elementos da interface.

Depois disso, o código verifica qual tema está ativo no momento. Se a classe “light” estiver presente, significa que o site está no modo claro; caso contrário, ele está no modo escuro.

Em seguida, o tema escolhido é salvo no navegador usando o localStorage. Isso permite que o site lembre a preferência do usuário, mesmo depois que a página for atualizada ou aberta novamente.

Por fim, quando a página carrega, o código verifica se existe um tema salvo no localStorage. Se existir, ele aplica automaticamente esse tema, mantendo o site no mesmo modo que o usuário escolheu anteriormente. </p>

- [✅] 4. Animação do Título

<p> Primeiro, o código seleciona o elemento do título da página e define o texto que será exibido (por exemplo: “CODEMASTER”). Também são criadas algumas variáveis para controlar a posição das letras e o estado da animação.

Depois, é criada uma função responsável por animar o texto do título. Essa função faz com que as letras apareçam uma por uma, simulando um efeito de digitação.

Quando todas as letras já foram exibidas, o código muda o modo da animação e começa a apagar as letras aos poucos, criando o efeito contrário.

Quando o texto é quase totalmente apagado, a animação reinicia o processo de digitação e alterna a cor do título, mudando entre a cor padrão do tema (preto ou branco) e uma cor de destaque (laranja).

Além disso, o código possui uma função que atualiza a cor do texto de acordo com o tema do site (claro ou escuro), garantindo que o título continue visível.

Por fim, quando a página é carregada, a animação do título é iniciada automaticamente.</p>

- [✅] 5. Animação da Seção Home

<p> Primeiro definimos alguns estilos iniciais para essa seção, deixando ela invisível e um pouco deslocada para baixo.

Em seguida, o código cria uma transição suave, que controla a forma como a animação vai acontecer.

Após um pequeno atraso, os estilos são alterados: a seção fica visível novamente e volta para sua posição original.

Com isso, é criado um efeito de aparecimento suave, fazendo a seção inicial surgir na tela quando a página é carregada.</p>

- [✅] 6. Animação das Seções

<p> Primeiro, o código seleciona todas as seções da página para aplicar animações quando elas aparecerem na tela.

Depois, ele define um estado inicial para cada seção, deixando todas invisíveis e configurando uma transição suave. Além disso, algumas seções recebem transformações diferentes, como aparecer de baixo para cima, diminuir de tamanho ou girar.

Em seguida, é criado um IntersectionObserver, que observa quando cada seção entra ou sai da área visível da tela enquanto o usuário rola a página.

Quando uma seção entra na tela, o código remove a transformação e deixa a opacidade em 1, fazendo com que ela apareça com animação.

Quando a seção sai da tela, ela volta ao estado inicial (invisível e transformada). Assim, quando o usuário voltar até ela, a animação acontece novamente. </p>

- [✅] 7. Botão de voltar ao topo

<p> O código seleciona o link do botão de voltar ao topo da página, que está dentro de um elemento com a classe “top”.

Depois, ele adiciona um evento de clique nesse botão.

Quando o usuário clica, o código cancela o comportamento padrão do link, que normalmente faria a página pular diretamente para outro lugar.

Em seguida, o script usa uma função do navegador para rolar a página suavemente até o topo.

Assim, quando o botão é clicado, o site volta para o início da página com uma animação suave de rolagem.</p>

- [✅] 8. Carrossel de Projetos

<p> Primeiro, o código seleciona os elementos do carrossel, como o container dos slides, cada slide individual e os botões de avançar e voltar.

Depois, ele cria uma variável para controlar qual slide está sendo exibido no momento e outra para controlar a troca automática dos slides.

Em seguida, é criada uma função responsável por mostrar o slide atual. Para isso, o código esconde todos os slides e depois exibe apenas o slide correspondente ao índice atual.

O script também cria duas funções para navegar entre os slides: uma para ir para o próximo slide e outra para voltar ao anterior. Quando o usuário usa os botões, o slide muda e o tempo da troca automática é reiniciado.

Além disso, o código cria um sistema de troca automática, que faz o carrossel avançar para o próximo slide a cada 5 segundos.

Por fim, o script inicia o carrossel quando a página carrega e adiciona um comportamento extra: quando o usuário passa o mouse sobre o carrossel, a troca automática é pausada, e quando o mouse sai, ela volta a funcionar. </p>

- [✅] 9. Formulário de Contato

<p> Primeiro, o código seleciona o formulário de contato e o elemento onde será exibida a mensagem de agradecimento.

Depois, ele adiciona um evento de envio ao formulário. Isso significa que quando o usuário clicar no botão de enviar, uma função será executada.

Quando o formulário é enviado, o código impede o comportamento padrão da página, que normalmente faria a página recarregar imediatamente. Em seguida, ele mostra a mensagem de agradecimento para o usuário.

Depois disso, o script coleta todos os dados preenchidos no formulário e os envia para o endereço definido no atributo action do formulário usando a Fetch API.

Se o envio for realizado com sucesso, o código aguarda 2 segundos e recarrega a página, limpando o formulário. Caso ocorra algum erro no envio ou na conexão, uma mensagem de alerta é exibida informando o problema. </p>

- [ ] 10. Seção Sobre Mim
 
