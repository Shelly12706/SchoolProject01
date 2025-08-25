# 魔法學院課程管理系統

# 專案簡介
此系統為魔法學院課程管理系統，採用 **Java Swing + MVC + SQL** 架構，支援學生選課、老師管理課程、成績登錄、報表統計等功能。  
# 功能特色

| 類別 | 功能特色 |
|------|----------|
| **Util** | - `CodeGenerator`：自動生成學生、老師、課程編號 <br> - `PasswordUtil`：密碼雜湊 SHA-256 / MD5，支援驗證 <br> - `DbConnection`：提供 MySQL 連線 |
| **DAO** | - 提供 CRUD 介面 <br> - `StudentDao`, `TeacherDao`, `CourseDao`, `EnrollmentDao` <br> - `dao.impl` 實作資料庫操作 |
| **Service** | - 商業邏輯處理 <br> - `StudentService`, `TeacherService`, `CourseService`, `EnrollmentService` <br> - `service.impl` 實作 Service 介面，封裝 DAO 操作 |
| **Controller** | - Swing 畫面控制 <br> - `LoginFrame`, `CoursePanel`, `TeacherPanel`, `ReportPanel` <br> - 處理按鈕事件、流程導向、報表呼叫 |
| **報表** | - `ReportPanel` 顯示課程學生數、通過率、平均分數、個人成績趨勢 <br> - 支援 Excel 匯出 |

---
# 專案架構

```text
MagicAcademy/
├─ src/main/java/
│  ├─ model/
│  │  ├─ Student.java
│  │  ├─ Teacher.java
│  │  ├─ Course.java
│  │  └─ Enrollment.java
│  ├─ dao/
│  │  ├─ StudentDao.java
│  │  ├─ TeacherDao.java
│  │  ├─ CourseDao.java
│  │  ├─ EnrollmentDao.java
│  │  └─ impl/
│  │     ├─ StudentDaoImpl.java
│  │     ├─ TeacherDaoImpl.java
│  │     ├─ CourseDaoImpl.java
│  │     └─ EnrollmentDaoImpl.java
│  ├─ service/
│  │  ├─ StudentService.java
│  │  ├─ TeacherService.java
│  │  ├─ CourseService.java
│  │  ├─ EnrollmentService.java
│  │  └─ impl/
│  │     ├─ StudentServiceImpl.java
│  │     ├─ TeacherServiceImpl.java
│  │     ├─ CourseServiceImpl.java
│  │     └─ EnrollmentServiceImpl.java
│  ├─ controller/
│  │  ├─ LoginFrame.java
│  │  ├─ MainMenuFrame.java
│  │  ├─ CoursePanel.java
│  │  ├─ TeacherPanel.java
│  │  └─ ReportPanel.java
│  └─ util/
│     ├─ CodeGenerator.java
│     ├─ PasswordUtil.java
│     └─ DbConnection.java
└─ pom.xml



---
![老師登入](pic/teacher_login.png)  
![老師新增課程_衝堂](pic/teacher_add_course_conflict.png)  
![老師課程管理](pic/teacher_course_manage.png)  
![老師課程管理_刪除](pic/teacher_course_delete.png)  
![老師課程管理_修改](pic/teacher_course_edit.png)  
![老師課程管理_新增](pic/teacher_course_add.png)  
![老師成績管理](pic/teacher_grade_manage.png) 
![老師成績管理_單筆](pic/teacher_grade_single.png)  
![老師成績管理_批次](pic/teacher_grade_batch.png)  
![老師課程及成績管理](pic/teacher_course_grade_manage.png)  
![老師端統計總表](pic/teacher_report_total.png)

![學生登入](pic/student_login.png)
![註冊畫面](pic/register.png)
![學生選修成績](pic/student_select_grade.png)  
![學生選課_不能低於](pic/student_course_invalid.png)  
![學生選課_衝堂機制](pic/student_course_conflict.png)  
![學生選課完成](pic/student_course_done.png)  
![學生成績趨勢](pic/student_grade_trend.png)

  



  






