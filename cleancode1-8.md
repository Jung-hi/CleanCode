# INTRO
***
## 1. S5원칙
* 정리(Seiri) 또는 조직(정렬) : 적절한 명명법 등과 같은 방법을 사용해 무엇이 어디에 있는지 알아야 한다.
* 정돈(Seiton) 또는 단정함(체계화) : 코드는 누구나 예상하는 위치에 있어야 한다.
* 청소(Seiso) 또는 정리(광내기): 과거 이력이나 미래 바람을 기억한 주석 혹은 주석으로 처리한 코드는 정리한다.
* 청결(Seiketsu) 또는 표준화: 그룹 내에서 일관적인 구현 스타일과 기법의 필요성에 따라 정돈한다.
* 생활화(Shutsuke) 또는 규율: 관례를 따르고 본인의 코드를 돌아보고, 변경할 수 있어야한다. 작은 것에도 충실한 사람이 큰 것에도 충실하다.


## 2. 사소한 것에 정직해라
* 코드에 정직하고, 코드의 상태에 관하여 동료들에게 정직하고, 자기코드에 대해서 자신에게 정직해라.
## 3. 보이스카웃법칙
* 처음에 왔을 때보다 캠프장을 더 깨끗이 치우고 떠나라.   
　

# 1장. 깨끗한 코드
***
## 1. 나쁜 코드
* 기한을 맞추기 위해 나쁜코드를 양산하게 되면 개발속도를 크게 떨어트린다.   
(코드를 고칠 때마다 엉뚱한 곳에서 문제가 생김)
* 나쁜코드는 나쁜코드를 유혹한다 (깨진창문의 원리)

## 2. 깨끗한 코드
* 세세한 사항까지 꼼꼼하게 처리해야 한다. (메모리누수, 경쟁상태, 일관성 없는 명명법)
* 가독성이 좋아야 한다.   
 (눈에 잘들어오는 코드, 읽기 편한코드, 변수/함수/클래스 등이 어떤 역할을 갖고, 어떤 동작을 하며, 서로 어떤 관계를 맺는지 직관적으로 파악할 수 있는 코드)

## 3. 간단한 코드
* 모든 테스트를 통과한다
* 중복이 없다
* 시스템 내 모든 설계 아이디어를 표현한다
* 클래스, 메서드, 함수 등을 최대한 줄인다

## 4. 깨끗한 코드를 만드는 법
* 중복 피하기
* 한기능만 수행하기
* 제대로 표현하기
* 작게 추상화 하기   
　   
　   
　   


## <i><center>"깨끗한 코드란? 제3자가 읽기 쉽고, 고치기 쉬운 코드이다."</i></center>
　
　   

>
# 2장. 의미 있는 이름
***
## 1. 의도를 분명히 밝혀라
* 좋은 이름을 지으려면 시간이 걸리지만 좋은 이름으로 절약하는 시간이 훨씬 더 많다.
* 변수나 함수 그리고 클래스 이름은 다음과 같은 굵직한 질문에 모두 답해야 한다.
변수(혹은 함수나 클래스)의 존재 이유는? 수행 기능은? 사용 방법은?
따로 주석이 필요하다면 의도를 분명히 드러내지 못했다는 말이다.
* 의도가 드러나는 이름을 사용하면 코드 이해와 변경이 쉬워진다.

## 2. 그릇된 정보를 피하라
* 그릇된 단서는 코드 의미를 흐린다. 실제 List가 아니라면 xxxList라 명명하지 않는다.
* 유사한 개념은 유사한 표기법을 사용한다. 일관성이 떨어지는 표기법은 그릇된 정보다.
* 이름으로 그릇된 정보를 제공하는 진짜 끔찍한 예가 소문자 L이나 대문자 O 변수다. 소문자 L은 숫자 1처럼 보이고 대문자 O는 숫자 0cjfja qhdlsek.

## 3. 의미있게 구분하라
* 컴파일러나 인터프리터만 통과하려는 생각으로 코드를 구현하는 프로그래머는 스스로 문제를 일으킨다.
* 컴파일러를 통과할지라도 연속된 숫자를 덧붙이거나 불용어(noise word)를 추가하는 방식은 적절하지 못한다. 이름이 달라야 한다면 의미도 달라져야 한다.
* 불용어를 추가한 이름 역시 아무런 정보도 제공하지 못한다.
  * Product라는 클래스가 있다고 가정
  * 다른 클래스를 ProductInfo 혹은 ProductData라 부른 다면 개념을 구분하지 않은 채 이름만 달리한 경우다.
  * Info나 Data는 a, an, the와 마찬가지로 의미가 불분명한 불용어다.
* 불용어는 중복이다.
  * NameString이 Name보다 뭐가 나은가?
  * Customor라는 클래스와 CustomerObject라는 클래스를 발견했다면 차이를 알겠는가? 고객 급여 이력을 찾으려면 어느 클래스를 뒤져야 빠를까?
  읽는 사람이 차이를 알도록 이름을 지어라.
  
## 4. 발음하기 쉬운 이름을 사용하라
* 발음하기 어려운 이름은 토론하기도 어렵다. 발음하기 쉬운 이름은 중요하다. 프로그래밍은 사회 활동이기 때문이다.

