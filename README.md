# Plotly Notebook
Repositório criado com intuito de publicar  conteúdos relacionados ao aprendizado da biblioteca plotly no python 

<h1> Estudos pandas e plotly </h1>
A biblioteca Plotly oferece uma variedade de opções para criar visualizações interativas. Aqui estão algumas das funções e gráficos mais comuns disponíveis no Plotly Express:
<br>
<br>

<strong> 1. Gráficos de Barras: </strong>

```python

px.bar(): #Cria gráficos de barras.

```
```python 
px.histogram(): #Cria histogramas.
````
<strong> 2. Gráficos de Linhas:</strong>

```python 
px.line(): #Cria gráficos de linhas.

````

```python
px.scatter(): #Cria gráficos de dispersão.

````

<strong> 3. Gráficos de Pizza e Donut: </strong>

```python
px.pie(): #Cria gráficos de pizza.

px.sunburst(): #Cria gráficos de sunburst.

px.treemap(): #Cria gráficos de treemap.
```

<strong> 4. Gráficos 3D:</strong>

```python
px.scatter_3d(): #Cria gráficos de dispersão tridimensionais.

px.line_3d(): #Cria gráficos de linhas tridimensionais.
```

<strong> 5. Gráficos Geográficos: </strong>

```python

px.scatter_geo(): #Cria gráficos de dispersão geográficos.

px.choropleth(): #Cria mapas coropléticos.
```

<strong>6. Gráficos de Caixas:</strong>

```python
px.box(): #Cria gráficos de caixas.
```

<strong> 7. Gráficos de Violino:</strong>
```python
px.violin(): #Cria gráficos de violino.
```

<strong> 8. Gráficos de Calor:</strong>

```python
px.imshow(): #Cria gráficos de calor.
```

<strong> 9. Gráficos Animados:</strong>

```python
px.scatter(), px.line(), etc., com o parâmetro animation_frame: #Cria gráficos animados ao longo de uma dimensão.
```

<strong> 10. Gráficos de Radar:</strong>

```python
px.line_polar(): #Cria gráficos de linhas em coordenadas polares.
```

<strong> 11. Gráficos de Radar (Áreas):</strong>

```python
px.area_polar(): #Cria gráficos de áreas em coordenadas polares.
```


<strong> 12. Gráficos de Barras Empilhadas ou Agrupadas: </strong>
Configuração do parâmetro barmode para stack ou group em gráficos de barras.

<strong> 13 Mapas de Calor (Superfície):</strong>

```python 
px.surface(): #Cria mapas de calor em 3D
```
<strong> 14. Gráficos de Sankey:</strong> 

```python
px.sankey(): #Cria gráficos de fluxo de Sankey.
```
<h3>Artigo </h3>
link: https://oander.site/Artigos/Plotando%20gra%CC%81ficos%20com%20Plotly
<br><br>

![image](https://github.com/oanderoficial/plotly_notebook/assets/32654298/eb019215-d525-411a-8424-8d5b6fc1c9b0)

<h4> Exemplos: </h4>

<strong> Gráfico de dispersão 3D </strong>

```python
import pandas as pd
import plotly.express as px

# DataFrame de exemplo
data = {'X': [1, 2, 3, 4],
        'Y': [9, 11, 12, 13],
        'Z': [100, 110, 120, 130]}
df = pd.DataFrame(data)

# Gráfico de dispersão 3D
figura = px.scatter_3d(df, x='X', y='Y', z='Z', title='Gráfico de Dispersão 3D', template='plotly_dark')
figura.show()

```
