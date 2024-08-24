# [G](https://github.com/star-bits/sogang-aieg106/blob/main/g.ipynb) of RAG

- Few shot prompting으로 생성되는 답변의 포맷을 맞춤. autocast()를 이용한 Automatic Mixed Precision. Metric 파일을 뜯어와 스코어를 바로 확인하도록 구현.
- Retrieval의 경우, 모든 문장을 다음 문장과 비교해가며 문단 단위로 chunk를 만들고, 그 chunk들을 FAISS index에 넣는 방식으로 시도했지만 generation만 적용한 방법보다 오히려 스코어가 낮게 나왔음. 
