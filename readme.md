# Teste Técnico Front-End — Vue 3 + Quasar + TypeScript

## Objetivo

Este teste tem como objetivo avaliar suas habilidades como Desenvolvedor(a) Front-End, considerando:

* Organização de código
* Componentização
* Uso de Vue 3, Quasar e TypeScript
* Consumo ou simulação de dados
* Responsividade
* Atenção à experiência do usuário
* Cuidado visual e senso estético na construção da interface
* Implementação de um fluxo simples de autenticação

## Prazo

O prazo para entrega é de **2 dias úteis** a partir do recebimento do teste.

## Cenário

Você deverá desenvolver uma interface simples para um **Painel de Gestão de Veículos**.

A aplicação deve conter um login simples e, após a autenticação, permitir visualizar uma lista de veículos, filtrar os dados, acessar detalhes e cadastrar um novo item.

O objetivo não é criar um sistema completo, mas demonstrar sua capacidade de construir uma interface funcional, organizada, responsiva e visualmente agradável.

## Autenticação

A aplicação deve conter uma tela de login com autenticação simples por e-mail e senha.

Não é necessário criar back-end. A autenticação pode ser simulada no front-end.

### Dados sugeridos para acesso

```txt
E-mail: admin@datapage.com.br
Senha: 123456
```

A tela de login deve conter:

* Campo de e-mail
* Campo de senha
* Validação de e-mail válido
* Validação de senha obrigatória
* Feedback visual para erro de login
* Feedback de carregamento ao tentar entrar
* Redirecionamento para o painel após login válido
* Proteção das rotas internas
* Logout funcional

Será considerado diferencial:

* Persistência simples da sessão no `localStorage` ou `sessionStorage`
* Redirecionamento automático caso o usuário já esteja autenticado
* Layout visualmente agradável para a tela de login

## Requisitos obrigatórios

A aplicação deve conter:

### 1. Listagem de veículos

Exibir uma lista de veículos em formato de cards ou tabela.

Cada veículo deve apresentar, no mínimo:

* Marca
* Modelo
* Ano
* Placa
* Valor
* Status
* Tipo do veículo

### 2. Filtros

A interface deve permitir filtrar os veículos por:

* Tipo: carro, moto ou caminhão
* Status: disponível, vendido ou reservado

Também deve conter uma busca por texto, permitindo pesquisar por marca ou modelo.

### 3. Detalhes do veículo

Ao clicar em um veículo, deve ser possível visualizar mais informações sobre ele em uma página, modal ou drawer.

Os detalhes devem conter:

* Marca
* Modelo
* Ano
* Placa
* Cor
* Valor
* Tipo
* Status
* Descrição curta

### 4. Cadastro simples de veículo

Criar um formulário simples para adicionar um novo veículo à listagem.

Campos obrigatórios:

* Marca
* Modelo
* Ano
* Placa
* Valor
* Tipo
* Status

O formulário deve conter:

* Validações básicas
* Feedback de sucesso
* Feedback para campos obrigatórios

### 5. Estados da interface

A aplicação deve prever:

* Estado de carregamento
* Estado vazio quando não houver resultados
* Feedback visual para ações do usuário

## Requisitos técnicos

Obrigatório utilizar:

* Vue 3
* Quasar Framework
* TypeScript
* Vue Router

Será considerado diferencial:

* Pinia ou outro gerenciador de estado
* Composables
* Máscaras em campos como placa e valor
* Organização em services
* Deploy da aplicação
* Uso de boas práticas de acessibilidade

## Dados

Não é necessário criar back-end.

Você pode utilizar:

* Dados mockados em arquivo JSON
* Dados locais em um service
* Simulação de API com Promise
* JSON Server, caso prefira

Exemplo de estrutura de veículo:

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
  description: string
}
```

## Sugestão de estrutura

```txt
src/
├─ components/
├─ layouts/
├─ pages/
├─ router/
├─ services/
├─ stores/
├─ types/
├─ utils/
```

## Avaliação

O teste será avaliado considerando:

* Clareza e organização do código
* Uso adequado de Vue 3, Quasar e TypeScript
* Componentização
* Responsividade
* Funcionamento do login e proteção de rotas
* Funcionamento dos filtros e busca
* Validações do formulário
* Tratamento de estados da interface
* Experiência do usuário
* Senso estético e cuidado visual da interface
* Simplicidade e objetividade da solução

A parte visual também será considerada na avaliação. Não esperamos uma interface extremamente elaborada, mas é importante demonstrar noção de hierarquia visual, espaçamento, alinhamento, contraste, consistência e cuidado com a apresentação dos elementos.

## Uso de ferramentas de IA

O uso de ferramentas de IA é permitido como apoio ao desenvolvimento.

Caso utilize IA, informe no README:

* Quais ferramentas utilizou
* Em quais partes do projeto a IA ajudou
* Quais decisões foram revisadas por você
* Como garantiu que compreende o código entregue

## Entrega

A entrega deve conter:

* Link do repositório
* Instruções para rodar o projeto
* Breve descrição das decisões técnicas
* Informações sobre uso de IA, caso tenha utilizado
* Link de deploy, se houver

## Observação

O objetivo deste teste não é medir a quantidade de funcionalidades, mas a qualidade da entrega.

Priorizamos uma solução simples, bem organizada, funcional, responsiva e visualmente bem resolvida.
