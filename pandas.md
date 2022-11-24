## 파일
### 데이터 파일 로드
```
df = pd.read_csv('') 
+ encoding ='cp949' # 한글 안깨지게
+ header=None # 칼럼 초기화
+ names = [] # 칼럼명 지정
```
### 파일 미리보기
- 앞에서부터 5개 ``` df.head() ```
- 뒤에서부터 5개 ``` df.tail() ```
- 행, 열 개수 확인 ``` df.shape() ```
- 결측치 파악 ``` df.isnull().sum() ```
- 파일 정보 ``` df.info() ```
- 수치형 변수 분포 ``` describe() ```


## 인덱스 
__적용하려면 inplace = True 하기__
- 제거 ```df.style.hide_index() ```
- 대체 ```df.set_index("인덱스 컬럼명") ```
- 첫 행을 column으로 지정 ```
df1 = df.rename(columns=df.iloc[0]) 
df2 = df2.drop(df.index[0])
```

## 칼럼
- 전체 칼럼 출력 ``` df.columns ```
- 특정 칼럼 값 확인 ``` df.['칼럼명'] ```
- 칼럼명 변환 ``` df.columns = [] ```
