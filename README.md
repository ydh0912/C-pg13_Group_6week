# C-pg13_Group_6week
6주차 토론


6주차 토론

for 문으로 소문자 a~z
일단 printf문을 사용해 printf("%d %d",'a','z') 로 각 소문자의 아스키코드를 찾는다(97,122)
그후
for문에서 i의 값을 97로 초기화 후 i < 123로 97부터 122까지의 아스키코드를 찾음 그후 i++로 하나씩 증가

인터넷에서 대소문자 변환 함수를 찾는다.

tolower() 소문자 변환 , toupper() 대문자 변환

toupper(i));    <--- 소문자를 대문자로 변환 (A B C...)

for문

for(초기화, 조건식, 증감){    
	명령어1;
}

변수를 초기화 후 조건식이 참이면 아래 명령어가 실행 거짓이면 실행 X


다중 for문
for(초기화, 조건식, 증감){
   for(초기화, 조건식, 증감){
	명령어1;

    }
}

변수를 초기화 후 조건식이 참이면 아래 명령어가 실행 거짓이면 실행 X
또 아래 for문이라 똑같이 변수를 초기화 후 조건식이 참이면 아래 명령어가 실행 거짓이면 실행 X

2번째 for문이 끝나면 첫번째 for문의 변수가 증감후 다시 조건식이 참이면 실행하고 조건식이 거짓일때 까지 계속 반복이 되는거 같다

----------------------------------------------------------------------
*
**
***
****
*****

출력하기 위해선 일단 처음에 하나가 찍히고 다음엔 두개가 찍히고 이렇게 하나씩 하나씩 뒤에 생김

일단 하나의 for문으로는 그냥 별만 찍히고 한줄 뛰기가 힘들기에 for문이 다중으로 필요'

아마 다중에서 첫번쨰 for문은 한줄 뛰기용으로 쓰고 두번쨰 다중 for문에 별을 찍는게 맞는거 같음

하지만 조건식에서 숫자만 넣으면 똑같이 *이 하나씩 안찍히고 숫자만큼 찍히고 한줄뛰고 이렇게 되므로

첫 번째 for문에서 변수를 가져와서 그 변수를 조건식에 넣어서 i = 1 일떄 j <= i 로 하면 하나가 찍히고 i = 2면 두 개가 찍히고 이렇게 해결

밖에 for만큼 아래 for가 돌면 되게 만드는걸로 해결





----------------------------------------------------------------------
break는 반복문이나 switch~case문에서 바로 빠져나옴
continue는 바로 증감식으로 올라간다. skip...











----------------------------------------------------------------------


continue and break 사용해서 2의 배수 와 6의 배수인 수를 구하기 

int a;
int sum = 0;
int count = 0;
for (a = 1; a < 1001; a++) {

	if (a % 2 != 0 && a % 6 != 0) continue;

	if (a % 2 == 0 && a % 6 == 0) {
		printf("%d ", a);

		count++;
		if (count >= 10) break;
	}
	
}










----------------------------------------------------------------------
