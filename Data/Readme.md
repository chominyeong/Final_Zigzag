### 코드 description
#### 지그재그_상품&리뷰_크롤링.ipynb
- 카테고리별 링크를 가져와 selenium으로 크롤링 진행
- 카테고리는 의류 / 가방 / 슈즈 / 뷰티 선정
<br>


#### 지그재그_리뷰_EDA.ipynb
- 글자 수, 토큰 분포 확인
- 전체 / 카테고리 별 단순 명사 추출
- 전체 / 카테고리 별 2글자 이상 명사 추출
- n-gram 추출 (n=2, 3)
<br>


#### Zigzag_리뷰_키워드추출_후보군.ipynb
- 키워드 추출 2가지 후보군
1. CountVectorizer
2. TfidfVectorizer
<br>


#### Zigzag_리뷰_키워드추출.ipynb
**1️⃣ [1차 키워드 추출] 상품ID = 130108350**
- 상품명 / 리뷰 코멘트 / clean_count / clean_tfidf 각각
  1. 빈도 분석
  2. PMI
  3. Word Embedding
-> PMI는 사용 불가, 리뷰 코멘트보다는 CountVectorizer (review_count) & TfidfVectorizer (review_tfidf)로 다시 한 번 진행 (형용사 & 명사 사용)
<br>

**2️⃣ [2차 키워드 추출] 상품ID = 130108350**
1. 상품명에서 명사 출력    
2. 리뷰 코멘트 전처리 - CountVectorizer (clean_count)    
   - 명사 / 형용사 출력    
   - 형용사 사용 - Word Embedding    
<br>
<br>
<br>

**참고**
: https://github.com/jyjnote/Zigzag-
