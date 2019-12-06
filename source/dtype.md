Intro
=====

파이썬으로 데이터를 다루기 위해 가장 기본적으로 알아야 하는 것이
데이터의 형태입니다. 데이터는 숫자, 문자, 배열, 집합, 순서쌍 등 다양한
형태를 가질 수 있습니다. 파이썬에는 몇 가지 기본적인 자료형들이 정의되어
있으며, 각각의 자료형마다 다른 연산과 조작을 할 수 있습니다. 이번 장의
목표는 **내가 다루는 데이터가 어떤 형태인지를 알고, 자료형에 맞는 연산과
조작을 할 수 있는 능력**을 키우는 것입니다.

기본적인 파이썬 자료형
----------------------

다음은 파이썬에서 사용되는 기본적인 자료형들의 예시입니다. 자세한 내용은
앞으로 차근차근 다룰 예정이니 눈으로만 봐두시면 됩니다. \# 표시가 붙은
부분은 코드에 대한 주석으로, 실제 실행되는 파이썬 코드가 아닙니다.

    # 1. 숫자: 정수와 소수
    365 # 정수
    3.14 # 소수
    1.25 #소수

    # 2. 문자열: 따옴표로 감싼 문자들의 배열
    'Hello world!'
    "DataScience Lab"

    # 3. 불(bool): 참거짓
    True
    False

    # 4. 리스트: 대괄호 []로 감싼 배열
    [1.1, 2.2, 3.3, 4.4, 5.5]
    ["a","b","c","d"]

    # 5. 튜플: 소괄호 ()로 감싼 배열
    (1,2,3,4,5)
    (True,False,False,True)

    # 6. 딕셔너리: 중괄호 {}로 감싼 키:값
    {"김연아":"피겨", "손흥민":"축구", "박찬호":"야구"}
    {1:"짜장면", 2:"짬뽕"}

기본적인 함수와 연산자
----------------------

다음은 간단한 함수들과 연산자들입니다. 앞으로도 계속 사용할
명령어들이므로 꼭 직접 코딩해보시기 바랍니다. 특히, 비교연산자 `==`와
할당연산자 `=`의 차이에 유의하세요! 할당연산자 `=`는 두 대상이 같은지
비교하는 연산자가 아니라, 변수에 값을 할당하는 할당연산자입니다. **즉
`a=5`은 “a는 5와 같다”가 아니라, “a에 5를 할당하라”는 명령입니다!**

<table>
<thead>
<tr class="header">
<th>함수/연산자</th>
<th>기능</th>
<th>예시 코드</th>
<th>실행결과</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>print()</code></td>
<td>대상을 출력</td>
<td><code>print("Hello world!")</code></td>
<td><code>Hello world!</code></td>
</tr>
<tr class="even">
<td><code>type()</code></td>
<td>대상의 자료형을 반환</td>
<td><code>type(5)</code></td>
<td><code>int'</code></td>
</tr>
<tr class="odd">
<td><code>==</code></td>
<td>“두 대상이 같다”를 판단</td>
<td><code>'Python'=='R'</code></td>
<td><code>False</code></td>
</tr>
<tr class="even">
<td><code>!=</code></td>
<td>“두 대상이 같지 않다”를 판단</td>
<td><code>'Python'!='R'</code></td>
<td><code>True</code></td>
</tr>
<tr class="odd">
<td><code>=</code></td>
<td>왼쪽 변수에 오른쪽 값을 할당</td>
<td><code>a=5</code></td>
<td></td>
</tr>
</tbody>
</table>

1. 숫자
=======

1.1. 정수와 소수
----------------

파이썬의 숫자는 **정수**와 **소수**로 나뉘며, 각각 **`int`**와
**`float`**으로 표기합니다. 아래는 정수 `2`와 소수 `3.14`의 자료형을
확인하는 코드와 결과입니다. `2`의 자료형은 `int`, `3.14`의 자료형은
`float`임을 확인할 수 있습니다.

    type(2)

    ## <class 'int'>

    type(3.14)

    ## <class 'float'>

1.2 파이썬으로 계산하기
-----------------------

숫자들 간에는 정수와 소수 구분 없이 다음의 연산이 가능합니다.
번거롭더라도 최소한 사칙연산 코드는 따라 쳐보면서 파이썬에 익숙해지시기
바랍니다! 사칙연산을 제외한 연산자들은 사용하는 빈도가 많지 않으니, 이런
연산이 있다고만 알아두시면 됩니다.

