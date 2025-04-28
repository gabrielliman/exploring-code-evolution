# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: https://github.com/keras-team/keras

2. Gráfico selecionado: "Lines of Code (LOC)" e "Python files"
  
3. Explicação: No gráfico "Lines of Code (LOC)", observa-se uma forte expansão no início do histórico analisado, principalmente entre 2020 e 2021, quando o número de linhas de código praticamente quintuplicou, ultrapassando 200 mil linhas. Esse crescimento inicial provavelmente reflete a adição de novas funcionalidades, expansão de módulos e possíveis refatorações importantes. Entre 2021 e 2023, o projeto continuou crescendo, atingindo seu pico em 2023, com aproximadamente 300 mil linhas de código. A partir de 2024, nota-se uma queda significativa no número de linhas, o que pode ser explicado por limpezas de código, remoção de módulos obsoletos, ou processos de refatoração para tornar o repositório mais eficiente e modularizado. Em 2025, há uma leve recuperação, indicando que o projeto continua sendo ativamente desenvolvido, mas talvez agora de forma mais controlada.
Já no gráfico "Python files", a evolução é mais estável. Desde 2020, há um crescimento contínuo na quantidade de arquivos .py, refletindo a expansão do projeto em termos de número de componentes, testes ou utilitários. Mesmo em 2024, ano em que o número de linhas caiu no gráfico anterior, o número de arquivos se manteve praticamente estável. Isso sugere que a diminuição de linhas de código foi mais relacionada a otimizações internas do que à eliminação de funcionalidades inteiras. Em 2025, o número de arquivos cresce novamente, indicando a criação de novos módulos ou separação de lógicas em arquivos menores, o que é uma prática recomendada para facilitar a manutenção e a escalabilidade do projeto.
Em resumo, os gráficos mostram que o projeto Keras teve uma fase inicial de rápido crescimento, seguida por uma fase de otimização e maturidade, alinhando-se com boas práticas de desenvolvimento em projetos de grande escala.



