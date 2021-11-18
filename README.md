# TextAnalytics using _ nltk

# wordcloud 이용하여 단어빈도 분석하기

## **통계적 처리**

gutenberg 내 corpus들의 평균 단어 길이, 평균 문장 길이, 그리고 각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수(어휘 다양성 점수)를 먼저 알아보겠습니다.

```
평균단어길이:4, 평균 문장 길이 : 24,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 26, austen-emma.txt

평균단어길이:4, 평균 문장 길이 : 26,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 16, austen-persuasion.txt

평균단어길이:4, 평균 문장 길이 : 28,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 22, austen-sense.txt

평균단어길이:4, 평균 문장 길이 : 33,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 79, bible-kjv.txt

평균단어길이:4, 평균 문장 길이 : 19,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 5, blake-poems.txt

평균단어길이:4, 평균 문장 길이 : 19,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 14, bryant-stories.txt

평균단어길이:4, 평균 문장 길이 : 17,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 12, burgess-busterbrown.txt

평균단어길이:4, 평균 문장 길이 : 20,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 12, carroll-alice.txt

평균단어길이:4, 평균 문장 길이 : 20,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 11, chesterton-ball.txt

평균단어길이:4, 평균 문장 길이 : 22,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 11, chesterton-brown.txt

평균단어길이:4, 평균 문장 길이 : 18,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 10, chesterton-thursday.txt

평균단어길이:4, 평균 문장 길이 : 20,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 24, edgeworth-parents.txt

평균단어길이:4, 평균 문장 길이 : 25,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 15, melville-moby_dick.txt

평균단어길이:4, 평균 문장 길이 : 52,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 10, milton-paradise.txt

평균단어길이:4, 평균 문장 길이 : 11,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 8, shakespeare-caesar.txt

평균단어길이:4, 평균 문장 길이 : 12,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 7, shakespeare-hamlet.txt

평균단어길이:4, 평균 문장 길이 : 12,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 6, shakespeare-macbeth.txt

평균단어길이:4, 평균 문장 길이 : 36,
각 어휘 항목이 텍스트에 평균적으로 나타나는 횟수 : 12, whitman-leaves.txt
```

제가 중점적으로 분석할 austen, cheserton, sakespeare 세 작가의 작품은

**austen : austen-emma.txt**

**cheserton : chesterton-brown.txt**

**sakespeare : shakespeare-hamlet.txt** 

이렇게 3가지를 중심으로 해서 분석할 예정입니다. 

자세한 내용은 pdf 참고 부탁드립니다
