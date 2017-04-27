

# Medical Appointment No Shows

- Dataset : Kaggle Data

- 분석

필요없는 column을 제거해주고 문자를 숫자로 음수값을 양수값으로 바꿔주는 전처리 시행

heatmap과 pairplot을 이용해 분포와 변수들의 상관관계를 알아보았다

변수들의 중요도를 알아보기 위해 랜덤포레스트를 이용하여 모든 노드에 IG를 비교하여 변수의 중요도를 알아보았다

역시나 나이와 시간이 압도적으로 관계가 있는 것을 알 수 있었다

그리고 LogisticRegression 과 RandomForest 모형을 돌려보았다

LogisticRegression 을 실행한 결과

Train Score : 0.696736318408 Test Score : 0.698141414141 auc : 0.56207855268257911

RandomForest 를 실행한 결과

Train Score : 0.811084577114 Test Score : 0.639262626263 auc : 0.69673631840796024

RandomForest가 조금 높게 나왔지만 만족할만한 수치는 나오지 않았다

조금 더 스케일링이 필요한 것
