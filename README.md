# HTML?
- "Hyper Text Mark-up Language" 의 약자. 웹 페이지의 모습을 기술하기 위한 규약. 프로그래밍 언어가 아니라 마크업 언어이다.

# HTML 기본 구조
```
<!DOCTYPE html>
<html>
<head>
  <title>title</title>
  <meta charset="utf-8" />
</head>
<body>

</body>
</html>
```
- head tag
  - 문서의 형태, 타이틀 정보, 스타일 정보, 자바스크립트에 대한 정보가 들어가는 부분
  - 웹 브라우저가 알아야 할 중요한 정보들이 들어가는 곳
  
- body tag
  - 정보 전달을 위한 데이터가 들어가는 부분
  - 화면에 직접 출력되는 부분

# HTML 구성요소
- 요소(Elements)
  - HTML에서 시작태그와 종료태그로 이루어진 모든 명령어들
- 태그(Tag)
  - 요소의 하나로서 시작태그와 종료태그로 이루어져 있음
  - ```
      <h1>hello my world!<h1/>
    ```
- 속성(Attributes)
  - 좀 더 구체화된 명령어
  - 요소의 시작태그안에 사용
  - 다양한 효과를 부여
  - ```
      <p font-size: 10px;>hello my world!<p/>
    ```
- 값(Arguments)
  - 속성과 관련된 값을 의미
# HTML tag
![TAG_LANK](./img/tag_rank.JPG)  
 
Link: https://www.advancedwebranking.com/html/

- html tag에는 종류가 많기 때문에 자주 쓰이는 tag들을 제외한 나머지 tag들은 필요할때 찾아가면서 쓰는 것이 좋다.

- 대표적인 태그 몇가지
  - ```
      <p>hello world!<p/>
    ```
    - <p>hello world!<p/>
  - ```
    <img src="./img/lab.jpg" width="100px">
    ```
    - <img src="./img/lab.jpg" width="100px">
  - ```
      <table border="2">
        <tr>
            <td>이름</td>     <td>성별</td>   <td>주소</td>
        </tr>
        <tr>
            <td>땅땅이</td>  <td>남</td>      <td >대구</td>
        </tr>
        <tr>
            <td>춘식이</td>  <td>여</td>      <td>제주도</td>
        </tr>
      </table>
      ```
    - <table border="2">
        <tr>
            <td>이름</td>     <td>성별</td>   <td>주소</td>
        </tr>
        <tr>
            <td>땅땅이</td>  <td>남</td>      <td >대구</td>
        </tr>
        <tr>
            <td>춘식이</td>  <td>여</td>      <td>제주도</td>
        </tr>
      </table>

  - ```
      <form action="값을 보내고 싶은 경로">
        <p>아이디 : <input type="text" name="id"></p>
        <p>비밀번호 : <input type="password" name="pwd"></p>
        <input type="submit">
      </form>
      ```
    - <img src="./img/form1.png" height="90px"></img><br/> 
  - ```
      <select name="color">
        <option value="red">붉은색</option>
        <option value="black">검은색</option>
        <option value="blue">파란색</option>
      </select>
      <select name="color2" multiple>
        <option value="red">붉은색</option>
        <option value="black">검은색</option>
        <option value="blue">파란색</option>
      </select>
    ```
    - <img src="./img/form2.png" height="90px"></img><br/> 
  - ```
    <p>
        <h1>색상(단일선택)</h1>
        붉은색 : <input type="radio" name="color" value="red">
        검은색 : <input type="radio" name="color" value="black" checked>
        파란색 : <input type="radio" name="color" value="blue">
    </p>
    <p>
        <h1>사이즈(다중선택)</h1>
        95 : <input type="checkbox" name="size" value="95">
        100 : <input type="checkbox" name="size" value="100" checked>
        105 : <input type="checkbox" name="size" value="105" checked>
    </p>
    ```
    - <img src="./img/form3.png" height="180px"></img><br/>

  - ```
        <div style="border: 6px solid black; border-radius: 50%; background: deepskyblue; border: 6px solid black; width: 300px; height: 300px;"></div>
    ```
    - <img src="./img/divCircle.png" height="180px"></img><br/>
      - border-radius 속성은 모서리의 둥근 정도를 조절함

# semantic tag
- semantic tag?
  - 문서의 정보를 보다 잘 표현하기 위해 사용하는 의미를 갖는 태그들
- 쓰는 이유
  - 의미있는 태그를 사용하여 개발자와 브라우저에게 어떤 의미를 가진 요소인지 인식
  - 개발자에게는 코드를 보고 어떤 구조로 이루어져있는지 좀 더 빠른 파악이 가능하고
  브라우저에게는 검색 엔진이 좀 더 정확한 검색을 할 수 있도록 도움
- semantic tag 종류
  - https://opentutorials.org/course/2039/10954
