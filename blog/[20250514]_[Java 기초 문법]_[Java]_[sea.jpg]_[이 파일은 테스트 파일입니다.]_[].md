# Java 기초 문법

### 1. 자바 프로그램 구조

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("안녕하세요!");
    }
}
```

- `public class Main` : Main이라는 이름의 클래스 정의 (자바는 모든 코드를 클래스 안에 작성)
- `public static void main(String[] args)` : 프로그램의 **시작점** (main 메서드는 자바 프로그램이 시작되는 곳)
- `System.out.println("문장");` : 화면에 출력하는 코드

---

### 2. 변수와 자료형

| 자료형 | 설명 | 예시 |
| --- | --- | --- |
| `int` | 정수 | `int age = 20;` |
| `double` | 실수 | `double pi = 3.14;` |
| `boolean` | 참/거짓 | `boolean isTrue = true;` |
| `char` | 문자 하나 | `char grade = 'A';` |
| `String` | 문자열 (클래스) | `String name = "수진";` |

---

### 3. 조건문

```java
int age = 18;
if (age >= 20) {
    System.out.println("성인입니다.");
} else {
    System.out.println("미성년자입니다.");
}
```

---

### 4. 반복문

### for 문

```java
for (int i = 0; i < 5; i++) {
    System.out.println(i);
}
```

### while 문

```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
```

---

### 5. 함수(메서드) 만들기

```java
public static int plus(int a, int b) {
    return a + b;
}
```

---

### 6. 클래스와 객체

```java
public class Person {
    String name;
    int age;

    public void introduce() {
        System.out.println("이름: " + name + ", 나이: " + age);
    }
}
```

```java
Person p = new Person(); // 참조값 저장
p.name = "수진";
p.age = 21;
p.introduce();
```

---