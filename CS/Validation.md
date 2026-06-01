# Validation (유효성 검증)

- 입력된 데이터나 값이 올바른지 확인하는 과정
- 문법적으로는 올바르나, 의도한 값이 아닌지를 확인한다.

## Validation 예시

1. 범위 검사

	> `if(hp<0)` 등

1. Null 검사

	> `if(obj == null)` 등

1. 문자열 검사

	> `if(string.IsNullOrEmpty(name))`닉네임 등 필요한 문자열이 비어있는지 확인

1. 형식 검사

	> 이메일을 입력 받을 때, `abc@naver.com`은 정상이지만 `abc@@`는 비정상

## Validation 전용 메서드 (유니티)

```csharp
private void OnValidate(){}
```
- Inpector내에서 값 변경 시 자동으로 호출된다.

## Validation과 예외 처리

1. Validation은 문제 발생 전에 검사하여 문제 발생을 예방한다.
1. 예외처리는 문제가 발생 한 후 처리한다.