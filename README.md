# VibingData.co - Projetos de Dados Reais

> *"Dados são o novo petróleo."*
> — alguém que nunca limpou um CSV na vida

---

## 1. A VibingData.co

A VibingData.co é uma startup de dados que promete transformar **planilhas enormes em dashboards incríveis no Streamlit**.

No pitch deck, tudo parece muito bem estruturado: pipelines modernos, arquitetura de dados robusta, times multidisciplinares alinhados com OKRs.

Na prática, os dados chegam por WhatsApp. Às vezes como `.xlsx`. Às vezes o arquivo trava o Excel. Às vezes são nove CSVs sem documentação nenhuma com um "boa sorte" implícito.

Mas alguém tem que fazer o trabalho. E esse alguém, desta vez, é o Gustavo.

---

## 2. Gustavo

Gustavo é Analista de Dados na VibingData.co.

Antes disso, era, segundo o próprio LinkedIn, *"Arquiteto de Software Sênior | Especialista em Design Patterns | Clean Architecture Evangelist"*.

Na prática, Gustavo era o tipo de profissional que sabia explicar a diferença entre CQRS e Event Sourcing em detalhes minuciosos, mas travava na hora de abrir um terminal. Conhecia os nomes de todos os padrões de projeto do GoF. Nunca tinha implementado nenhum.

Quando finalmente foi encarregado de entregar um MVC funcional de uma loja, não entregou. Semanas se passaram. Reuniões foram remarcadas. Justificativas foram ficando cada vez mais elaboradas e cada vez menos técnicas.

No fim, um estagiário foi chamado. Em duas semanas, o estagiário entregou o que Gustavo não conseguiu em meses.

Gustavo foi demitido.

Depois disso, mandou currículo pra várias empresas. A maioria não respondeu. Algumas fizeram entrevista e não deram retorno. A VibingData.co respondeu.

Ele aceitou no mesmo dia.

---

## 3. O Primeiro Dia

Gustavo chegou esperando uma reunião de alinhamento. Talvez um tour pelo Confluence. Uma apresentação de arquitetura. Alguma cerimônia que deixasse claro que ali, diferente do último lugar, as coisas eram feitas com rigor.

O que ele recebeu foi uma mensagem no Slack:

> *"Oi Gustavo! Bem-vindo :) Já te adicionei nos dois projetos da semana. Os datasets estão na pasta compartilhada. Preciso dos dashboards até sexta. Qualquer dúvida me chama!"*

Eram dois projetos. Era segunda-feira. Sexta era em quatro dias.

Gustavo respondeu *"Claro, pode deixar!"* e abriu os arquivos.

O primeiro travou o notebook dele por três minutos antes de carregar.

---

## 4. Os Dois Projetos

### Projeto 1 - Olist

A Olist é uma plataforma que conecta pequenos vendedores a grandes marketplaces brasileiros. Eles têm um problema: as avaliações dos clientes caíram nos últimos meses e não sabem exatamente por quê.

Eles contrataram a VibingData para descobrir. O dataset tem **100 mil pedidos reais de 2016 a 2018**, divididos em **9 arquivos CSV separados** - pedidos, clientes, vendedores, produtos, pagamentos, avaliações e geolocalização.

Nenhum arquivo faz sentido sozinho. Todos precisam ser conectados.

O cliente quer um dashboard que mostre onde as avaliações caem, por quê, e quem são os vendedores com pior performance.

### Projeto 2 - Stack Overflow Developer Survey

A própria VibingData quer entender o mercado. O RH precisa calibrar os salários do time com base em dados reais do setor tech.

O dataset é o **Stack Overflow Annual Developer Survey** - dezenas de milhares de respostas de desenvolvedores do mundo todo sobre salário, linguagens, satisfação no trabalho e experiência.

O cliente, nesse caso, é interno. O que não significa que é mais simples - significa que qualquer erro vai aparecer na próxima reunião de time.

---