<table>
<thead>
<tr class="header">
<th>연산자</th>
<th>기능</th>
<th>예시 코드</th>
<th>실행결과</th>
<th>결과의 자료형</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>a + b</code></td>
<td>덧셈</td>
<td><code>1+1</code></td>
<td><code>2</code></td>
<td><code>int</code></td>
</tr>
<tr class="even">
<td><code>a - b</code></td>
<td>뺄셈</td>
<td><code>3-2.5</code></td>
<td><code>0.5</code></td>
<td><code>float</code></td>
</tr>
<tr class="odd">
<td><code>a * b</code></td>
<td>곱셉</td>
<td><code>2*4.5</code></td>
<td><code>9.0</code></td>
<td><code>float</code></td>
</tr>
<tr class="even">
<td><code>a / b</code></td>
<td>나눗셈</td>
<td><code>0.9/0.3</code></td>
<td><code>3.0</code></td>
<td><code>float</code></td>
</tr>
<tr class="odd">
<td><code>a // b</code></td>
<td>나눗셈의 몫</td>
<td><code>8//3</code></td>
<td><code>2</code></td>
<td><code>int</code></td>
</tr>
<tr class="even">
<td><code>a % b</code></td>
<td>나눗셈의 나머지</td>
<td><code>8%3</code></td>
<td><code>2</code></td>
<td><code>int</code></td>
</tr>
<tr class="odd">
<td><code>a ** b</code></td>
<td>a의 b제곱</td>
<td><code>5**2</code></td>
<td><code>25</code></td>
<td><code>int</code></td>
</tr>
</tbody>
</table>

**덧셈**

    print(1+1)

    ## 2

**뺄셈**

    print(3 - 2.5)

    ## 0.5

**곱셈**

    print(2 * 4.5)

    ## 9.0

**나눗셈**

    print(0.9/ 0.3)

    ## 3.0

2. 문자열
=========

2.1. Hello World
----------------

문자열은 말 그대로 문자들의 나열을 의미하며, `str`로 표기합니다. 작은
따옴표(`''`), 혹은 큰 따옴표(`""`) 안에 원하는 내용을 적어주면 문자열
데이터를 만들 수 있습니다. 둘 중 무엇을 사용하든 상관은 없습니다.
프로그래밍 언어를 배울 때는 `"Hello World"`를 출력해보는 것이
관례입니다. 다같이 인사해보세요! `type("Hello world")`을 실행해보면
`"Hello world"`의 자료형이 문자열(`str`)임을 확인할 수 있습니다.

    print("Hello world")

    ## Hello world

    type("Hello world")

    ## <class 'str'>

숫자도 따옴표로 감싸면 문자열이 됩니다. `type("365")`를 실행해본 결과
`"365"`는 문자열 데이터입니다. 문자열 `"365"`와 숫자 `365`가 같은지
테스트해보면 결과는 ‘같지 않다’ 입니다. `"365"`는 문자열이고, `365`는
숫자이기 때문입니다.

    type("365")

    ## <class 'str'>

    365 == "365" # 365 는 "365"와 같다: 거짓이므로 False를 반환합니다.

    ## False

2.2. 인덱싱 & 슬라이싱
----------------------

문자열은 **문자를 순서대로 나열한 데이터입니다.** 따라서 문자열을
구성하는 하나하나의 문자에 순서대로 번호를 매길 수 있으며, 이 번호를
**인덱스**라고 부릅니다. 아래 그림은 `"Hello World"`라는 문자열에
앞쪽부터 번호를 매긴 결과입니다. 파이썬의 인덱스는 0부터 시작하기
때문에, 가장 먼저 나온 문자인 `"H"`의 인덱스는 `0`이 됩니다. 그 이후
순차적으로 1, 2, … 10 까지의 번호가 매겨졌습니다. 공백 역시 문자열에
포함된다는 사실을 유의해주세요!

