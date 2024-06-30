# Jampa Ruby Website

O website foi desenvolvido utilizando o Jekyll e o tema  [Kasper](https://github.com/rosario/kasper) em sua base.

## Instalação

- Faça fork desse repositório
- Clone o seu repositório fork para a sua maquina
- Instale o Jekyll com o comando `gem install jekyll`
- E a dependencia de paginação com o comando `gem install jekyll-paginate`
## Rodando a aplicação

Utilize o comando `jekyll serve` para iniciar localmente a aplicação.

## Como agendar novos eventos?

Para agendar novo eventos é necessário cumprir algumas etapas:

1. Criar um novo post

2. Alterar detalhes sobre evento na pagina Home

3. É necessario criar o post para centralizar todas as informações sobre o novo evento, é fácil fazer essa criação seguindo o modelo do arquivo `Post-modelo`, no entanto, as informações necessárias são: 
	- Agenda do evento: hórarios separados com suas  devidas descrições e palestrantes.
	- Palestrantes: Nome e breve descrição de todos os palestrantes
	- Local e hórario
	- Inscrições: Breve descrição contendo informações sobre como se inscrever no evento.

4. Quando o novo post for criado, é necessario atualizar a propriedade `isEvent` no arquivo `index.html` para `true` e também atualizar a propriedade `next_event` com a nova data e horário, esse passo vai atualizar o banner principal da página.

## Quando não tiver nenhum evento agendado o que fazer?

Nesse caso, para não ficar uma mensagem desatualizada para o usuário é necessário trocar a propriedade `isEvent` do arquivo `index.html` para false. Essa alteração vai apresentar uma mensagem mais amigável informando para o usuário que ainda não temos nenhum evento agendado no momento.