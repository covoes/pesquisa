# Escrita

- Notação matemática deve seguir a convenção de:
  - Escalares: letras minúsculas em itálica: ![x,y](https://render.githubusercontent.com/render/math?math=x%2Cy)
    - Quando tiverem significado importante e não forem alterados, como número de objetos e número de atributos, usar letra maiúscula como *N* e *M*. Assim, ao ter um somatório sobre o número de objetos, você pode utilizar a letra minúscula para fazer a indexação. Essa é a notação padrão no livro do Bishop (PRML), por exemplo.
  - Vetores: letras minúsculas em negrito: ![\mathbf{x}, \mathbf{y}](https://render.githubusercontent.com/render/math?math=%5Cmathbf%7Bx%7D%2C%20%5Cmathbf%7By%7D)
  - Matrizes: letras maiúsculas em negrito: ![\mathbf{X}, \mathbf{Y}](https://render.githubusercontent.com/render/math?math=%5Cmathbf%7BX%7D%2C%20%5Cmathbf%7BY%7D)
  - Conjuntos: letras caligráficas maiúsculas (`\mathcal` no LaTeX): ![\mathcal{X}, \mathcal{Y}](https://render.githubusercontent.com/render/math?math=%5Cmathcal%7BX%7D%2C%20%5Cmathcal%7BY%7D)
  - Por exemplo, podemos definir um cojunto de dados como ![\mathcal{X} = \{\mathbf{x}_i\}_{i=1}^N, \mathbf{x}_i \in \mathbb{R}^M](https://render.githubusercontent.com/render/math?math=%5Cmathcal%7BX%7D%20%3D%20%5C%7B%5Cmathbf%7Bx%7D_i%5C%7D_%7Bi%3D1%7D%5EN%2C%20%5Cmathbf%7Bx%7D_i%20%5Cin%20%5Cmathbb%7BR%7D%5EM)
- LaTeX
  - Caso não conheça LaTeX, sugiro dar uma olhada nas ![notas do curso de LaTeX da Profa. Carla Negri](http://professor.ufabc.edu.br/~carla.negri/latex/apostila.pdf).
  - Um novo parágrafo só é iniciado ao ter uma linha em branco entre duas sentenças. 
  Aproveite-se disso e não coloque todo o conteúdo do parágrafo em uma única linha de texto. 
  Cada frase ficando em uma linha facilita identificar as mudanças nas revisões.
  - Procure sempre ter seu texto em um repositório git (seja github/bitbucket/etc), para que as revisões sejam feitas via pull request.
  - Tags para símbolos matemáticos neste [link](https://www.caam.rice.edu/~heinken/latex/symbols.pdf)

# Experimentos/Análises

- A média só conta parte da história, sempre guarde os valores de cada execução se possível.
  - Caso não seja possível, guarde ao menos o desvio-padrão.
- Prefira boxplots a gráficos de barra
- Escolha cores amigáveis aos daltônicos
  - [Aqui tem algumas dicas](https://thenode.biologists.com/data-visualization-with-flying-colors/research/)
- Não esqueça de por rótulos nos eixos dos gráficos
- No caso de gráfico de linhas, além da cor use diferentes tipos de linha (pontilhada, tracejada, sólida etc)
- Gere um arquivo de log para cada experimento e adicione nele o hash do commit referente a versão do código sendo usada
- Setar a semente do gerador de números aleatórios nos experimentos e guardar o número que foi usado
  - Cuidado para que cada repetição de um experimento use uma semente diferente das outras
  
