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

- [ ] 4. Animação do Título

- [ ] 5. Animação da Seção Home

- [ ] 6. Animação das Seções

- [ ] 7. Botão de voltar ao topo

- [ ] 8. Carrossel de Projetos

- [ ] 9. Formulário de Contato

- [ ] 10. Seção Sobre Mim
 