## 5. 검색하기 쉬운 이름을 사용하라
* 문자 하나를 사용하는 이름과 상수는 텍스트 코드에서 쉽게 눈에 띄지 않는다는 문제점이 있다.
  * MAX_CLASSES_PER_STUDENT는 grep으로 찾기가 쉽지만, 숫자 7은 은근히 까다롭다.
  * 7이 들어가는 파일 이름이나 수식이 모두 검색되기 때문이다.
  * 검색은 되었지만 7을 사용한 의도가 다른 경우도 있다.
* 개인적으로는 간단한 메서드에서 로컬 변수만 한 문자를 사용한다.
* 이름 길이는 범위 크기에 비례해야 한다. 변수나 상수를 코드 여러 곳에서 사용한다면 검색하기 쉬운 이름이 바람직하다.

## 6. 인코딩을 피하라
* 굳이 부담을 더하지 않아도 이름에 인코딩할 정보는 아주 많다.
* 유형이나 범위 정보까지 인코딩에 넣으면 그만큼 이름을 해독하기 어려워진다.
#### 　(1) 헝가리식 표기법 → 객체는 강한 타입이며 IDE는 코드를 컴파일하지 않고도 타입 오류를 감지할 정도로 발전했다. 따라서 이제는 헝가리식 표기법이나 기타 인코딩 방식이 오히려 방해가 될 뿐이다.
#### 　(2) 멤버 변수 접두어 → 클래스와 함수는 접두어가 필요없을 정도로 작아야 마땅하다. 또한 멤버 변수를 다른 색상으로 표시하거나 눈에 띄게 보여주는 IDE를 사용해야 마땅하다.
#### 　(3) 인터페이스 클래스와 구현 클래스 → 때로는 인코딩이 필요한 경우. 인터페이스 클래스 이름과 구현 클래스 이름 중 하나를 인코딩해야 한다면 구현 클래스 이름을 택하겠다.

## 7. 자신의 기억력을 자랑하지 마라
* 전문가 프로그래머는 명료함이 최고라는 사실을 이해한다. 프로그래는 자신의 능력을 좋은 방향으로 사용해 남들이 이해하는 코드를 내놓는다.

## 8. 클래스 이름
* 클래스 이름과 객체 이름은 명사나 명사구가 적합하다.

## 9. 메서드 이름
### 1) 메서드 이름은 동사나 동사구가 적합하다.
### 2)생성자를 overload할 때는 정적 팩토리 메서드를 사용한다.
#### (1)정적 팩토리 메서드 : 객체 생성의 역할을 하는 클래스(https://tecoble.techcourse.co.kr/post/2020-05-26-static-factory-method/)
#### (2)생성자 대신 정적 팩토리 메서드를 사용하면 메서드 이름에 객체의 생성 목적을 담아낼 수 있다.
#### (3)정적 팩터리 메서드와 캐싱구조를 함께 사용하면 매번 새로운 객체를 생성할 필요가 없어진다.
#### (4)상속을 사용할 때 하위 자료형 객체를 반환할 수 있다. Basic, Intermediate, Advanced 클래스가 Level라는 상위 타입을 상속받고 있는 구조를 생각해보자. 시험 점수에 따라 결정되는하위 등급 타입을 반환가능하다.

## 10. 기발한 이름은 피하라
* 재미난 이름보다 명료한 이름을 선택하라.
* 의도를 분명하고 솔직하게 표현하라.

## 11. 한 개념에 한 단어를 사용하라
* 추상적인 개념 하나에 단어 하나를 선택해 이를 고수한다. 예를 들어, 똑같은 메서드를 클래스마다 fetch, retrice, get으로 제각각 부르면 혼란스럽다.
* 일관성 있는 어휘는 코드를 사용할 프로그래머가 반갑게 여길 선물이다.

## 12. 말장난을 하지 마라
* 한 단어를 두 가지 목적으로 사용하지 마라. 다른 개념에 같은 단어를 사용한다면 그것은 말장난에 불과하다.

## 13. 해법 영역에서 가져온 이름을 사용하라
* 코드를 읽을 사람도 프로그래머라는 사실을 명심한다. 그러므로 전산 용어, 알고리즘 이름, 패턴 이름, 수학 용어 등을 사용해도 괜찮다.
* 기술 개념에는 기술 이름이 가장 적합한 선택이다.

## 14. 문제 영역(domain)에서 가져온 이름을 사용하라
* 적절한 '프로그래머 용어'가 없다면 domain에서 이름을 가져온다. 그러면 코드를 보수하는 프로그래머가 분야 전문가에게 의미를 물어 파악할 수 있다.

## 15. 의미있는 맥락을 추가하라
* 스스로 의미가 분명한 이름이 없지 않다. 하지만 대다수 이름은 그렇지 못하다.   
 그래서 클래스, 함수, 이름 공간에 넣어 맥락을 부여한다. 모든 방법이 실패하면 마지막 수단으로 접두어를 붙인다.
