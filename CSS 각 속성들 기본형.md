## CSS 각 속성들 기본형

**텍스트를 표현하는 다양한 속성들**

1. 글꼴을 지정하는 font-family 속성

   ```css
   font-family: <글꼴 이름> | [<글꼴 이름], [글꼴 이름]>
   ```

   

2. 이탤릭체로 글자를 표시하는 font-style 속성

   ```css
   font-style: normal | italic | oblique
   ```



3. 글자 굴기를 지정하는 font-weight 속성

   ```css
   font-weight: normal | bold | bolder | lighter | 100~900 
   ```

   

4. 글자색을 지정하는 color 속성

   ```css
   color: <색상>
   ```

   

5. 텍스트를 지정하는 text-align 속성

   ```css
   text-align: start | end | left | right | center | justify | match-parent
   ```



6. 줄 간격을 조절하는 line-height 속성

   ```css
   line-height: npx;
   ```





7. 텍스트의 줄을 표시하거나 없애 주는 text-decoration 속성

   ```css
   text-decoration: none | underline | overline | line-through
   ```

   `none`: 텍스트에 줄을 표시하지 않음

   `underline`: 밑줄 표시

   `overline`: 윗줄 표시

   `line-through`: 취소선 표시



8. 텍스트에 그림자 효과를 추가하는 text-shadow 속성

```css
text-shadow: none | <가로 거리> <세로 거리> <번짐 정도> <색상>
```



9. 텍스트의 대소 문자를 변환하는 text-transform 속성

```css
text-transform: none | capitalize | uppercase | lowercase | full-width
```

`none`: 줄을 표시하지 않는다.

`capitalize`: 첫 번째 글자를 대문자로 변환한다.

`uppercase`: 모든 글자를 대문자로 변환한다.

`lowercase`: 모든 글자를 소문자로 변환한다.

`full-width`: 가능한 한 모든 문자를 전각 문자로 변환한다.



