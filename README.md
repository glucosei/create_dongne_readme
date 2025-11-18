## 🖥️ 프로젝트 소개
![alt text](image.png)
- 실사용자 수: 
- 주요 타겟: 중앙대학교 소프트웨어대학 동문(크자회 회원)
- 핵심 기능: 동문 수첩, 게시판, 학부 공지, 경조사 서비스
- 서비스 링크: https://causw.co.kr

## 🕰️ 개발 기간
* 언제부터 ~


### ⚙️ 개발 환경
- **Language** : Java
- **Framework** : SpringBoot
- **Database** : Amazon Aurora MySQL
- **ORM** : JPA(Hibernate)
- **Build**: Gradle 

## 🖥️ 서버 환경
![alt text](image-1.png)

## 📌 주요 기능
-동문 수첩: 이용자의 프로필을 등록하고 회원들과 공유할 수 있는 동문 수첩 서비스를 운영합니다.<br>
-게시판: 회원들이 자유롭게 등록하고, 댓글을 달 수 있는 자유 게시판과 학생회 및 크자회의 공지를 등록하는 게시판등을 운영합니다.<br>
-학부 공지: 학부 홈페이지에 등록되는 공지들을 모아서 등록 및 공지해주는 서비스를 운영합니다.<br>
-경조사 서비스: 경조사를 등록하고 원하는 그룹에게 공유하는 서비스를 운영합니다.<br>

## 🏗️ 시스템 아키텍처 
- app-main/

 └─ src/main/java/net.causw.app.main
    ├─ controller/        
    ├─ service/           
    ├─ repository/        
    ├─ domain/
    │   ├─ model/         
    │   ├─ policy/        
    │   └─ validation/    
    ├─ dto/               
    ├─ infrastructure/    
    └─ CauswApplication

  -global/

 └─ src/main/java/net.causw.global
    ├─ constant/     
    ├─ exception/    
    └─ util/         

#대표 도메인
- User & Academic

  UserController, UserAcademicRecordApplicationController, UserCouncilFeeController

- Circle & Community

  CircleController, BoardController, PostController, CommentController, ChildCommentController

- Event & Schedule 

  EventController, CalendarController, SemesterController, CeremonyController

- Application & Form

  FormController, InquiryController

- Facility & Resource

  LockerController, StorageController

- Notification

  NotificationLogController, PushController

- Common / Global

  CommonController, GlobalExceptionHandler


## 📂 디렉터리 구조 

## Contact
Email : caucsedongne@gmail.com