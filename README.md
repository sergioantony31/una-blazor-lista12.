# una-blazor-lista12.

# 🌍 EcoMonitor

## 👤 GRUPO #3
**Nome:** Lucas Gonçalves -  RA: 32617617 
**Curso:** (Ciência da computação)

**Nome:** Sergio Antonio - RA: 326128163 
**Curso:** (Analise e Desenvolvimento de Sistemas) 

**Nome:** Paulo André Lima Patrício – RA: 326128523
**Curso:** (Analise e Desenvolvimento de Sistemas) 

**Nome:** Miguel Oliveira Silva – RA: 326128330 
**Curso:** (Analise e Desenvolvimento de Sistemas) 

**Nome:**Arthur Carvalho Oliveira – RA: 32611916 
**Curso:** (Analise e Desenvolvimento de Sistemas) 

---

## 🎯 Descrição do Projeto
Dar continuidade ao processo da atividade elaborada anteriormente proposta pelo professor Daniel com o nome : " ONG "ReCiclo" ". 

O EcoMonitor é uma aplicação desenvolvida em Blazor Interactive Server com o objetivo de incentivar práticas sustentáveis através de um sistema de gamificação.

O usuário pode registrar ações ambientais, como reciclagem, plantio de árvores e descarte correto de eletrônicos, acumulando pontos e acompanhando seu progresso em tempo real.

---

## 🧠 Heurísticas de Nielsen Aplicadas

### 1. Visibilidade do Status do Sistema
O sistema mantém o usuário constantemente informado sobre seu progresso por meio da atualização imediata do contador de pontos após cada interação. Isso garante transparência e reforça a sensação de controle.

---

### 2. Feedback Imediato
Cada ação realizada pelo usuário (clique no botão) gera uma resposta instantânea do sistema, como:
- Incremento do total acumulado
- Mudança visual no botão
- Exibição de mensagem de conquista

Esse retorno imediato melhora a experiência e engajamento do usuário.

---

### 3. Consistência e Padrões
Os componentes seguem um padrão visual consistente:
- Estrutura de layout semelhante entre os cards
- Uso padronizado de cores (azul para padrão, verde para sucesso/meta)
- Botões com comportamento uniforme

Isso facilita o aprendizado e uso da interface.

---

### 4. Reconhecimento em vez de Memorização
O usuário não precisa lembrar valores ou regras, pois todas as informações relevantes estão visíveis na tela:
- Pontos por ação
- Total acumulado
- Status da meta

Isso reduz a carga cognitiva.

---

### 5. Controle e Liberdade do Usuário
O usuário pode interagir livremente com qualquer uma das ações disponíveis, sem restrições de ordem ou sequência, podendo escolher quais atividades registrar a qualquer momento.

---

### 6. Estética e Design Minimalista
A interface apresenta apenas informações essenciais, evitando poluição visual. O uso de cards simples, cores suaves e espaçamento adequado melhora a legibilidade e a experiência geral.

---

### 7. Prevenção de Erros
O sistema limita a interação a ações válidas (botões específicos), evitando entradas incorretas ou comportamentos inesperados.

---

### 8. Flexibilidade e Eficiência de Uso
O componente reutilizável permite rápida interação com múltiplas ações ambientais, tornando o sistema eficiente tanto para novos usuários quanto para usuários frequentes.


## ▶️ Guia de Execução

### 📌 Pré-requisitos
- .NET SDK instalado (versão 8 ou superior)

### 🚀 Passos para rodar o projeto

1. Abra o terminal na pasta do projeto
2. Execute o comando:

```bash
dotnet run
3. Acesse no navegador:
https://localhost:xxxx/

_______________________________________________________________________________________________________________

Explicação Técnica

O componente EcoStatus foi desenvolvido de forma reutilizável utilizando o atributo [Parameter].

[Parameter]
public string Titulo { get; set; }

[Parameter]
public int Peso { get; set; }
________________________________________________________________________________
Como funciona:
Titulo define o nome da ação ambiental
Peso define quantos pontos são adicionados por clique

Isso permite reutilizar o mesmo componente para diferentes ações, apenas alterando os valores passados na página principal.
__________________________________________________________________________________
Uso do componente:
<EcoStatus Titulo="Reciclagem de Plástico" Peso="1" />
<EcoStatus Titulo="Plantio de Árvores" Peso="10" />
<EcoStatus Titulo="Descarte de Eletrônicos" Peso="5" />
__________________________________________________________________________________
Conclusão

O projeto demonstra o uso de:

Componentização em Blazor
Parâmetros reutilizáveis
Manipulação de estado
Interatividade em tempo real

Além disso, aplica princípios de usabilidade para melhorar a experiência do usuário.
