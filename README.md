## ✅ Commit Convention (공통)  
커밋 메세지 구조는 아래의 구조를 따른다. <br></br>
커밋 메세지 각 파트는 빈 줄을 두어 구분한다.

### 구조
> [타입] (옵션): [제목]<br></br>
> [본문]

### 예시
> “feat: 로그인 기능 구현”
> - Next Auth 패키지 설치
> - Prisma DB 어댑터 추가

### 커밋 타입
타입은 모두 소문자로 한다.
* feat : 새로운 기능 추가
* fix : 버그 수정
* docs : 문서 수정
* style : 코드 포맷팅
* refactor : 코드 리팩토링
* test : 테스트 코드
* chore : 빌드 업무


## ✅ PR Convention (공통)
> 제목 : DENTALCHART #(IssueNumber) [포괄적 제목]
>
> <작업 내용>
>
>- 로그인 퍼블리싱
>- 회원가입 api 기능 구현
>
> <첨부>
>
><!-- 테스트or결과 스크린샷 첨부 -->
>
> <관련된 이슈, 커밋, PR>
>
> closes #(Number)


### 첨부할 필수 이미지 목록
* build 캡쳐
> yarn build or yarn build --debug

<img width="799" alt="build" src="https://user-images.githubusercontent.com/60413257/218659167-22030b2a-71e4-4843-ba13-349460b65d5c.png">

* lint, prettier 캡쳐
> 이 부분은 husky&lint-staged로 pre-commit 스테이지에서 자동 실행 . 캡쳐 첨부 강제 X

<img width="1248" alt="lintcheck" src="https://user-images.githubusercontent.com/60413257/218660151-a3414260-299c-4588-aefe-77d3d9b58c5d.png">

* 타입 체크 캡쳐
> 새로 추가한 타입이나 인터페이스에 대해서 이미지 첨부 부탁드립니다.

<img width="365" alt="typecheck" src="https://user-images.githubusercontent.com/60413257/218660254-389ca897-a179-4ec9-a99e-623367a66bad.png">

* 작업한 내용 결과물
> 결과물은 본인이 구현한 부분에 대한 설명을 위해서라도 반드시 첨부해주세요.

<img width="825" alt="slidercheck" src="https://user-images.githubusercontent.com/60413257/218660374-a9035da0-9505-41a5-898e-692b6c927ffb.png">
[슬라이더 구현]

### feature -> develop 배포 전 수행 목록
* build 체크
* lint, prettier 체크
* github action
* 코드 리뷰

### develop -> master 배포 전 수행 목록]
* build 체크
* preview 체크
