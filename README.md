# StackOverflow-semantic-search
## A semantic search engine for StackOverflow questions
Dataset : https://www.kaggle.com/stackoverflow/stacksample
        size: 3gb (zipped)
        loading : loading the dataset using Pandas would be a big mistake if you don't have about 5+ Gb of free ram as only the Questions.csv and Answers.csv takes about 5 Gb
                  to load the data use import csv and the encoding is latin1.
```python
import csv
with open('../input/stacksample/Questions.csv',encoding='latin1') as csv_file:
    read_csv=csv.reader(csv_file,delimiter=',')
    cnt=0
    next(read_csv,None)
    for row in read_csv:
        cnt+=1
print(cnt,len(row)) # no of rows 1264216 , no of columns 7
}
```
