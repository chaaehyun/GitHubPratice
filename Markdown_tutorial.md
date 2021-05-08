# **Markdown Syntax**

### **<Heading; 제목 만들기>**
- 단어나 구 앞에 숫자기호를 추가한다.  

- 사용하는 숫자 기호의 수는 제목 크기와 일치해야 한다.

- #의 수는 1에서 6으로 갈 수록 제목의 크기는 작아진다.  

>ex) 제목 크기 4`<h4>`를 만드려면 네 개의 #을 사용  
`#### My Header`

- 1단계 제목의 경우 ) 텍스트 아래줄에 '=' 문자를 1개 이상 추가한다.

- 2단계 제목의 경우 ) 텍스트 아래줄에 '-' 문자를 1개 이상 추가한다.

>## Heading level 1
>===================
>## Heading level 2
>`-----------------------`

        <주의 사항>
        - 숫자기호 # 와 제목 이름 사이에 공백이 있어야한다.

### **<paragraphs; 단락>**  
- 단락을 만드려면 빈 줄을 이용하여 하나 이상의 텍스트 줄을 구분한다.  
>ex)  
I love you
>
>    so much

    단락 주의 사항  
    - 단락이 목록에 없으면 공백이나 탭을 하지 않는다.

### **<Line Breaks; 줄 바꿈>**
- 줄 바꿈을 하려면 두 개이상의 공백으로 줄을 끝낸다.  

        <주의 사항>  
        - 줄 끝에 공백이나 `<br>`HTML 태그를 사용할 수 있다.
        - 권장하지 않는 경우  
         1) 줄 끝에 `\`(슬래시) 입력 : 모든 MarkDown 응용 프로그램이 지원하는 것은 아니다.

            좋은 예시)  
            First line.  (공백 있음)  
            Two llne.

            First line. (HTML 태그 있음)<br>
            Two line 

            나쁜 예시)  
            First line. (`\`있음) \
            Two line.

### **<Emphasis; 강조>**
- 글씨체를 bold체로 바꾸거나 italic체로 변경 가능함  
1. Bold  
    - 단어 또는 구문 앞 뒤에 두 개의 별표 또는 밑줄을 추가한다.

    - 단어 중간을 굵게 하려면 문자 앞뒤에 공백없이 별표를 두개 추가한다.  

    >ex)  
    I love **bold text**.  
    I love __bold text__.  
    Love **is** good.  

        <주의 사항>
        마크다운은 단어 중간에 있는 밑줄을 처리하는 방법을 사용하지 않는다.  
        -> 별표를 사용한다.

2. Ltalic  
    - 단어 또는 구문 앞 뒤에 별표 또는 밑줄을 추가한다.

    - 단어 중간을 기울이려면 문자 앞 뒤에 공백없이 별표 하나 또는 밑줄 하나 추가한다.

    >ex)  
    I love *italic*.  
    I love _italic_.  
    I _love_ you.

        * 마크다운은 단어 중간에 있는 밑줄을 처리하는 방법을 사용하지 않는다.  
        -> 별표를 사용한다.

3. Bold and Italic  
    - Bold체와 Italic체를 동시에 강조하려면  
    -> 단어나 구 앞 뒤에 별표 또는 밑줄 세개 추가
    (별표와 밑줄 합쳐서 3개)

            <주의사항>
             ___ 는 사용하지 않는게 좋다.

### **<Blockquotoes; 인용구>**  
- 단락 앞에 > 를 추가한다.

- **여러 단락이 있는 인용구인 경우**  
-> 단락 사이의 빈 줄에 > 를 추가한다.

>ex)  
>I love you.
>
>You love me?

### **<Nested Blockquotoes; 중첩 인용구>**  
- 인용구는 중첩이 가능하다. 중첩하려는 단락 앞에 >> 를 추가한다.  

>ex)  
>I love you
>
>>you love me?

### **<다른 요소가 있는 인용구>**  
- 인용구는 다른 MarkDown 형식의 요소를 포함 할 수 있다.

- 모든 요소를 사용할 순 없다.  
-> 어떤 요소가 작동하는지 알아봐야한다.

>ex)  
> ## This is good! //Heading
>
> - Because I'm handsome. // 앞에 원형 포인트
>
> *Everything* is **good**. // italic체, bold체

### **<List; 목록>**
- 항목을 정렬 된 목록과 정렬되지 않은 목록으로 구성할 수 있다.

1. 정렬된 리스트
    - 정렬 된 목록을 만들려면 숫자 뒤에 마침표가 있는 항목을 추가한다.

    - 숫자는 1부터 시작해야 하며, 순서대로 쓸 필요는 없다.

    >ex)  
    >2. Second list  
    >3. Third list  
    >4. Fourth list

    >ex)
    >1. First list
    >1. Second list
    >1. Third list

            <주의 사항>  
            - 1) 2) 는 모든 응용 프로그램에서 지원하는 것이 아니기 때문에, 마침표를 사용하기로 한다.

2. 정렬되지 않은 리스트
    - 라인 항목 앞에 -,*,+ 를 추가한다.  
    = 원형 포인트
    - 중첩 가능

            <주의 사항>
            - 동일한 목록에서 구분 기호를 혼합하지 않는다. 

- 목록의 연속성을 유지하면서 목록에 다른 요소를 추가하려면 공백 4개 또는 탭 1개 들여쓰기를 사용한다.

### **<Code Blocks; 코드 블록>**  
- 보통 공백 4개 또는 탭 1개 들여쓰기로 이용된다.

- 목록에 있는 경우에는 공백 8개 또는 탭 2개 들여쓰기를 사용한다.

### **<Images; 이미지>**  
ex) ![보라카이 사진](abc.png)  

- ![이미지 이름](이미지 경로 및 URL)

- 따옴표로 마우스 가져다 놓으면 뜨는 설명 추가 가능  
[![대체 텍스트](이미지 경로 또는 소스 URL "이미지 설명")]

- 이미지에 링크 삽입 가능  
[![대체 텍스트](이미지 경로 또는 소스 URL "이미지 설명")](링크 주소)

        <주의 사항>  
        - 앞에 ! 를 붙인다.
        - 사진 파일 이름을 영어로 저장한다.

### **<Code; 코드>**
- 단어나 구를 코드로 표시하려면 백틱``(`)``으로 묶는다.
ex) I think this type is `good`.

