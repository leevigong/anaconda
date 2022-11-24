## 파일
### 데이터 파일 로드
```
df = pd.read_csv('') 
+ encoding ='cp949' # 한글 안깨지게
```
### 파일 미리보기
- 앞에서부터 5개
``` df.head() ```
- 뒤에서부터 5개
``` df.tail() ```

## 인덱스 
__적용하려면 inplace = True 하기__
- 제거 ```df.style.hide_index() ```
- 대체 ```df.set_index("인덱스 컬럼명") ```