* 예를 들어, firstName, lastName, street, houseNumber, city, state, zipcode라는 변수가 있다.
  * 변수를 훑어보면 주소라는 사실을 금방 알아챈다. 하지만 어느 메서드가 state라는 변수 하나만 사용한다면? 변수 state가 주소 일부라는 사실을 금방 알아챌까?
  * addr라는 접두어를 추가해 addrFirstName, addrLastName, addrState라 쓰면 맥락이 좀 더 분명해진다. 변수가 좀 더 큰 구조에 속한다는 사실이 적어도 독자에게는 분명해진다.
  * 물론 Address라는 클래스를 생성하면 더 좋다.

## 16. 불필요한 맥락을 없애라
* 일반적으로는 짧은 이름이 긴 이름보다 좋다. 단, 의미가 분명한 경우에 한해서다. 이름에 불필요한 맥략을 추가하지 않도록 주의한다.




　
## <i><center>"의미 있는 이름을 짓는 것은 코드를 작성하는 것과 직결되는 문제이다." </i></center>

　



>


# 3장. 함수
***

## 1.작게 만들어라
* 함수 안의 줄 수는 적을수록 좋다.
* 들여 쓰기 레벨도 최대 2단까지만 있는 것이 가장 바람직하다.

## 2. 한 가지만 해라
* 한 가지 일을 하는 함수들과 그 함수들을 호출하는 함수 하나로 이루어져 있어야 한다.
의미 있는 이름으로 함수를 추출할 수 있다면 한 가지의 일만 하고 있는 것이다.

## 3. 함수 당 추상화 수준은 하나로
* 코드는 위에서 아래로 읽혀야 한다.

## 4. 함수 인수 최대한 적게 쓰기
* 가장 좋은 경우는 인수가 없는 것, 다음에는 단항 함수(인수가 1개)이다.
* 입력값이 있는 변환 함수는 반환 값이 있는 것이 좋다.
* 플래그 인수(ex. isTrue)는 사용하지 않는 것이 좋다.
* 인수가 많이 필요하다면 독자적인 클래스 생성을 고려해보는 것도 좋은 방법이다.

## 5. 부수 효과 일으키지 말기
* 함수는 정말 그 일만 해야 한다.

## 6. 명령과 조회 분리하기
* 함수는 무언가를 수행하거나 답하거나 둘 중 하나만 해야 한다.

　



>


# 4장. 주석
***
## 1. 주석은 언제나 실패를 의미한다.

* 주석은 오래될 수록 코드에서 멀어진다. 
* 코드는 변화하고 여기저기 옮겨질 때 주석은 코드를 따라가지 못한다.


```java
MockRequest request;
private final String HTTP_DATE_REGEXP = "[SMTWF][a-z]{2}\\,\\s[0-9]{2}\\s[JFMASOND][a-z]{2}\\s" +
        "[0-9]{4}\\s[0-9]{2}\\:[0-9]{2}\\:[0-9]}2|\\sGMT";
private Response response;
private FitNesseContext context;
private FileResponder responder;
private Locale saveLocale;
// Example: "Tue, 02 Apr 2003 22:18:49 GMT"
```
* HTTP_DATE_REGEXP 상수와 주석 사이에 다른 인스턴스 변수들이 추가되었을 가능성이 크다.
* 신뢰가 되지 않는 부정확한 주석보다는 아예 없는 주석이 낫다.   
  <i><div style="text-align:right">*상수: 변하지 않는 변수   
　</i></div>    

  
## 2. 주석은 나쁜 코드를 보완하지 못한다.
* 지저분한 모듈에는 주석을 달지말고 코드를 정리하자.
* 표현력이 풍부하고 깔끔하며 주석이 거의 없는 코드는 복잡하고 주석이 많이 달린 코드보다 훨씬 좋다.

## 3. 코드로 의도를 표현하라.
* 코드로 대다수의 의도를 표현할 수 있다. 주석의 설명을 함수로 표현할 수 있다.


```java
// 직원에게 복지 혜택을 받을 자격이 있는지 검사한다.
if ((employee.flags & HOURLY_FLAG) &&
(employee.age > 65))
```
상단의 코드를 하단의 코드로 변경
```java
if (employee.isEligibleForFullBenefits())
```
<i><div style="text-align:right">*EligibleForFullBenefits: 전체 혜택을 받을 수 있는 자격</i></div>   
　

## 4. 좋은주석
* 법적인 주석: 저작권 정보 또는 소유권 정보  


```java
// Copyright (C) 2003,2004,2005 by Object Mentor, Inc. All rights reserved.
```
　

* 정보를 제공하는 주석: 코드로 표현하지 못할 경우 용이


```java
 // kk:mm:ss EEE, MMM dd, yyyy 형식이다.
 Pattern timeMatcher = Pattern.compile(
         "\\d*:\\d*:\\d* \\w*, \\w* \\d*, \\d*");
```
　

* 의도를 설명하는 주석: 구현을 이해하게 도와줄 뿐만 아니라 결정에 깔린 의도를 설명   


```java
 public void testConcurrentAddWidgets() {
        ...
        // 스레드를 대량 생성하는 방법으로 경쟁 조건을 만든다.
        for (int i = 0; i < 25000; i++){
            WidgetBuilderThread widgetBuilderThread =
                new WidgetBuilderThread(WidgetBuilder, text, parent, failFlag);
            Thread thread = new Thread(widgetBuilderThread)
            thread.start();
          }
          assertEquals(false, failFlag.get());
        }
```
　
* 의미를 명료하게 밝히는 주석: 모호한 인수나 반환값은 그 의미를 읽기 좋게 표현    


