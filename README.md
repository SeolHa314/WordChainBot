# WordChainBot

이 봇은 끝말잇기를 할 수 있는 디스코드 봇 입니다.

## 단어추가에 대하여
dict.txt 파일은 끝말잇기에 사용될 단어에 대한 데이터베이스입니다.
따라서 끝말잇기 도중 누락된 단어를 찾으시게 된다면 dict.txt에 단어를 추가해주시기 바랍니다.

## 한방단어에 대하여
한방단어에 대한 데이터베이스는 봇 실행시 dict.txt에 나열된 단어들에 한정하여 사용시 끝말잇기가 종료되는 단어들을 따로 선별하여 구성됩니다.

```python
for i in wordDict:
    for j in wordDict[i]:
        if j[-1] not in wordDict:
            delList.append(j)
```
