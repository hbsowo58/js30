1. css에서 변수사용 가상선택자 :root를 사용하여 최상단에서 하는방법(클래스를 사용하기때문에 우선순위 높음)

--red : #DC3545;
background-color: var(--red, #F00) var 예약어를 사용하며, 두번째 파라미터는 --red 변수에 값이 유효하지 않은경우 사용될 값

background-color: var(--red, var(--blue, #F00));

2중구조(변수 --red에 값이 유효하지않은 경우 --blue를 사용하고) 그후에도 유효하지 않으면 #F00을 사용