```java
assertTrue(a.compareTo(a) == 0); // a == a
        assertTrue(a.compareTo(b) != 0); // a != b
```
　
* 결과를 경고하는 주석: 제3자가 수정을 하게 될 경우 유용


```java
 public static SimpleDateFormat makeStanardHttpDateFormat() {
        // SimpleDateFormat은 스레드에 안전하지 못하다.
        // 따라서 각 인스턴스를 독립적으로 생성해야 한다.
        SimpleDateFormat df = new SimpleDateFormat("EEE, dd MMM yyy HH:mm:ss z");
        dt.setTimeZone(TimeZone.getTimeZone("GMT"));
        return df;
        }
```
　
* TODO 주석: 앞으로 발생할 이벤트에 맞춰 코드를 고치라는 주의 등에 유용. 나쁜코드를 남기는 핑계가 되면 안됨


```java
 // TODO 현재는 필요하지 않다.
 protected VersionInfo makeVersion() {
     return null;
 }
```
　
* 중요성을 강조하는 주석


```java
String listItemContent = match.group(3).trim();
// 여기서 trim으로 시작공백을 제거함으로써 다른 문자열로 인식될 위험을 제거합니다.
```
　
　
## 5. 나쁜주석
* 주절거리는 주석: 코드로 설명 할 수 있는데 코드를 설명하는 주석


```java
// 속성 파일이 없다면 기본값을 모두 메모리로 읽어 들였다는 의미다.
```   
   　
* 같은 이야기를 중복하는 주석: 코드에 있는 내용을 주석으로 서술하면 주석 읽는 시간이 더 걸림


```java
 // this.closed가 true일 때 반환되는 유틸리티 메서드다.
// 타임아웃에 도달하면 예외를 던진다.

public synchronized void waitForClose(final long timeoutMillis)
        throws Exception
        {
            if(!closed)
            {
                wait(timeoutMillis);
                if(!closed)
                    throw new Exception("MockResponseSender could not be cloesd");
            }
        }
```
　
* 오해할 여지가 있는 주석:    
　상단 예시 참조) //this.closed가 true로 변하는 순간 메서드가 반환되지 않음. this.closed가 true일때 반환됨
　
* 의무적으로 다는 주석: 모든 변수에 주석을 달면 코드를 복잡하게 만들고 혼동이 오게 만듬


```java
 /**
 *
 * @param title CD 제목
 * @param author CD 저자
 */
public addCD(String title, String author,
            int tracks, int durationInMinutes) {
    CD cd = new CD();
    cd.title = title;
    cd.author = author;
    cd.tracks = tracks;
    cd.duration = durationInMinutes;
    cdList.add(cd);
        }
```   
　
* 이력을 기록하는 주석(공로를 돌리거나 저자를 표시하는 주석): 형상관리시스템이 없던 시절 사용했던 주석으로 현재는 불필요


```java
 /**
 * 변경 이력 (11-Oct-2001부터)
 * -------------------------------
 * 11-Oct-2001 : 클래스를 다시 정리하고 새로운 패키지로 옮김
 * 11.Nov-2001 : getDescription() method를 추가
 */
```   
　
* 있으나 마다 한 주석: 당연한 사실을 언급해서 정보를 제공하지 못하는 주석은 제거
* 함수나 변수로 표현 가능한 주석
* 닫는 괄호에 다는 주석: 중첩이 심하고 장황한 함수라면 의미가 있을지도 모르겠지만 이런 경우 함수를 줄이기


```java
 package clean.code.chapter04;

import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class wc {
    public static void main(String[] args) {
        BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
        String line;
        int lineCount = 0;
        int charCount = 0;
        int wordCount = 0;
        try {
            while ((line = in.readLine()) != null) {
                lineCount++;
                charCount += line.length();
                String words[] = line.split("\\W");
                wordCount += words.length;
            } //while
            System.out.println("wordCount = " + wordCount);
            System.out.println("lineCount = " + lineCount);
            System.out.println("charCount = " + charCount);
        } // try
        catch (IOException e) {
            System.err.println("Error:" + e.getMessage());
        } //catch
    } //main
}
```   
　
* 전역정보: 시스템의 전반적인 정보가 아닌 근처에 있는 코드에 대하 주석만 기술   
　　　　(추후 전역 정보가 변했을 때 주석을 함께 변경하는 것을 보장하기 어려움)   
　 
* 비공개코드에서 javadocs: 공개 API는 javadocs가 유용하지만 공개하지 않을 경우에는 코드가 장황해져 쓸모가 없다.
<i><div style="text-align:right">*javadocs: java에서 제공하는 공식적인 주석 가이드</i></div>


　
## <i><center>"나쁜코드에 주석을 달지마라. 주석이 필요없는 코드를 짜라."</i></center>

　   
　
>
# 5장. 형식 맞추기
***
## 1. 형식을 맞추는 목적
* 형식은 의사소통의 일환이고, 전문 개발자의 일차적인 의무이기 때문에 너무나도 중요하다.
* 구현한 기능이 다음 버전에서 바뀌어 원래 코드의 흔적이 없어지더라도 처음 잡은 구현 스타일과 가독성 수준은 영향을 미침   
## 2. 적절한 행 길이를 유지하라
* 큰 파일보다 작은 파일이 일반적으로 이해하기 쉽다.
* 200줄 미만의 코드로도 충분히 크고 복잡한 시스템을 만들 수 있다.   
　
### 1) 신문기사처럼 작성하라
* 이름은 간단하면서도 설명이 가능하게 짓는다.
* 소스 파일 첫 부분은 고차원 개념과 알고리즘을 설명한다.
* 아래로 내려갈수록 의도를 세세하게 묘사한다.
* 마지막에는 가장 저차원 함수와 세부내역이 나온다.