<table>
<thead>
<tr class="header">
<th>인덱스</th>
<th>0</th>
<th>1</th>
<th>2</th>
<th>3</th>
<th>4</th>
<th>5</th>
<th>6</th>
<th>7</th>
<th>8</th>
<th>9</th>
<th>10</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>문자열</td>
<td>H</td>
<td>e</td>
<td>l</td>
<td>l</td>
<td>o</td>
<td></td>
<td>w</td>
<td>o</td>
<td>r</td>
<td>l</td>
<td>d</td>
</tr>
</tbody>
</table>

파이썬의 인덱스는 뒤에서부터 부여할 수도 있습니다. `"Hello world"`의
인덱스를 뒤에서부터 매기면 다음과 같습니다. 즉 가장 뒤에서부터 `-1`,
`-2`, … 와 같이 음수 인덱스가 매겨집니다.

<table>
<thead>
<tr class="header">
<th>인덱스</th>
<th>-11</th>
<th>-10</th>
<th>-9</th>
<th>-8</th>
<th>-7</th>
<th>-6</th>
<th>-5</th>
<th>-4</th>
<th>-3</th>
<th>-2</th>
<th>-1</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>문자열</td>
<td>H</td>
<td>e</td>
<td>l</td>
<td>l</td>
<td>o</td>
<td></td>
<td>w</td>
<td>o</td>
<td>r</td>
<td>l</td>
<td>d</td>
</tr>
</tbody>
</table>

### 인덱싱

문자열에 부여된 **인덱스를 통해서 개별 문자를 뽑아낼 수 있고, 이것을
인덱싱이라고 합니다.** 비유하면, 여러분과 파이썬이 다음과 같은 대화를
한다고 생각하시면 됩니다.

> You: `"Hello world"`의 0번 문자를 찾아줘!
>
> Python: `"Hello world"`의 0번 문자는 `"H"` 입니다.

그렇다면 `"Hello world"`의 0번 문자를 찾아줘!’라는 명령을 어떻게
파이썬에 전달할 수 있을까요? 문자열 바로 뒤에 대괄호`[]`를 적고, 대괄호
안에 원하는 인덱스 숫자를 넣어주면 됩니다. 실제 파이썬 코드를 실행하면
다음과 같은 결과를 얻을 수 있습니다. 예시 코드들을 따라 쳐보면서
인덱싱의 문법에 익숙해지시기 바랍니다. 실행 결과의 자료형은 당연하게도
문자열입니다!

    "Hello world"[0]

    ## 'H'

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>문자열</th>
<th>인덱스</th>
<th>예시 코드</th>
<th>결과</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>"Python"</code></td>
<td>0</td>
<td><code>"Python"[0]</code></td>
<td><code>'P'</code></td>
</tr>
<tr class="even">
<td><code>"DataScience Lab"</code></td>
<td>12</td>
<td><code>"DataScience Lab"[12]</code></td>
<td><code>'L'</code></td>
</tr>
<tr class="odd">
<td><code>"010-5782-3579"</code></td>
<td>7</td>
<td><code>"010-5782-3579"[7]</code></td>
<td><code>'2'</code></td>
</tr>
<tr class="even">
<td><code>"Life is short, you need Python."</code></td>
<td>-1</td>
<td><code>"Life is short, you need Python."[-1]</code></td>
<td><code>'.'</code></td>
</tr>
</tbody>
</table>

### 슬라이싱

슬라이싱은 말 그대로 잘라내기 입니다. 일정 구간에 걸쳐서 인덱싱을
실행한다고 생각하시면 편합니다. 역시 대화로 표현하면 다음과 같습니다.

> You: `"Hello world"`의 0번부터 4번까지의 문자를 찾아줘!
>
> Python: `"Hello world"`의 0번부터 4번까지 문자는 `"Hello"` 입니다.

슬라이싱을 할 때는, `[a:b]`와 같이 대괄호 안에 구간을 입력해주면 됩니다.
구간을 입력할 때는 주의사항이 있습니다. 예시와 함께 보겠습니다.

    "Hello world"[0:4]

    ## 'Hell'

`[0:4]`의 구간을 입력했으므로 0, 1, 2, 3, 4번 문자가 출력되어야 할 것
같은데, 이상하게 `'Hell'`까지만 출력되었습니다. 이는 슬라이싱에서 구간
`[a:b]`가 `a` 이상 `b` 미만으로 해석되기 때문입니다. 즉 0번부터
4번까지를 슬라이싱 하려면 구간을 `[0:5]`와 같이 입력해야 합니다. 코드를
수정하면 정상적으로 실행되는 것을 볼 수 있습니다.

    "Hello world"[0:5]

    ## 'Hello'

