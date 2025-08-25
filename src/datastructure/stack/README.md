# 스택(Stack)

## 1. 정의
스택(Stack)은 **후입선출(LIFO, Last In First Out)** 구조의 자료구조입니다.  
- 마지막에 들어온 데이터가 **가장 먼저 나가는 구조**입니다.

---

## 2. 특징
- 한쪽 끝(top)에서만 삽입(push)과 삭제(pop)가 이루어짐
- 삽입과 삭제가 제한적이므로 구현이 간단함
- 주로 **함수 호출, 뒤로 가기, undo 기능** 등에 활용됨

---

## 3. 주요 연산
| 연산 | 설명 |
|------|------|
| push | 스택의 가장 위에 데이터를 추가 |
| pop  | 스택의 가장 위 데이터를 제거하고 반환 |
| peek/top | 스택의 가장 위 데이터를 제거하지 않고 반환 |
| isEmpty | 스택이 비어있는지 확인 |
| size | 스택에 들어있는 데이터 개수 반환 |

---

## 4. 구현 예시 (Java)

### 4.1. 기본 Stack 클래스 사용
```java
import java.util.Stack;

Stack<Integer> stack = new Stack<>();
stack.push(10);
stack.push(20);

System.out.println(stack.peek()); // 20
System.out.println(stack.pop());  // 20
System.out.println(stack.pop());  // 10
System.out.println(stack.isEmpty()); // true