### 2) 개념은 빈 행으로 분리하라
* 각 행은 수식이나 절을 나타내고 일련의 행 묶음은 완결된 생각 하나를 표현
* 생각 사이에는 빈 행을 넣어 분리
```java
package fitnesse.wikitext.widgets;
import java.util.regex.Matcher;
import java.util.regex.Pattern;
public class BoldWidget extends ParentWidget {
    public static final String REGEXP = "'''.+?'''";
    private static final Pattern pattern = Pattern.compile("'''(.+?)'''",
            Pattern.MULTILINE + Pattern.DOTALL
    );
    public BoldWidget(ParentWidget parent, String text) throws Exception {
        super(parent);
        Matcher match = pattern.matcher(text);
        match.find();
        addChildWidgets(match.group(1));
    }
    public String render() throws Exception {
        StringBuffer html = new StringBuffer("<b>");
        html.append(childHtml()).append("</b>");
        return html.toString();
    }
}
``` 
* 아래와 같이 개념은 빈행으로 분리(가독성 좋아짐)
```java
package fitnesse.wikitext.widgets;

import java.util.regex.Matcher;
import java.util.regex.Pattern;

public class BoldWidget extends ParentWidget {
    public static final String REGEXP = "'''.+?'''";
    private static final Pattern pattern = Pattern.compile("'''(.+?)'''",
            Pattern.MULTILINE + Pattern.DOTALL
    );

    public BoldWidget(ParentWidget parent, String text) throws Exception {
        super(parent);
        Matcher match = pattern.matcher(text);
        match.find();
        addChildWidgets(match.group(1));
    }

    public String render() throws Exception {
        StringBuffer html = new StringBuffer("<b>");
        html.append(childHtml()).append("</b>");

        return html.toString();
    }
}
```  
### 3) 세로 밀집도 (수직거리)
* 서로 밀접한 코드 행은 세로로 가까이 놓아야 한다.
```java
public class ReporterConfig {
    /**
     * 리포터 리스너의 클래스 이름
     */
    private String m_className;

    /**
     * 리포터 리스너의 속성
     */
    private List<Property> m_properties = new ArrayList<Property>();
    public void addProperty(Property property) {
        m_properties.add(property);
    }
``` 
<i><div style="text-align:right">* 세로 밀집도는 연관성을 표현</i></div>
```java
public class ReporterConfig {
    private String m_className;
    private List<Property> m_properties = new ArrayList<Property>();

    public void addProperty(Property property) {
        m_properties.add(property);
    }
```  
#### (1) 인스턴스 변수
* 위의 세로 밀집도와 동일하게 변수간에 세로로 거리를 두지 않는다.

#### (2) 종속 함수
* 한 함수가 다른 함수를 호출한다면 두 함수는 세로로 가까이 배치한다.
* 호출하는 함수를 호출되는 함수보다 먼저 배치한다.  

#### (3) 개념적 유사성
* 한 함수가 다른 함수를 호출해 생기는 직접적인 종속성
* 변수와 그 변수를 사용하는 함수

　

### 3) 가로 형식 맞추기
* 행 길이는 짧은 편이 바람직하다.
* 120자 정도로 제한 하는 것을 권장하며, 그 이상은 주의 부족

#### (1) 들여쓰기
* 파일 전체에 적용되는 정보
* 파일 내 개별 클래스에 적용되는 정보
* 클래스 내 각 메서드에 적용되는 정보
* 블록 내 블록에 재귀적으로 적용되는 정보
* 들여쓰기를 통해 왼쪽으로 코드를 맞춰 코드가 속하는 범위를 시각적으로 표현할 수 있다.

## 4. 팀 규칙
* 소프트웨어의 일관적인 스타일로 보일 수 있게 합의하는 코드 규칙
* 좋은 소프트웨어 시스템은 읽기 쉬운(가독성) 문서로 이루어진다.

