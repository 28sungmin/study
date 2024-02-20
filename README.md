TextRank

TextRank 알고리즘은 2004년 구글에서 발표한 PageRank 알고리즘을 기반으로 한 알고리즘이다[1].<br />
PageRank 알고리즘은 수집된 인터넷 문서 각각을 그래프의 노드, 문서 내부의 링크 정보를 간선으로 가정하여 방향성이 있는 그래프를 만들어 문서의 중요도를 계산한다.[2] TextRank 알고리즘은 PageRank의 개념을 자연어 처리에 응용한 것으로 문장, 단어와 같은 특정 단위들 간의 중요도를 계산하는 알고리즘이다. 문서 내의 각 문장을 그래프의 정점(vertex)으로 가정하는 경우 중요한 문장들을 선별할 수 있으며, 이를 통해 문서 요약이 가능하다. <br />
TextRank 알고리즘은 각 문장의 중요도를 구할 수 있어야 하는데, 문장 간 상관행렬을 이용하여 구할 수 있다.

입력 문서의 각 문장들에 대해 형태소 분석을 수행하고, 체언류와 용언류의 TF-IDF를 계산하여 문장-단어 행렬을 생성했다 그 뒤 생성된 문장-단어 행렬의 전치 행렬을 구하여 서로 곱해주면 문장 간의 상관관계(correlation)을 나타내는 행렬을 얻을 수 있다. 이렇게 구한 문장 간 상관행렬은 문장 간의 가중치 그래프로 나타낼 수 있고, 아래의 TextRank 수식을 통해 각 문장의 중요도를 구할 수 있다.

참고문헌<br />
[1] 이상영 외(2023), "TextRank 알고리즘 및 인공지능을 활용한 브레인스토밍", JPEE : Journal of practical engineering education = 실천공학교육논문지, v.15 no.2, pp.509 - 517 <br />
[2] 배원식과 차정원(2010), "TextRank 알고리즘을 이용한 문서 범주화", 정보과학회논문지. Journal of KIISE. 컴퓨팅의 실제 및 레터, v.16 no.1, pp.110-114 <br />
[3] 정석원 외(2017), "TextRank 알고리즘과 주의집중 순환 신경망을 이용한 하이브리드 문서 요약", 한국어정보학회 2017년도 제29회 한글및한국어정보처리학술대회, pp.47 - 50 <br />