- example
  - ```
      <html> 
      <head> 
        <title>문서 제목</title>
        <meta> 
      </head>
      <body> 
        <header> 
      	  <h1>안녕하세요!</h1> 
        </header>
        <section> 
          <nav> 
            <ol> 
              <li>홈으로 이동</li> 
              <li>메뉴로 이동</li>
       	    </ol>
          </nav>
          <main> 
            <article> 
              <h2>주요 내용...</h2>
				    </article>
				    <article>
		          <h2>주요 내용...2</h2>
				    </article>
          </main>
          <aside></aside> 
        </section>
        <footer> 
          <ul>
            <li>작성자 : 000</li>
            <li>저작권 ...</li>
          </ul>
        </footer>
      </body>
      </html>
    ```

---------------------------------
---------------------------------
# CSS?
- 종속형 시트 또는 캐스케이딩 스타일 시트(Cascading Style Sheets, CSS)는 마크업 언어가 실제 표시되는 방법을 기술하는 스타일 언어(style sheet language)로[1], HTML과 XHTML에 주로 쓰이며, XML에서도 사용할 수 있다. 기본 파일 명 W3C의 표준이며, 레이아웃과 스타일을 정의할 때의 자유도가 높다.
  
# CSS example
- html
  - ```
      <p class="cssName">hello my world!<p/>
    ```
- css
  - ```
      .cssName{
        font-size: 30px;
        text-align: center;
      }
    ```
- result
  - <img src="./img/cssExample.png" height="180px"></img><br/>


# CSS, HTML 연결

1. Inline Style Sheet
  - ```
      <p style="color: blue">Lorem ipsum dolor.</p>
    ``` 
2. Internal Style Sheet
  - ```
      <!doctype html>
      <html>
      <head>
      <style>
        p {
          color: red;
        }
      </style>
      </head>
      <body>
        <p>This is my paragraph.</p>
      </body>
      </html>
    ```
3. Linking Style Sheet
  - css
    - ```
        p {
          color: red;
        }
      ```
  - html
    - ```
      <!doctype html>
      <html>
      <head>
        <link rel="stylesheet" href="style.css">
      </head>
      <body>
        <p>This is my paragraph.</p>
      </body>
      </html>
      ```

# inline vs block vs inline-block
- inline
  - ```
      <a>a1 tag</a><a>a2 tag</a>
    ```
  - <a>a1 tag</a><a>a2 tag</a>
  - margin, padding, border, width, height 속성을 수정할 수 없다.
- block
  - ```
      <h1>h1 tag</h1><h1>h2 tag</h1>
    ```
  - <h1>h1 tag</h1><h1>h2 tag</h1>
  - 가로 전체(줄)를 차지한다.  
- inline-block
  - ```
      <a>a1 tag</a><a>a2 tag</a>
    ```
  - <img src="./img/inline_block.png" height="180px"></img><br/>
  - inline과 다르게 margin, padding, border, width, height 속성을 수정할 수 있다.
# CSS box model
- box model?
  - 모든 HTML 요소는 박스(box) 모양으로 구성되며, 이것을 박스 모델(box model)이라고 부릅니다.
- 구성
  - 내용(content) : 텍스트나 이미지가 들어있는 박스의 실질적인 내용 부분입니다.

  - 패딩(padding) : 내용과 테두리 사이의 간격입니다. 패딩은 눈에 보이지 않습니다.

  - 테두리(border) : 내용와 패딩 주변을 감싸는 테두리입니다.

  - 마진(margin) : 테두리와 이웃하는 요소 사이의 간격입니다. 마진은 눈에 보이지 않습니다.
- <img src="./img/boxModel.png" height="180px"></img><br/>

# CSS selector
- id
  - ```
      <p id="idName">hello my world!<p/>
    ```
  - ```
      #idName{
        ...
      }
    ```
- class
  - ```
      <p class="className">hello my world!<p/>
    ```
  - ```
      .className{
        ...
      }
    ```
- tag
  - ```
      <p>hello my world!<p/>
    ```
  - ```
      p{
        ...
      }
    ```
- 더 많은 css selector를 공부하고 싶다면
  - Link: https://flukeout.github.io/


# CSS selector 우선순위
- id > class > tag
  - ```
      <p class="className" id="idName">hello my world!<p/>
    ```
  - ```
      .className{
        font-style: italic;
        color: blue;
      }

      #idName{
        color: red;
      }
    ```
  - <img src="./img/selector.png" height="90px"></img><br/>
    - 겹치는 속성만 우선순위로 결정되고 나머지 부분들은 적용이 된다.
------------------------------
------------------------------
- 예시 사이트 : https://zktm9903.github.io/studyHTML-CSS/myHTML
  - html file 경로 = ./myHTML.html
  - css file 경로 = ./css/myCSS.css