## 5. 밥 아저씨의 형식규칙
```java
public class CodeAnalyzer implements JavaFileAnalysis {
    private int lineCount;
    private int maxLineWidth;
    private int widestLineNumber;
    private LineWidthHistogram lineWidthHistogram;
    private int totalChars;

    public CodeAnalyzer() {
        lineWidthHistogram = new LineWidthHistogram();
    }

    public static List<File> findJavaFiles(File parentDirectory) {
        List<File> files = new ArrayList<File>();
        findJavaFiles(parentDirectory, files);
        return files;
    }

    private static void findJavaFiles(File parentDirectory, List<File> files) {
        for (File file : parentDirectory.listFiles()) {
            if (file.getName().endsWith(".java"))
                files.add(file);
            else if (file.isDirectory())
                findJavaFiles(file, files);
        }
    }

    public void analyzeFile(File javaFile) throws Exception {
        BufferedReader br = new BufferedReader(new FileReader(javaFile));
        String line;
        while ((line = br.readLine()) != null)
            measureLine(line);
    }

    private void measureLine(String line) {
        lineCount++;
        int lineSize = line.length();
        totalChars += lineSize;
        lineWidthHistogram.addLine(lineSize, lineCount);
        recordWidestLine(lineSize);
    }

    private void recordWidestLine(int lineSize) {
        if (lineSize > maxLineWidth) {
            maxLineWidth = lineSize;
            widestLineNumber = lineCount;
        }
    }

    public int getLineCount() {
        return lineCount;
    }

    public int getMaxLineWidth() {
        return maxLineWidth;
    }

    public int getWidestLineNumber() {
        return widestLineNumber;
    }

    public LineWidthHistogram getLineWidthHistogram() {
        return lineWidthHistogram;
    }

    public double getMeanLineWidth() {
        return (double)totalChars/lineCount;
    }

    public int getMedianLineWidth() {
        Integer[] sortedWidths = getSortedWidths();
        int cumulativeLineCount = 0;
        for (int width : sortedWidths) {
            cumulativeLineCount += lineCountForWidth(width);
            if (cumulativeLineCount > lineCount/2)
                return width;
        }
        throw new Error("Cannot get here");
    }

    private int lineCountForWidth(int width) {
        return lineWidthHistogram.getLinesforWidth(width).size();
    }

    private Integer[] getSortedWidths() {
        Set<Integer> widths = lineWidthHistogram.getWidths();
        Integer[] sortedWidths = (widths.toArray(new Integer[0]));
        Arrays.sort(sortedWidths);
        return sortedWidths;
    }
}
```  




　
## <i><center>"규칙을 정하고 일관성 있게 코드를 짜라." </i></center>
   
　

   

> 
# 6장. 객체와 자료구조
***
## 1. 자료 추상화
* 구현을 감추기 위해서 추상화가 필요
* 사용자가 구현을 모른채 자료의 핵심을 조작할 수 있어야 진정한 의미의 클래스이다.
```java
public class Point {
    public double x;
    public double y;
}
```  
```java
public interface Point {
    double getX();
    double getY();
    void setCartesian(double x, double y);
    double getR();
    double getTheta();
    void setPolar(double r, double theta);
``` 
## 2. 자료/객체 비대칭
* 객체와 자료 구조는 본질적으로 상반된다.
* 객체는 추상화 뒤로 자료를 숨긴 채 자료를 다루는 함수만 공개
* 자료 구조는 자료를 그대로 공개

### 1) 절차적인 도형
* 함수 추가시 용이
* 절차 지향에서 어려운 변경 코드는 객체 지향에서 쉽다.
* 새로운 동작을 추가하는 유연성이 필요하면 자료 구조, 절차적인 코드가 더 적합하다.

```java
public class Square {
    public Point topLeft;
    public double side;
}

public class Rectangle {
    public Point topLeft;
    public double height;
    public double width;
}

public class Circle {
    public Point center;
    public double radius;
}

public class Geometry {
    public final double PI = 3.141592653589793;

    public double area(Object shape) throws NoSuchShapeException {
        if (shape instanceof Square) {
            Square s = (Square)shape;
            return s.side * s.side;
        } else if (shape instanceof Rectangle) {
            Rectangle r = (Rectangle)shape;
            return r.height * r.width;
        } else if (shape instanceof Circle) {
            Circle c = (Circle)shape;
            return PI * c.radius * c.radius;
        }
        throw new NoSuchShapeException();
    }
}
```
### 2) 객체 지향적인 도형
* 클래스 추가시 용이
* 객체지향에서 어려운 변경 코드는 절차 지향 코드에서 쉽다.
* 새로운 자료 타입을 추가하는 유연성이 필요하면 객체가 더 적합하다.
```java
public class Square implements Shape { 
	private Point topLeft;
	private double side;

	public double area() { 
		return side * side;
	} 
}

public class Rectangle implements Shape { 
	private Point topLeft;
	private double height;
	private double width;

	public double area() { 
		return height * width;
	} 
}

public class Circle implements Shape { 
	private Point center;
	private double radius;
	public final double PI = 3.141592653589793;

	public double area() {
		return PI * radius * radius;
	} 
}
```
### 3) 절차적인 코드와 객체 지향 코드
#### (1) (자료 구조를 사용하는)절차적인 코드

* 기존 자료 구조를 변경하지 않으면서 새 함수를 추가하기 쉽다.
* 새로운 자료 구조를 추가기 어렵다. 그러기 위해선 모든 함수를 고쳐야 한다.
* 새로운 자료 타입이 아니라 새로운 함수가 필요한 경우에 더 유리
#### (2)객체 지향 코드
* 기존 함수를 변경하지 않으면서 새 클래스를 추가하기 쉽다.
새로운 클래스를 추가하기 어렵다. 그러기 위해선 모든 클래스를 고쳐야 한다.
새로운 함수보다는 새로운 자료 타입이 필요한 경우 더 유리
모든 문제를 객체로 해결하려는 생각은 좋지 않다.
## 3. 디미터 법칙
* 모듈은 자신이 조작하는 객체의 속사정을 몰라야 한다.   
　
  <i><div style="text-align:right">* 휴리스틱이란? 경험에 기반하여 문제를 해결하거나 발견해 내는 방법   
