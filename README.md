# 🏦 HRBANK 인적 자원 관리 시스템
<div align ="center">
  
**HRBANK [🔗 지금 이용해보러가기](https://sb01-hrbank-team05-production.up.railway.app/)**
</div>


## 프로젝트 소개
- **HRBANK**는 기업의 인적 자원을 안전하게 관리하는 서비스입니다.
- Batch로 데이터를 관리하는 Open EMS입니다.

## 개발 기간
- 기능 구현 : 2025.03.13.~ 2025.03.22
- 리팩토링 : 2025.03.24 ~.

## 작업 방식
- 오전 스크럼 1회 (09:00 ~ 09:30)
- 예상치 못한 버그 발생은 깃 이슈 작성

## 함께한 팀원
<div align= "center">
  
  |강소율|이소영|이규셕|전성삼|오하람|
  |:---:|:---:|:---:|:---:|:---:|
  |<img width="160" alt="image" src="https://github.com/user-attachments/assets/b0c2314f-8c9e-4dab-8caa-a6b4c29bce44">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/57d56c9d-7438-4e89-90de-5b219c45e132">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/8f7f6fbb-b867-4afe-94be-d478dc556547">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/92567bfc-2186-4e1e-849d-b92b843bff70">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/0f51714c-e0b6-4b0c-a755-acb7230915d7">|
  |[@soyul9280](https://github.com/soyul9280)|[@gitSoyoungLee](https://github.com/gitSoyoungLee)|[@impmonzz](https://github.com/impmonzz)|[@hodu31](https://github.com/hodu31)|[@Haram0111](https://github.com/Haram0111)|

</div>

## 프로젝트 목표
- 그동안 배운 기술 스택으로 서비스 만들어보기
- PR, 깃이슈 열심히 작성하기
- 완결보다 완성하기

## 기술스택
<div align= "center">
  <span>
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white">
  <img src="https://img.shields.io/badge/springjpa-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white">
  </span>
</div>

<br>
<br>
</details>

## 역할 분담
### 강소율 (Leader)
- 직원 수 추이 API
- 총 직원수 API
- 부서별 / 직함별 직원 분포 API
- 파일 다운로드 API
  
### 이소영
- 직원 정보 수정 이력 목록 조회 API
- 직원 정보 수정 이력 상세 조회 API
- 수정 이력 건수 조회 API

### 전성삼
- 파일 다운로드 API
- 직원 등록 API
- 직원 목록 조회 API
- 직원 상세 조회 API
- 직원 삭제 API
- 직원 수정 API

### 이규석
- 부서 목록 조회 API
- 부서 등록 API
- 부서 상세 조회 API
- 부서 삭제 API
- 부서 수정 API

### 오하람
- 데이터 백업 목록 조회 API
- 데이터 백업 생성 API
- 최근 백업 정보 조회 API
  
## 폴더구조

```
📦src
 ┣ 📂main
 ┃ ┣ 📂java
 ┃ ┃ ┣ 📂com
 ┃ ┃ ┃ ┣ 📂codeit
 ┃ ┃ ┃ ┃ ┣ 📂demo
 ┃ ┃ ┃ ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜QueryDslConfig.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜SwaggerConfig.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜WebConfig.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂controller
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂api
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeController.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂dto
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂data
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseChangeLogDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseDepartmentDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseEmployeeDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DiffDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeDistributionDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeTrendDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂request
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentCreateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentUpdateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeCreateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeUpdateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂response
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupHistoryDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseBackupDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜ErrorResponse.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂entity
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂enums
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupStatus.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeType.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmploymentStatus.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜PropertyName.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜Backup.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContent.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescription.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLog.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜Department.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜Employee.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂exception
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DuplicateEmailException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜FileNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜FileStorageException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜GlobalExceptionHandler.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂mapper
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeMapper.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂repository
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogCustomRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogCustomRepositoryImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepositoryCustom.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepositoryImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeStatsRepository.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂service
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂impl
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeService.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂storage
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentStorage.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜LocalBinaryContentStorage.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂util
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ClientInfo.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜CursorPageUtil.java
 ┃ ┃ ┃ ┃ ┃ ┗ 📜HrbankApplication.java
 ┃ ┃ ┃ ┃ ┗ 📜.DS_Store
 ┃ ┃ ┃ ┗ 📜.DS_Store
 ┃ ┃ ┗ 📜.DS_Store
 ┃ ┣ 📂resources
 ┃ ┃ ┗ 📂static
 ┃ ┃ ┃ ┣ 📂assets
 ┃ ┃ ┃ ┃ ┣ 📂images
 ┃ ┃ ┃ ┃ ┃ ┗ 📜default-profile.svg
 ┃ ┃ ┃ ┃ ┗ 📜index-CKRSZsvY.js
 ┃ ┃ ┃ ┣ 📜favicon.ico
 ┃ ┃ ┃ ┗ 📜index.html
 ┃ ┗ 📜.DS_Store
 ┣ 📂test
 ┃ ┣ 📂java
 ┃ ┃ ┗ 📂com
 ┃ ┃ ┃ ┗ 📂codeit
 ┃ ┃ ┃ ┃ ┗ 📂demo
 ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentServiceTest.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeTest.java
 ┃ ┃ ┃ ┃ ┃ ┗ 📜HrbankApplicationTests.java
 ┃ ┗ 📂resources
 ┃ ┃ ┗ 📂static
 ┃ ┃ ┃ ┣ 📂assets
 ┃ ┃ ┃ ┃ ┣ 📜index-CpuUHdy1.js
 ┃ ┃ ┃ ┃ ┗ 📜index-kQJbKSsj.css
 ┃ ┃ ┃ ┣ 📜favicon.ico
 ┃ ┃ ┃ ┗ 📜index.html
 ┗ 📜.DS_Store
```

## 주요 기능
- 대시보드
  - 직원 정보, 수정 이력, 데이터 백업 관련 정보 조회
  - 직원 증감 그래프 조회
 
- 부서관리
  - 부서 등록, 수정, 삭제, 검색
 
- 직원관리
  - 직원 등록, 정보 수정, 삭제, 상세 조회, 검색
 
- 수정이력
  - 직원 정보 수정 이력 관리 및 검색
 
- 데이터백업
  - 새 백업 생성 (요청 및 배치 백업 지원)
  - 파일 다운로드
  - 조회 검색
 

**협업 문서 [🔗 notion](https://agate-spectacles-6eb.notion.site/1b5c5631fb0180f6aee4ccdd7b897b74?pvs=4)**