- 백틱 탈출  
-> 단어나 구를 이중 백틱 (``)으로 묶어 탈출시킬 수 있다.

### **<Horizontal Rules; 수평선>**
- 수평선을 만들 땐, 3개 이상의 별표(***), 대시(---), 또는 밑줄(___)을 한 줄에 단독으로 사용해준다.  
    
        <주의 사항>
        - 호환성을 위해서 수평 규칙 앞뒤에 빈 줄을 넣는다.

### **<Links; 링크>**
- 링크 텍스트를 괄호로 묶은 다음 (ex : [naver])   
바로 뒤에 주소를 괄호로 묶는다. (ex : (https://naver.com))  
-> `[텍스트](주소)`

- 제목 추가하기; 마우스를 가져다대면 뜨는 이름  
쌍따옴표 안에 써준다.  
>ex) My favorite search engine is [naver](https://naver.com "The best search engine for privacy").  

-> `[텍스트](주소 "설명")`

- 링크주소와 이메일 직접 삽입
    - `<https://www.markdownguide.org>`  
    -> <https://www.markdownguide.org>

    - `<fake@example.com>`  
    -> <fake@example.com> 

- 링크 서식 지정
    - 링크를 강조하려면  
    -> 굵게 하기 : 괄호 앞뒤에 별표 2개 추가  
    -> 기울이게 하기 : 괄호 앞뒤에 별표 1개 추가
    
    - 링크를 코드로 표시하려면 -> 괄호 안에 백틱을 추가  

    >ex)  
My favorite search engine is **[naver](https://naver.com "The best search engine for privacy")**.  
My favorite search engine is *[naver](https://naver.com "The best search engine for privacy")*.   
My favorite search engine is [`code`](#code).

- 참조 스타일 링크
    - 같은 링크 URL을 여러번 사용하거나 글 안의 링크를 따로 이용하고 싶을 때 사용
    
    - 첫번째 방법, 텍스트로 유지  
    -> `[텍스트][1]`  
    첫번째 대괄호 안에는 링크가 삽입되었다는 것을 표시해야하는 텍스트,  
    두번째 대괄호 안에는 문서의 다른 곳에 저장된 링크를 가르키는 데 사용된 레이블 표시

            <주의 사항>
            - 첫번째 대괄호와 두번째 대괄호 사이에 공백을 포함 할 수 있다.  
            - 두번째 대괄호에는 대소 문자를 구분하지 않는다. 또한, 문자, 숫자, 공백 또는 구두점 포함 가능하다.

    - 두번째 방법, 파일을 다른 곳에 저장  
    -> [1]: Welcome to Soongsil!  
    괄호와 콜론, 그리고 하나의 공백이 필요하다.  
    링크의 URL을 괄호로 묶을 수 있으며, " ", ' '를 이용하여 설명을 덧붙일 수 있다.

- 이미지에 링크 삽입  
-> [![이미지설명(이미지 소스 URL)]](링크URL)

<`README.md` URL>
- [README.md](https://github.com/chaaehyun/My-first-Repository/blob/main/README.md)