최적의 해 대신 현실적으로 만족할 만한 수준의 해를 구하는 방법</i></div>
### 1) 기차충돌
* 객차가 한줄로 이어진 기차처럼 보임 (디미터 법칙을 어김)
```java
final String outputDir = ctxt.getOptions().getScratchDir().getAbsolutePath();
```
* 아래와 같이 함수를 반환하는 값을 나누어 사용
```java
Options opts = ctxt.getOptions();
        File scratchDir = opts.getScratchDir();
final String outputDir = scratchDir.getAbsolutePath();
```
* 자료구조였을 경우엔 아래와 같이 구현한다.

```java
final String outputDir = ctxt.options.scratchDir.absolutePath;
```




　
## <i><center>"모듈은 자신이 조작하는 객체의 속사정을 몰라야 한다." </i></center>

　



>


# 7장. 오류 처리
***
* 상당수 코드 기반은 전적으로 오류 처리 코드에 좌우되기 때문에 깨끗한 코드와 연관성이 있다.
## 1. 오류 코드보다 예외를 사용하라
* 호출한 즉시 오류를 확인해야 하기 때문에 호출자 코드가 복잡 해진다.
* 오류 확인을 잊어버리기 쉽다.
``` java
public class DeviceController {
	...
	public void sendShutDown() {
		DeviceHandle handle = getHandle(DEV1);
		// 디바이스 상태를 점검한댜.
		if (handle != DeviceHandle.INVALID) {
			// 레코드 필드에 디바이스 상태를 저장한다.
			retrieveDeviceRecord(handle);
			// 디바이스가 일시정지 상태가 아니라면 종료한다.
			if (record.getStatus() != DEVICE_SUSPENDED) {
				pauseDevice(handle);
				clearDeviceWorkQueue(handle);
				closeDevice(handle);
			} else {
				logger.log("Device suspended. Unable to shut down");
			}
		} else {
			logger.log("Invalid handle for: " + DEV1.toString());
		}
	}
	...
}
```
* 오류 발생 시 예외를 던지는 편이 더 좋다.
* 논리가 오류 처리 코드와 뒤섞이지 않아 호출자 코드가 더 깔끔해짐   
　
  <i><div style="text-align:right">* 예외란? 프로그램 실행 중에 정상적인 프로그램의 흐름에 어긋나는 이벤트
</i></div>
```java
public class DeviceController {
	...
	public void sendShutDown() {
		try {
			tryToShutDown();
		} catch (DeviceShutDownError e) {
			logger.log(e);
		}
	}

	private void tryToShutDown() throws DeviceShutDownError {
		DeviceHandle handle = getHandle(DEV1);
		DeviceRecord record = retrieveDeviceRecord(handle);
		pauseDevice(handle); 
		clearDeviceWorkQueue(handle); 
		closeDevice(handle);
	}

	private DeviceHandle getHandle(DeviceID id) {
		...
		throw new DeviceShutDownError("Invalid handle for: " + id.toString());
		...
	}
	...
}
```



## 2. Try-Catch-Finally문부터 작성하라
* try-catch-finally 문에서 try 블록에 들어가는 코드를 실행하면 어느 시점에서든 실행이 중단된 후 catch 블록으로 넘어갈 수 있다.
* try 블록에서 무슨 일이 생기든지 catch 블록은 프로그램 상태를 일관성 있게 유지해야 함
* try-catch-finally 문을 시작으로 코드를 짜면 호출자가 기대하는 상태를 정의하기 쉬워짐
### 1) TDD 방식으로 메소드 구현
<i><div style="text-align:right">*Test Driven Develpment: 테스트 주도 개발
</i></div>
* 단위 테스트를 만든다.
* 단위 테스트에 맞춰 코드를 구현한다.
* 파일 접근을 시도하도록 구현한다.
* 테스트 성공 후 리펙터링 가능
* 장점: 높은코드의 안전성, 재설계 시간의 단축, 디버깅 시간의 단축

## 3. 미확인 unchecked 예외를 사용하라
### 1) 미확인 예외란?
* Unchecked 예외 는 실행 단계에서 확인되며 명시적인 처리를 강제하지는 않는 예외


## 4. 예외에 의미를 제공하라
* 오류가 발생한 원인과 위치를 찾기 쉽도록 호출 스택만으로는 부족한 정보를 충분히 덧붙여야 함
* 오류 메시지에 정보를 담음
* 실패한 연산 이름, 실패 유형 언급