슬라이싱의 구간 표현법을 정리하면 다음과 같습니다.

<table>
<thead>
<tr class="header">
<th>구간</th>
<th>설명</th>
<th>예시 코드</th>
<th>실행 결과</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>[a:b]</code></td>
<td><code>a</code>번 문자부터 <code>b</code>번 문자 직전까지 슬라이싱</td>
<td><code>'www.naver.com'[4:9]</code></td>
<td><code>'naver'</code></td>
</tr>
<tr class="even">
<td><code>[:]</code></td>
<td>문자열의 전 구간을 슬라이싱</td>
<td><code>"Super Awesome Code"[:]</code></td>
<td><code>'Super Awesome Code'</code></td>
</tr>
<tr class="odd">
<td><code>[a:]</code></td>
<td><code>a</code>번 문자부터 끝까지 슬라이싱</td>
<td><code>"Avengers: Endgame"[-7:]</code></td>
<td><code>'Endgame'</code></td>
</tr>
<tr class="even">
<td><code>[:b]</code></td>
<td>처음부터 <code>b</code>번 문자 직전까지 슬라이싱</td>
<td><code>"서울특별시 서대문구"[:5]</code></td>
<td><code>'서울특별시'</code></td>
</tr>
</tbody>
</table>

2.3. 문자열의 메소드
--------------------

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>메소드</th>
<th>기능</th>
<th>예시</th>
<th>결과</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>strip()</code></td>
<td>문자열 양쪽의 공백을 제거</td>
<td><code>"     Hello world      ".strip()</code></td>
<td><code>"Hello world"</code></td>
</tr>
<tr class="even">
<td><code>replace()</code></td>
<td>문자열 내의 특정 문자를 다른 문자로 교체</td>
<td><code>"You need Python".replace("Python", "R")</code></td>
<td><code>"You need Python"</code></td>
</tr>
<tr class="odd">
<td><code>split()</code></td>
<td>특정 문자를 기준으로 문자열을 쪼갬</td>
<td><code>"one,two,three,four".split(",")</code></td>
<td><code>['one','two','three','four]</code></td>
</tr>
<tr class="even">
<td><code>join()</code></td>
<td>특정 문자열을 삽입</td>
<td><code>"/".join("ABCDE")</code></td>
<td><code>"A,B,C,D,E"</code></td>
</tr>
</tbody>
</table>

메소드는 일종의 함수이며, 대상 뒤에 점 `.`을 찍고 사용할 수 있습니다.
문자열에 사용하는 대표적인 메소드들을 네 가지만 배워 보겠습니다.

### **strip()**

**`strip()` 메소드는 문자열 양쪽의 공백을 개수에 상관없이 모두
제거합니다. 원하는 문자열 뒤에 점을 찍어서 `"문자열".strip()`과 같이
적어주면 됩니다. ** 문자열 `"   Hello world   "`는 양쪽에 공백이 있고,
가운데에도 한 칸의 공백이 있습니다. `"   Hello world   "`를 변수 `s`에
할당하고, `s.strip()`을 실행한 결과, 양쪽의 공백만 지워지고 가운데
공백은 잘 남아있는 것을 확인할 수 있습니다.

    s = "   Hello world   "
    s.strip()

    ## 'Hello world'

사실 `s.strip()`은 `s`를 실제로 변화시키지는 않으며, 변화한 상태를
일시적으로 보여줄 뿐입니다. `s`를 출력해보면 양쪽의 공백이 그대로
남아있습니다. 공백을 제거한 결과를 `s`에 저장하고 싶다면,
`s=s.strip()`과 같이 다시 할당을 해주어야 합니다. 처음 `s = s.strip()`과
같은 식을 마주하면 당황스러울 것입니다. 하지만 `=`는 같음을 뜻하는
연산자가 아니고, 할당을 뜻하는 연산자입니다. 즉 `s=s.strip()`이라는
코드는 **“`s.strip()`을 실행하고 이 결과를 `s`에 할당하라”**는
의미입니다.

    s

    ## '   Hello world   '

    s = s.strip() # s.strip()을 실행하고 이 결과를 s에 할당하라
    s

    ## 'Hello world'

**탭을 의미하는 `\t` 문자열과 개행을 의미하는 `\n` 문자열 역시 공백으로
인식됩니다.** `\t` 와 `\n`을 사용한 공백은 웹 문서를 크롤링해서 작업할
때 자주 볼 수 있습니다. 아래 예제에서는 왼쪽에 `\n`, 오른쪽에 `\t` 세
개를 사용해서 `'Hello world'`를 감싸주었습니다. 이 결과를 변수 `s`에
할당하고 `s.strip()`을 실행한 결과, `'Hello world'`만 남아있는 것을
확인할 수 있습니다. `\t`와 `\n`이 공백으로 인식되어 지워졌기 때문입니다.

    s = "\n\n\nHello world\t\t\t"
    s = s.strip() 
    print(s)

    ## Hello world

### **replace()**

**`replace()` 메소드는 문자열 내의 특정 문자를 다른 문자로 모두
교체합니다. `s.replace("교체할 문자","새 문자")`와 같이 적어주면
됩니다.** 아래는 `"You need Python"` 에서 `"Python"`을 `"R"`로 바꾸어준
예제입니다. 먼저 `'You need Python'`라는 문자열을 `s`라는 변수에
할당하였습니다. `s.replace("Python","R")` 은 s에 할당된 문자열
`"You need Python"`에서 `'Python'`을 `'R'`로 바꾸어주는 코드입니다. 역시
`s.replace("Python","R")`를 실행하는것만으로는 `s`에 할당된 값이
변화하지 않으며, `s`를 변화시키고 싶다면 `s=s.replace("Python","R")`과
같이 다시 할당을 해주어야 합니다.

    s = 'You need Python' # 문자열을 변수 s에 할당
    s.replace("Python", "R") # s에서 Python -> R로 교체

    ## 'You need R'

    s # s는 변화하지 않음

    ## 'You need Python'

    s = s.replace("Python", "R") # Python을 R로 교체한 후 이 결과를 s에 할당
    s

    ## 'You need R'

    s = s.replace(" ", ",") # 모든 " "를 ","로 교체
    s 

    ## 'You,need,R'

### **split()**

**`split()` 메소드는 특정 문자를 기준으로 문자열을 쪼개어 리스트를
반환합니다. `s.split("기준문자")`와 같이 적어주면 됩니다.** 아무런
문자도 주어지지 않는다면 공백을 기준으로 문자열을 쪼갭니다. 역시 쪼갠
결과를 저장하려면 다시 할당을 해주어야 합니다.

    s = "Hello world"
    s.split(" ") # " " 를 기준으로 문자열을 쪼갬 > 이 결과를 리스트로 반환

    ## ['Hello', 'world']

    s = "one/two/three/four"
    s.split("/")

    ## ['one', 'two', 'three', 'four']

#### **join()**

**`join()` 메소드는 문자열 사이사이에 다른 문자를 삽입합니다. “삽입할
문자”.join(문자열)과 같이 적어주면 됩니다.** `join` 메소드는
문자열보다는 리스트에 대해 사용하는 경우가 많습니다. 이후 리스트를
다루면서 다시 한 번 언급하겠습니다.

    alphabet = "ABCDEFG"
    "|".join(alphabet)

    ## 'A|B|C|D|E|F|G'

3. 불리언
=========

불리언은 참/거짓을 나타내는 자료형이며, 각각 `True`, `False`로 씁니다.
크게 주의할 것은 없고, 파이썬에서 `0`이 `False`를 의미한다는 것은 알고
넘어가면 좋습니다.

    0 == False

    ## True

4. 리스트
=========

리스트는 `[요소1, 요소2, 요소3, ...]`과 같이 여러 요소들을 묶어놓은
자료형입니다. 각 요소들은 쉼표 `,`로 구분되며, 바깥은 대괄호 `[]`로
감싸줍니다. 리스트는 거의 모든 자료형을 요소로 가질 수 있으며, 요소들의
자료형이 모두 같을 필요도 없습니다. 다음은 모두 리스트의 예시입니다.

    [] # 빈 리스트
    [1,2,3,4,5] # 숫자 리스트
    ['a','b','c','d','e'] # 문자열 리스트
    ['a','b',3,4,'d',False] # 여러 자료형을 포함한 리스트
    [[1,2,3],[4,5,6]] # 리스트의 리스트

4.1. 리스트 인덱싱 & 슬라이싱
-----------------------------

리스트는 요소들의 순차적인 배열입니다. 따라서 문자열과 마찬가지로,
각각의 요소들에 번호를 매길 수 있습니다. 번호를 매기는 방식 역시
문자열과 동일합니다. 즉 앞에서부터 `0`, `1`, `2` … 순으로 인덱스가 붙고,
뒤에서부터 `-1`,`-2`,`-3` … 순으로 인덱스가 붙습니다. 예를 들어
`["Life", "is", "short", "you", "need", "Python"]` 과 같은 리스트에
인덱스를 매겨보면 다음과 같습니다.

<table>
<thead>
<tr class="header">
<th>인덱스</th>
<th>0</th>
<th>1</th>
<th>2</th>
<th>3</th>
<th>4</th>
<th>5</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>요소</td>
<td>“Life”</td>
<td>“is”</td>
<td>“short”</td>
<td>“you”</td>
<td>“need”</td>
<td>“Python”</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr class="header">
<th>인덱스</th>
<th>-6</th>
<th>-5</th>
<th>-4</th>
<th>-3</th>
<th>-2</th>
<th>-1</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>요소</td>
<td>“Life”</td>
<td>“is”</td>
<td>“short”</td>
<td>“you”</td>
<td>“need”</td>
<td>“Python”</td>
</tr>
</tbody>
</table>

### 인덱싱

문자열의 인덱싱과 슬라이싱에 익숙해졌다면, 리스트의 인덱싱과 슬라이싱
역시 어렵지 않을 겁니다. 리스트의 인덱싱 역시 문자열과 마찬가지로 대괄호
`[]`를 사용합니다.

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>리스트</th>
<th>인덱스</th>
<th>예시 코드</th>
<th>결과</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><code>[0.25, 0.5, 0.75, 1.0]</code></td>
<td>1</td>
<td><code>[0.25, 0.5, 0.75, 1.0][1]</code></td>
<td><code>0.5</code></td>
</tr>
<tr class="even">
<td><code>["You", "need", "Python"]</code></td>
<td>-1</td>
<td><code>["You", "need", "Python"][-1]</code></td>
<td><code>'Python'</code></td>
</tr>
<tr class="odd">
<td><code>[[1,2,3],[4,5,6],[7,8,9],[10,11,12]]</code></td>
<td>2</td>
<td><code>[[1,2,3],[4,5,6],[7,8,9],[10,11,12]][2]</code></td>
<td><code>[10,11,12]</code></td>
</tr>
</tbody>
</table>

    [0.25, 0.5, 0.75, 1.0][1]

    ## 0.5

    ["You", "need", "Python"][-1]

    ## 'Python'

    [[1,2,3],[4,5,6],[7,8,9],[10,11,12]][2]

    ## [7, 8, 9]

인덱싱을 사용하여 개별 요소를 추출하였다면, 해당 요소에 대해 다시
인덱싱이나 슬라이싱을 사용하는 것도 가능합니다. 아래는 리스트에서 개별
요소를 추출한 후, 해당 요소에 대해 다시 인덱싱/슬라이싱을 적용한
예제입니다.

    mylist = ["Life", "is", "short", "you", "need", "Python"] # 리스트 생성
    element = mylist[0] # 0번 요소인 "Life" 추출
    element[:2] # "Life"에서 2번 문자까지 슬라이싱

    ## 'Li'

    element[:2] == ["Life", "is", "short", "you", "need", "Python"][0][:2] # 위 과정을 붙여서 쓴 코드

    ## True

    mylist = [[1,2,3],[4,5,6],[7,8,9]] # 리스트 생성
    sublist = mylist[-1] # 마지막 요소인 [7,8,9] 추출
    sublist[2] # [7,8,9]에서 2번 문자 인덱싱

    ## 9

    sublist[2] == [[1,2,3],[4,5,6],[7,8,9]][-1][2] # 위 과정을 붙여서 쓴 코드

    ## True

### 슬라이싱

리스트 슬라이싱 역시 문자열 슬라이싱과 다르지 않습니다. 대괄호 안에
콜론을 써서 구간을 표현해주시면 됩니다.

    ['one', 'two', 'three', 'four', 'five'][:2]

    ## ['one', 'two']
