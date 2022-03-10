# hse_hw2_chip
## Анализ FastQC
### 1 реплика (ENCFF000BBJ)
![image](img/BBJ_fastqc_1.png)

Качество прочтений достаточно хорошее и под конец рида не сильно падает:

![image](img/BBJ_fastqc_2.png)
![image](img/BBJ_fastqc_3.png)
![image](img/BBJ_fastqc_4.png)

GC неплохой, близкий к идеальному:

![image](img/BBJ_fastqc_5.png)

Лишних адаптеров не нашлось:

![image](img/BBJ_fastqc_6.png)

### 2 реплика (ENCFF000BBK)
![image](img/BBK_fastqc_1.png)

Качество прочтений даже лучше, чем у первой реплики:

![image](img/BBK_fastqc_2.png)
![image](img/BBK_fastqc_3.png)
![image](img/BBK_fastqc_4.png)

GC состав примерно такой же, как для первой реплики:

![image](img/BBK_fastqc_5.png)

Лишних адаптеров нет:

![image](img/BBK_fastqc_6.png)

### Контроль (ENCFF000BAU)
![image](img/BAU_fastqc_1.png)

Качество ридов выглядит плохим, но при этом если посмотреть на боксплоты, то становится понятно, что плохих ридов очень мало, сами боксплоты без "усов" лежат в зеленой зоне:

![image](img/BAU_fastqc_2.png)
![image](img/BAU_fastqc_3.png)
![image](img/BAU_fastqc_4.png)

GC состав похож на реплики:

![image](img/BAU_fastqc_5.png)

Лишних адаптеров так же нет:

![image](img/BAU_fastqc_6.png)

Комментарий: Даже без подрезания ридов их качество достаточно хорошее


## Статистика выравнивания на chr16
|ID fastq | Всего ридов в файле	| Ридов выровнилось уникально	| Ридов выровнилось НЕ-уникально | Ридов не выровнилось|
|---|---|---|---|---|
|ENCFF000BBJ	| 43331646 |	1634955 (3.77%) |	6227042 (14.37%) |	35469649 (81.86%)|
|ENCFF000BBK	| 36708842 |	1421250 (3.87%) |	5431020 (14.79%) |	29856572 (81.33%)|
|ENCFF000BAU	| 84569628 |	2843887 (3.36%) |	10264984 (12.14%) |	71460757 (84.50%)|

## Диаграммы Эйлера-Венна

### Пересечение пиков 1 реплики (...BBJ) с пиками ENCODE

![image](Intervene_venn_BBJ_1.pdf)

### Пересечение пиков ENCODE с пиками 1 реплики (...BBJ)

![image](Intervene_venn_BBJ_2.pdf)

### Пересечение пиков 2 реплики (...BBK) с пиками ENCODE

![image](Intervene_venn_BBK_1.pdf)

### Пересечение пиков ENCODE с пиками 2 реплики (...BBK)

![image](Intervene_venn_BBK_2.pdf)
