# Django

## Django의 구동 원리 : MTV 패턴

### MTV
>  ( Model, Template, View )
> M, T, V 각기 독립적으로 임무 수행

- Model : 데이터베이스를 관리. ( DB 담당 )
- Template : 사용자들에게 보여지는 화면 ( HTML ) ( 보여주기 담당 ) 
- View : 데이터가 어떤상황에서 어떻게 처리되는지를 알려주는 함수들이 모여있는 곳 ( 처리 담당 )

+++
### MVC
> ( Model, View, Controller )
> MTV가 차용한 방식

- Model : 데이터베이스를 관리
- View : 사용자에게 보여지는 부분 담당 ( MTV의 View와는 다름 )
- Controller : 중간 관리 담당

-> MTV의 <VIEW>, MVC의 <CONTROLLER>가 패턴의 실제 동작하는 부분.
  
## 템플릿 변수
> HTML안에 파이썬 변수/문법을 쓰고 싶을 때 사용
```
{{ python_value }}
```

해당 파이썬 변수를 HTML파일에 담아 출력하기 위해 쓰는 변수.


### 템플릿 필터
> 템플릿 변수에 추가적인 속성 및 기능 제공
```
{{ python_value | filter }}
```

e.g. 
```
{{ python_value | length}} 
```
value의 길이 반환
```
{{ python_value | lower }}
```
value를 소문자로 출력