## 5. O VibingAI

A VibingData tem um modelo interno chamado **VibingAI**.

Ele foi treinado em dados reais de todas as áreas da empresa: tickets de suporte, histórico de projetos, contratos, documentação interna, dados de RH. A ideia era ter um assistente que conhecesse o contexto da empresa de verdade, não um modelo genérico que precisava ser explicado do zero a cada conversa.

Gustavo adotou o VibingAI imediatamente. Não como ferramenta de apoio - como substituto. Ele não lia os outputs com atenção. Não questionava o que o modelo sugeria. Colava o código gerado diretamente no notebook e passava pra próxima célula.

Pra Gustavo, o VibingAI era o analista de dados. Ele era o gerente.

O problema é que modelos treinados em dados de RH sabem coisas que não deveriam ser ditas em voz alta.

---

## 6. O Que Aconteceu

Dez dias depois de receber os projetos, seis dias além do prazo original, Gustavo estava no meio de uma célula do notebook pedindo ajuda ao VibingAI para fazer um merge entre duas tabelas do dataset da Olist.

O modelo respondeu:

```
Não foi possível completar a operação.
Usuário gustavo não faz parte dessa organização.
```

Gustavo leu a mensagem duas vezes.

Pediu pra repetir. O modelo repetiu.

Tentou reformular a pergunta. O modelo continuou sem acesso.

Fechou o notebook. Não salvou.

---

## 7. O Que Você Vai Encontrar

Neste repositório estão os dois notebooks que Gustavo deixou pra trás:

- **`notebook_olist.ipynb`** - análise da base da Olist. Gustavo carregou um dos nove arquivos, achou que era o dataset completo, e fez análises em cima de dados incompletos. Tem merges errados, dropnas que destroem dados, e uma célula no final com um comentário que ele não terminou de escrever.

- **`notebook_stackoverflow.ipynb`** - análise do Developer Survey. Gustavo filtrou os dados pra confirmar o que já acreditava sobre salários de arquitetos. Tem viés de confirmação embutido no código, colunas não tratadas, e uma visualização que parece certa mas está completamente errada.

Os dois notebooks rodam. Esse é o problema, código que roda não é código que está certo.

---

## 8. Sua Missão

Você recebeu esses notebooks.

O cliente ainda precisa do dashboard. O prazo já era. Mas o trabalho não foi feito, foi *começado*, que é diferente.

Sua tarefa é pegar o trabalho do Gustavo, entender o que está errado, corrigir, e terminar.

**Você pode escolher:**

- Continuar só o projeto **Olist**
- Continuar só o projeto **Stack Overflow**
- Continuar os **dois**

Independente da escolha, a entrega esperada é:

1. **Limpeza e tratamento dos dados** - documentada e justificada. Não basta corrigir, precisa explicar por que o código do Gustavo estava errado.
2. **Análise exploratória** - com visualizações que respondam às perguntas do cliente.
3. **Entrega final** - um dashboard em Streamlit **ou** um modelo preditivo. Você escolhe o formato, mas precisa justificar a escolha.

Não existe resposta certa. Existe análise honesta.

---

## 9. Setup e Dependências

### Datasets

Faça o download antes de começar:

- **Olist:** [kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
  Baixe todos os 9 arquivos CSV e coloque numa pasta chamada `/data/olist/`

- **Stack Overflow Survey:** [survey.stackoverflow.co](https://survey.stackoverflow.co/)
  Escolha o ano desejado, baixe o CSV e coloque em `/data/stackoverflow/`

### Rodando no Google Colab

```python
# Monte seu Google Drive
from google.colab import drive
drive.mount('/content/drive')

# Instale as dependências
!pip install pandas numpy matplotlib seaborn plotly streamlit
```

### Libs utilizadas nos notebooks

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
```

---

> Os dados não mentem.
> Às vezes a gente só não está fazendo as perguntas certas.
> E às vezes o código está errado mesmo.