# data-visualization

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)

![Badge code size](https://img.shields.io/github/languages/code-size/fab-souza/data-visualization)
![Badge de Atualização](https://img.shields.io/github/last-commit/fab-souza/data-visualization)

| :placard: Vitrine.Dev |    |
| -------------  | --- |
| :sparkles: Nome        | **Data Visualization**
| :label: Tecnologias | python
| :rocket: URL         | https://github.com/fab-souza/data-visualization/
| :fire: Desafio     | Conteúdo do curso [Data Visualization](https://www.alura.com.br/curso-online-data-visualization-com-seaborn)

![](https://user-images.githubusercontent.com/67301805/208895033-f126dcaa-a3d7-42f8-a40a-123db215c218.jpg#vitrinedev)


## Sobre o curso 📚

Neste curso sobre visualização de dados, do instrutor [Guilherme Lima](https://www.linkedin.com/in/guilherme-lima-458925178/), usamos um dataset sobre gorjetas de um restaurante, em que há registrado o valor consumido, valor da gorjeta, se houve pedido de sobremesa, dia da semana, qual era a refeição (almoço ou jantar) e o total de pessoas à mesa.

![image](https://user-images.githubusercontent.com/67301805/208898203-b89b3c6a-e4ba-407c-bcec-b423b3632013.png)

Eu aprendi como renomear os dados, seja para fazer sua tradução ou para atribuir um nome mais adequado à variável/dado, utilizando o *.rename()* e *.map()*. Também vi como fazer a visualização dos dados através da biblioteca **Seaborn**, por exemplo, se o valor da gorjeta é proporcional ao valor total da conta, se o pedido de sobremesa houve influência no valor da gorjeta, assim como, no dia da semana e horário da refeição. Para fazer as análises, foram usados a visualização gráfica e um teste de hipótese nula (H_0) e *valor-p*.

## Minha prática 👩🏻‍💻

Usei um dataset sobre filmes e séries da [Netflix](https://www.kaggle.com/datasets/thedevastator/the-ultimate-netflix-tv-shows-and-movies-dataset), disponível no [Kaggle](https://www.kaggle.com/), para pôr em prática o conteúdo deste curso. No total, há seis arquivos csv, porém só utilizei um, referente aos melhores filmes.

Depois, fiz a tradução das variáveis, através do *.rename()*, e traduzi os gêneros dos filmes e séries, com o *.map()*.

![image](https://user-images.githubusercontent.com/67301805/209211030-6eb2b87c-cc35-47f6-aa6b-bd45946b7987.png)

![image](https://user-images.githubusercontent.com/67301805/209211091-91e7c787-db72-4ac1-ab20-e282b5004f14.png)

Com os dataframes traduzidos, iniciei a parte analítica. A primeira análise foi: se há relação entre as notas dos filmes com sua duração. 

Ao plotar um gráfico entre a Duração com as Notas, não obtive um resultado que esperava.
&nbsp;![image](https://user-images.githubusercontent.com/67301805/210013922-88620236-8d0c-49df-80ec-47d8f3431a26.png)

Por exemplo, o gráfico entre a Duração X Ano de lançamento:

![image](https://user-images.githubusercontent.com/67301805/210014180-c61c9b41-2677-40f0-b568-58bbb7b1bc7a.png)

A variável referente ao ano de lançamento tem um intervalo maior do que as notas, por isso o primeiro gráfico não ficou com a mesma aparência.

Voltando a análise, utilizei o *.lmplot()* para apresentar se há a relação entre a duração dos filmes com suas notas:

![image](https://user-images.githubusercontent.com/67301805/210019151-d4921f50-721e-48f6-a45a-f05a976f81b6.png)

A inclinação da reta indica que quanto maior for a duração do filme, as notas tendem a aumentar também.

A segunda análise que fiz, foi: se há relação na distribuição das notas com o gênero dos filmes.

Utilizei os gêneros Comédia e Suspense, pois eles apresentaram uma amostra semelhante, 58 e 59 respectivamente. O gráfico *.lmplot()* entre a Nota X Duração apresentou uma distribuição diferente entre os gêneros.

![image](https://user-images.githubusercontent.com/67301805/210023733-e2c8b389-94ad-42cb-9b24-bad2dbee2d7c.png)

Para fazer a análise estatística, usei a biblioteca [**Scipy**](https://scipy.org/), que contém subpacotes de álgebra linear, cluster, processamento de sinal, entre outros, além de estatística. Determinei o teste de hipótese da seguinte forma: 
- Hipótese nula (H_0): a distribuição da nota é a mesma nos dois grupos;
- Hipótese alternativa (H_alt): a distribuição da nota não é a mesma.



## Ferramentas utilizadas 🧰
<p> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> 
    <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a>
    <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a>
    <a href="https://scipy.org/" target="_blank" rel="noreferrer"> <img src="https://scipy.org/images/logo.svg" alt="scipy" width="40" height="40"/> </a>
    </p>