10. 글자 간격을 조절하는 letter-spacing, word-spacing 속성

    ```css
    letter-spacing: nem, npx, n%     word-spacing: nem, npx, n%`
    ```



11. 불릿 모양과 번호 스타일을 지정하는 list-style-type 속성

    ```css
    list-style-type: disc | circle | square | decimal | decimal-leading-zero | lower-roman | upper-roman | lower-alpha | upper-alpha | none
    ```

    `disc`: 채운 원 모양

    `circle`: 빈 원 모양

    `square`: 채운 사각형 모양

    `decimal`: 1부터 시작하는 10진수

    `decimal-leading-zero`: 앞에 0이 붙는 10진수

    `lower-roman`: 로마 숫자 소문자

    `upper-roman`: 로마 숫자 대문자

    `lower-alpha 또는 lower-latin`: 알파벳 소문자

    `upper-alpha 또는 upper-latin`: 알파벳 대문자

    `none`: 불릿이나 숫자를 없앰





12. 불릿 대신 이미지를 사용하는 list-style-image 속성

    ```css
    list-style-image: <url(이미지 파일 경로)> | none
    ```




13. 목록을 들여 쓰는 list-style-position 속성

    ```css
    list-style-position: inside | outside;
    ```

    `inside`: 불릿이나 번호를 기본 위치보다 안으로 들여쓴다.

    `outside`: 기본값



14. 표 제목의 위치를 정해주는 caption-side 속성

    ```css
    caption-side: top | bottom
    ```

    `top`: 캡션을 표 윗부분에 표시한다. 기본값

    `bottom`: 캡션을 표 아랫부분에 표시한다.



15. 표에 테두리를 그려주는 border 속성

    ```css
    border: <픽셀 크기> <선 너비> | <선 모양> <선 색상>
    ```



16. 셀 사이의 여백을 지정하는 border-spacing 속성

    ```css
    border-spacing: 수평거리 수직거리
    ```

    

17. 표와 셀 테두리를 합쳐 주는 border-collapse 속성

    ```css
    border-collapse: collapse | separate
    ```

    `collapse`: 표와 셀의 테두리를 합쳐 하나로 표시한다.

    `separate`: 표와 셀 테두리르 따로 표시한다. 기본값



**레이아웃을 구성하는 CSS 박스모델**

18. 박스 모델에 그림자 효과를 주는 box-shadow 속성

    ```css
    box-shadow: <수평 거리> <수직 거리> <흐림 정도> <번짐 정도> <색상> inset
    ```

    `<수평 거리>`: 그림자가 가로로 얼마나 떨어져 있는지를 나타냄. 양수값은 요소의 오른쪽에, 음수값은 요소의 왼쪽에 그림자를 만듦. 필수 속성이다.

    `<수직 거리>`: 그림자가 세로로 얼마나 떨어져 있는지를 나타낸다. 양수값과 음수값의 기준은 수평 거리와 동일하다. 필수 속성이다.

    `<흐림 정도>`: 이 값을 생략하면 0을 기본값으로 하여 진한 그림자를 표시한다. 

    `<번짐 정도>`: 양수값을 사용하면 모든 방향으로 그림자가 퍼져서 박스보다 그림자가 크게 표시된다. 반대로 음수값은 모든 방향으로 그림자가 축소되어 

    보인다. 기본값은 0이다.

    `<색상>`: 한 가지만 지정할 수도 있고, 공백으로 구분해서 여러개의 색상을 지정할 수도 있다. 기본값은 현재 검은색이다.

    `inset`: 이 키워드를 함께 표시하면 안쪽 그림자로 그린다.



19. 테두리 스타일을 지정하는 border-style 속성

    ```css
    border-style: none | hidden | solid | dotted | dashed | double | groove | inset | outset | ridge
    ```

    `none`: 테두리가 없다. 기본값이다.

    `hidden`: 테두리를 감춘다. 표에서 border-collapse: collapse일 경우 다른 테두리도 표시되지 않는다.

    `solid`: 테두리를 실선으로 표시한다.

    `dotted`: 테두리를 점선으로 표시한다.

    `dashed`: 테두리를 짧은 직선으로 표시한다.

    `double`: 테두리를 이중선으로 표시한다. 두 선 사이의 간격이 border-width값이 된다.

    `groove`: 테두리를 창에 조각한 것처럼 표시한다. 홈이 파인 듯 입체 느낌이 난다.

    `inset`: 표에서 border-collapse: seperate일 경우 전체 박스 테두리가 창에 박혀 있는 것처럼 표시되고, 표에서 border-collapse: collapse일 경우 groove와 똑같이 표시된다.

    `outset`: 표에서 border-collapse: seperate일 경우 전체 박스 테두리가 창에서 튀어 나온 것처럼 표시되고, 표에서 border-collapse: collapse일 경우 ridge와 똑같이 표시된다.

    `ridge`: 테두리를 창에서 튀어나온 것처럼 표시함.



20. 테두리 두께를 지정하는 border-width 속성

    ```css
    border-width: <크기> | thin | medium | thick
    ```

    `thin`: 테두리 두께를 얇게 지정한다.

    `medium`: 테두리 두께를 보통으로 지정한다.

    `thick`: 테두리 두께를 두껍게 지정한다.



21. 둥근 테두리를 만드는 border-radius 속성

    ```css
    border-radius: <크기> | <백분율>
    ```

    `<크기>`: 반지름 크기를 px, em의 단위와 함께 수치로 표시한다.

    `<백분율>`: 현재 요소의 크기를 기준으로 비율(%)로 지정한다.



22. 요소 주변의 여백을 설정하는 margin 속성

    ```css
    margin: <크기> | <백분율> | auto
    ```

    `<크기>`: 너비값이나 높이값을 px이나 em 같은 단위와 함께 수치로 지정한다.  예시-> `margin: 50px;`

    `<백분율>`: 박스 모델을 포함한 부모 요소를 기준으로 너비값이나 높이값을 퍼센트(%)로 지정한다.  예시-> `margin: 0.1%;`

    `auto`: display 속성에서 지정한 값에 맞게 적절한 값을 자동으로 지정한다.  



23. 배치 방법을 결정하는 display 속성

    ```css
    display: block | inline | inline-block | none
    ```

    `block`: 인라인 레벨 요소를 블록 레벨 요소로 만든다.

    `inline`: 블록 레벨 요소를 인라인 레벨 요소로 만든다.

    `inline-block`: 인라인 레벨 요소와 블록 레벨 요소의 속성을 모두 가지고 있으며 마진과 패딩을 지정할 수 있다.

    `none`: 해당 요소를 화면에 표시하지 않는다.



24. 왼쪽이나 오른쪽으로 배치하는 float 속성

    ```css
    float: left | right | none
    ```

    `left`: 해당 요소를 문서의 왼쪽에 배치한다.

    `right`: 해당 요소를 문서의 오른쪽에 배치한다.

    `none`: 좌우 어느 쪽에도 배치하지 않는다. 기본값이다.



25. float 속성을 해제하는 clear 속성

    ```css
    clear: left | right | both
    ```

    `left`: `float: left` 를 해제한다.

    `right`: `float: right` 를 해제한다.

    `both`: `float: left` 와 `float: right` 를 해제한다.



26. 웹 요소의 위치를 정하는 left, right, top, bottom 속성

    ```css
    left: <크기>
    right: <크기>
    top: <크기>
    bottom: <크기>
    ```

    `left`: 기준 위치와 요소 사이에 왼쪽으로 얼마나 떨어져 있는지 지정한다.

    `right`: 기준 위치와 요소 사이에 오른쪽으로 얼마나 떨어져 있는지 지정한다.

    `top`: 기준 위치와 요소 사이에 위쪽으로 얼마나 떨어져 있는지 지정한다.

    `bottom`: 기준 위치와 요소 사이에 아래쪽으로 얼마나 떨어져 있는지 지정한다.



27. 배치 방법을 지정하는 position 속성

    ```css
    position: static | relative | absolute | fixed
    ```

    `static`: 문서의 흐름에 맞춰 배치한다. 기본값이다.

    `relative`: 위치값을 지정할 수 있다는 점을 제외하면 `static` 과 같다.

    `absolute`: `relative` 값을 사용한 상위 요소를 기준으로 위치를 지정해 배치한다.

    `fixed`: 브라우저 창을 기준으로 위치를 지정해 배치한다.



28. 배경색의 적용 범위를 조절하는 background-clip 속성

    ```css
    background-clip: border-box | padding-box | content-box
    ```

    `border-box`: 박스 모델의 가장 외곽인 테두리까지 적용한다. 기본값이다.

​       `padding-box`: 박스 모델에서 테두리를 뺀 패딩 범위까지 적용한다.

​       `content-box`: 박스 모델에서 내용(콘텐츠) 부분에만 적용한다.



29. 웹 요소에 배경 이미지를 넣는 background-image 속성

    ```css
    background-image: url('이미지 파일 경로')
    ```



30. 배경 이미지의 반복 방법을 지정하는 background-repeat 속성

    ```css
    background-repeat: repeat | repeat-x | repeat-y | no-repeat
    ```

    `repeat`: 브라우저 화면에 가득 찰 때까지 가로와 세로로 반복한다. 기본값이다.

    `repeat-x`: 브라우저 화면 너비에 가득 찰 때까지 가로로 반복한다.

    `repeat-y`: 브라우저 화면 높이에 가득 찰 때까지 세로로 반복한다.

    `no-repeat`: 한 번만 표시하고 반복하지 않는다.



31. 배경 이미지의 위치를 조절하는 background-position 속성

    ```css
    background-position: <수평 위치> | <수직 위치>;
    수평 위치: left | center | right | <백분율> | <길이 값>
    수직 위치: top | center | bottom | <백분율> | <길이 값>
    ```

    

32. 배경 이미지의 적용 범위를 조절하는 background-origin 속성

    ```css
    background-origin: content-box | padding-box | border-box
    ```

    `content-box`: 박스 모델에서 내용 부분에만 배경 이미지를 표시한다. 기본값이다.

    `padding-box`: 박스 모델에서 패딩까지 배경 이미지를 표시한다.

    `border-box`: 박스 모델에서 테두리까지 배경 이미지를 표시한다.



33. 배경 이미지를 고정하는 background-attachment 속성

    ```css
    background-attachment: scroll | fixed
    ```

    `scroll`: 화면을 스크롤하면 배경 이미지도 스크롤된다. 기본값이다.

    `fixed`: 화면을 스크롤하면 배경 이미지는 고정되고 내용만 스크롤된다.



34. 배경 이미지 크기를 조절하는 background-size 속성

    ```css
    background-size: auto | contain | cover | <크기> | <백분율>
    ```

    `auto`: 원래 배경 이미지 크기만큼 표시한다. 기본값이다.

    `contain`: 요소 안에 배경 이미지가 다 들어오도록 이미지를 확대/축소한다.

    `cover`: 배경 이미지로 요소를 모두 덮도록 이미지를 확대/축소한다.

    `<크기>`: 이미지의 너비와 높이를 지정한다. 값이 하나만 주어질 경우 너비값으로 인식하며, 이미지의 너비와 너비값에 맞춘 높이값도 자동 계산한다.

    `<백분율>`: 배경 이미지가 들어갈 요소의 크기를 기준으로 값을 백분율로 지정하고 그 크기에 맞도록 배경 이미지를 확대/축소한다.



35. 선형 그러데이션을 만들어주는 linear-gradient 속성

    ```css
    linear-gradient(to <방향> 또는 <각도>, <색상 중지점>, [<색상 중지점>, ......])
    ```

    
