# Front-End Challenge — Vue 3 + Quasar + TypeScript

## Objetivo

Este desafio tem como objetivo avaliar suas habilidades como Desenvolvedor(a) Front-End, com foco em:

* Arquitetura de projeto front-end
* Organização e clareza de código
* Componentização
* Integração com dados/API
* Experiência do usuário
* Responsividade
* Tratamento de erros, loading e estados vazios
* Validações de formulário
* Boas práticas com Vue 3, Quasar e TypeScript

## Cenário

Você deverá desenvolver um pequeno **Sistema de Gestão de Veículos**, com autenticação simulada e funcionalidades de cadastro, listagem, edição e exclusão de veículos.

A aplicação deve demonstrar domínio técnico no front-end, organização visual e capacidade de transformar requisitos em uma interface funcional, responsiva e bem estruturada.

## Autenticação

Implemente uma tela de login com:

* Campo de e-mail
* Campo de senha
* Validação de e-mail válido
* Validação de senha obrigatória
* Feedback de erro amigável
* Simulação de autenticação
* Controle de sessão no front-end
* Proteção de rotas privadas
* Logout funcional

### Dados sugeridos para login

Você pode utilizar dados fixos para simular o acesso:

```txt
E-mail: admin@datapage.com.br
Senha: 123456
```

### Diferenciais

* Persistência de sessão
* Tratamento de sessão expirada
* Interceptors para requisições
* Feedback visual durante o login

## CRUD de Veículos

A aplicação deve permitir:

### Criar veículo

Campos sugeridos:

* Marca
* Modelo
* Ano
* Placa
* Cor
* Valor
* Tipo: carro, moto ou caminhão
* Status: disponível, vendido ou reservado

O formulário deve conter:

* Validações obrigatórias
* Máscara para placa
* Máscara monetária para valor
* Feedback de sucesso e erro
* Tratamento para campos inválidos

### Listar veículos

A listagem deve conter:

* Tabela ou cards
* Busca por marca ou modelo
* Filtro por tipo
* Filtro por status
* Paginação ou carregamento organizado dos dados
* Estado vazio
* Estado de loading
* Tratamento de erro

### Editar veículo

A edição deve conter:

* Formulário pré-preenchido
* Validações
* Feedback de sucesso e erro
* Atualização dos dados na listagem

### Excluir veículo

A exclusão deve conter:

* Confirmação antes de excluir
* Feedback visual após exclusão
* Atualização da listagem

## Requisitos técnicos

Obrigatório utilizar:

* Vue 3
* Quasar Framework
* TypeScript
* Vue Router
* Pinia ou outro gerenciador de estado

Esperamos encontrar:

* Componentização adequada
* Separação de responsabilidades
* Código limpo e organizado
* Reutilização de componentes
* Responsividade para mobile e desktop
* Uso adequado dos componentes do Quasar
* Validações no formulário
* Estados visuais de loading, erro, sucesso e vazio
* Organização de services para consumo de dados
* Tipagem adequada com TypeScript

## Dados e API

Como este é um desafio Front-End, você não precisa desenvolver um back-end.

Você pode escolher uma das opções abaixo:

### Opção 1 — API mockada

Utilizar dados locais em JSON, simulando o retorno de uma API.

### Opção 2 — JSON Server

Criar uma API fake utilizando JSON Server ou ferramenta semelhante.

### Opção 3 — Serviço simulado

Criar uma camada de service com Promises, simulando chamadas assíncronas, loading e erros.

Exemplo de entidade:

```ts
export interface Vehicle {
  id: number
  brand: string
  model: string
  year: number
  plate: string
  color: string
  price: number
  type: 'carro' | 'moto' | 'caminhao'
  status: 'disponivel' | 'vendido' | 'reservado'
}
```

## Estrutura sugerida do projeto

```txt
src/
├─ assets/
├─ components/
├─ layouts/
├─ pages/
├─ router/
├─ services/
├─ stores/
├─ types/
├─ utils/
```

## Diferenciais

Não são obrigatórios, mas serão valorizados:

* Testes automatizados
* Uso de composables
* Uso de Vite
* Uso de Storybook
* Boas práticas de acessibilidade
* Cuidados com performance
* Design responsivo bem resolvido
* Layout visualmente agradável
* Documentação clara das decisões técnicas
* Deploy da aplicação
* Uso consciente de ferramentas de IA para apoio ao desenvolvimento

## Uso de ferramentas de IA

O uso de ferramentas de IA é permitido como apoio ao desenvolvimento.

Caso utilize IA, informe no README:

* Quais ferramentas utilizou
* Em quais partes do projeto a IA ajudou
* Quais decisões foram revisadas por você
* Quais cuidados tomou para garantir qualidade, segurança e entendimento do código

O objetivo é avaliar sua capacidade técnica, organização, tomada de decisão e domínio sobre a solução entregue.

## Entrega

No repositório, inclua:

* Código fonte completo
* README com instruções para rodar o projeto
* Tecnologias utilizadas
* Decisões técnicas
* Informações sobre uso de IA, caso tenha utilizado
* Link de deploy, se houver

## O que será avaliado

* Organização do projeto
* Clareza e qualidade do código
* Uso adequado de Vue 3, Quasar e TypeScript
* Componentização
* Responsividade
* Experiência do usuário
* Tratamento de estados da interface
* Validações
* Integração ou simulação de dados
* Capacidade de resolver problemas com simplicidade e qualidade

## Observação importante

O objetivo não é criar uma aplicação extremamente complexa, mas demonstrar:

* Organização
* Clareza
* Estrutura
* Domínio técnico
* Boas práticas
* Capacidade de entregar uma interface funcional e bem construída

Boa sorte!