## 5. 호출자를 고려해 예외 클래스를 정의하라
* 예외에 가독성을 높이기 위한 단순화 처리
```java
 ACMEPort port = new ACMEPort(12);

        try {
        port.open();
        } catch (DeviceResponseException e) {
        reportPortError(e);
        logger.log("Device response exception", e);
        } catch (ATM1212UnlockedException e) {
        reportPortError(e);
        logger.log("Unlock exception", e);
        } catch (GMXError e) {
        reportPortError(e);
        logger.log("Device response exception");
        } finally {
        ...
        }
```
위의 모든 예외에 대한 처리를 아래와 같이 호출하는 라이브러리 API를 감싸 예외 유형 하나로 반환
```java
 LocalPort port = new LocalPort(12);
 try {
     port.open();
    } catch (PortDeviceFailure e) {
     reportError(e);
     logger.log(e.getMessage(), e);
        } finally {
     ...
 }
```

## 6. null을 반환/전달 하지 마라
* 코드 내에서 무의미하게 null을 체크하게 된다.
```java
public void registerItem(Item item) {
        if (item != null) {
            ItemRegistry registry = peristentStore.getItemRegistry();
            if (registry != null) {
                Item existing = registry.getItem(item.getID());
                if (existing.getBillingPeriod().hasRetailOwner()) {
                    existing.register(item);
                }
           }
        }
}
```





　
## <i><center>"깨끗한 코드는 읽기도 좋아야 하고 안정성도 높아야 한다." </i></center>

　



>


# 8장. 경계
***
## 1. 외부 코드 사용하기
* 제공자가 사용자에게 인터페이스를 제공
* 제공자와 사용자의 입장차이로 인하여 문제가 야기될 수 있음
* 제공자가 제공한 인터페이스가 변경될 경우 수정할 코드가 많아 질 수 있음
  * 제공자가 준 객체(인터페이스)를 감싸는 방법으로 해결이 가능
  
## 2. 경계 살피고 익히기
* 공식 문서를 보고 공부한다
* 코드를 작성해 작동하는지 확인한다.
* 디버깅해서 문제없는지 확인한다. 

### <center> 외부 코드를 익히고 통합하는 어려운 일은 위처럼 할 수도 있지만 학습 테스트를 통해 할 수 있다.</center>

### 1) 학습테스트
* 먼저 간단한 테스트 코드를 작성해서 외부 라이브러를 알아본다. 
* 내가 사용하고자하는 목적대로 프로그램을 개발한다.

## 3. log4j 익히기
###### 예시) log4j를 익히는 방법 

### 1)공식 문서 읽기
### 2)테스트 케이스 작성하기 

```java
@Test
 public void testLogCreate() {
     Logger logger = Logger.getLogger("MyLogger");
     logger.info("hello");
 }
```
###### 위의 코드로 돌리고 나니 Appender가 필요하다는 오류 발생 

```java
@Test
 public void testLogAddAppender() {
     Logger logger = Logger.getLogger("MyLogger");
     ConsoleAppender appender = new ConsoleAppender();
     logger.addAppender(appender);
     logger.info("hello");
 }
```
###### 다시 수정하여 돌려보니 ConsoleAppender라는 클래스가 필요하다는 오류 발생 

```java
public class LogTest {
     private Logger logger;

     @Before
     public void initialize() {
         logger = Logger.getLogger("logger");
         logger.removeAllAppenders();
         Logger.getRootLogger().removeAllAppenders();
     }

     @Test
     public void basicLogger() {
         BasicConfigurator.configure();
         logger.info("basicLogger");
     }

     @Test
     public void addAppenderWithStream() {
         logger.addAppender(new ConsoleAppender(
             new PatternLayout("%p %t %m%n"),
             ConsoleAppender.SYSTEM_OUT));
         logger.info("addAppenderWithStream");
     }

     @Test
     public void addAppenderWithoutStream() {
         logger.addAppender(new ConsoleAppender(
             new PatternLayout("%p %t %m%n")));
         logger.info("addAppenderWithoutStream");
     }
 }
```

###### 반복적으로 하다보면 위의 테스트 케이스처럼 완성할 수 있음


## 4. 학습 테스트는 공짜 이상이다
* 학습 테스트는 위에서 보았듯이 시간이 많이 걸릴 수도 있지만 그만큼 이점이 있는 부분도 있다. 
* 패키지가 예상대로 도는지 검증하고, 통합 이후에도 주기적으로 검증이 가능하다.   
  프로그램에 오류가 있는지도 테스트 케이스로 확인이 가능하다. 
* 외부 라이브러리 버전이 업데이트 되더라도 테스트케이스를 통해 내가 개발한 부분이 문제가 없는지 확인이 가능하다. 



## 5. 아직 존재하지 않는 코드를 사용하기
* 만약 A사와 협업을 하는 상황이고 A라는 회사에서는 개발을 진행하지 않고 나만 개발을 진행한다고 하면   
   aa 라는 인터페이스를 정의 하고 A사와 공유 하고 난 후 나먼저  개발을 할 수있다.   
   즉, 존재 하지 않은 기능에 대해서 나먼저 구현이 가능한것 처럼 나와 A사의 병렬 업무처리가 가능함



## 6. 깨끗한 경계 
* 외부 라이브러리와 개발을 할 때는 경계를 깔끔하게 분리해야함
* 테스트 케이스를 작성해서 외부 라이브러리가 문제 없는지 확인   
* 외부 라이브러리를 내가 개발하는 프로그램의 용도로 변경해서 버전이 변경되도 문제 없도록 하듯이 개발해야함



