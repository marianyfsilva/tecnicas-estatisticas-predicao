# A população, escolaridade e o desemprego influenciam na taxa de roubos ocorridos em uma cidade?

Disciplina: INE5649-03238 (20212) - Técnicas Estatísticas de Predição

Professor: Luiz Ricardo Nakamura

Aluna: Mariany Ferreira da Silva, 19200646

---

## Dependencias

- [Python::3.9](https://www.python.org/downloads/)
- [Pip::22.0.3](https://pip.pypa.io/en/stable/installation/)
- [R](https://www.r-project.org/)
    - [ggplot2](https://ggplot2.tidyverse.org/)
- [Jupiter Notebook](https://jupyter.org/install#jupyter-notebook)

## Executar Jupiter Notebook

```
jupyter notebook
```

---

## Introdução, justificativa e objetivos

TO DO

## Materiais e métodos

TO DO

### Variáveis

- Variável Resposta: Roubos por 100 mil habitantes (robbbPerPop - porcentagem_de_roubos_a_cada_100_mil)

-1 >  forte  < -0.7 >  moderada  < -0.3 >  inexistente  < 0 >  inexistente  < 0.3 >  moderada  < 0.7 >  forte  < 1

- Variável Explicativa 1: População (population - populacao)
    ```
    cor(data$populacao, data$porcentagem_de_roubos_a_cada_100_mil)
    0.313707883492361       # 0.3 >  moderada  < 0.7
    ```
- Variável Explicativa 2: Indice de Renda per capta (perCapInc - indice_renda_per_capta)
    ```
    cor(data$indice_renda_per_capta, data$porcentagem_de_roubos_a_cada_100_mil)
    -0.199774789070242      # -0.3 >  inexistente  < 0
    ```
- Variável Explicativa 3: % Pessoas com nível básico incompleto (PctLess9thGrade - porcentagem_nivel_basico)
    ```
    cor(data$porcentagem_nivel_basico, data$porcentagem_de_roubos_a_cada_100_mil)
    0.286359376926176       # 0 >  inexistente  < 0.3
    ```
- Variável Explicativa 4: % Pessoas com nível médio incompleto (PctNotHSGrad - porcentagem_sem_nivel_medio)
    ```
    cor(data$porcentagem_sem_nivel_medio, data$porcentagem_de_roubos_a_cada_100_mil)
    0.38084784405838        # 0.3 >  moderada  < 0.7
    ```
- Variável Explicativa 5: % Pessoas com nível superior completo (PctBSorMore - porcentagem_com_nivel_superior)
    ```
    cor(data$porcentagem_com_nivel_superior, data$porcentagem_de_roubos_a_cada_100_mil)
    -0.199035533749529      # -0.3 >  inexistente  < 0 
    ```
- Variável Explicativa 6: % Desemprego (PctUnemployed - porcentagem_desempregados)
    ```
    cor(data$porcentagem_desempregados, data$porcentagem_de_roubos_a_cada_100_mil)
    0.425467868475479       # 0.3 >  moderada  < 0.7
    ```

### Dataset
[Kaggle - UCI - Data Set](https://www.kaggle.com/kkanda/communities%20and%20crime%20unnormalized%20data%20set?select=crimedata.csv)

### Dicionário de dados
[UCI - Data Set Information](http://archive.ics.uci.edu/ml/datasets/Communities%20and%20Crime%20Unnormalized)


### Diagramas de dispersão iniciais

|![populacao](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/populacao.png?raw=true)
![indice_de_renda_per_capta](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/indice_de_renda_per_capta.png?raw=true)
![pessoas_com_nivel_basico_incompleto](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/pessoas_com_nivel_basico_incompleto.png?raw=true)
![pessoas_com_nivel_medio_incompleto](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/pessoas_com_nivel_medio_incompleto.png?raw=true)
![pessoas_com_nivel_superior_completo](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/pessoas_com_nivel_superior_completo.png?raw=true)
![desempregados](https://github.com/marianyfsilva/tecnicas-estatisticas-predicao/blob/master/diagramas_de_dispersao/desempregados.png?raw=true)|

## Resultados e discussões

TO DO

## Considerações finais

TO DO

## Referências bibliográficas
