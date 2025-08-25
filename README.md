# 魔法學院課程管理系統

# 專案簡介
此系統為魔法學院課程管理系統，採用 **Java Swing + MVC + SQL** 架構，支援學生選課、老師管理課程、成績登錄、報表統計等功能。  
CoursePanel / TeacherPanel 小圖示互動表格
CoursePanel（學生端）
| 欄位 / 按鈕     | 說明     | 互動效果                    |
| ----------- | ------ | ----------------------- |
| 課程列表 JTable | 顯示所有課程 | 點擊「選課」按鈕 → 發生衝堂檢查       |
| 選課按鈕 🟢     | 選擇課程   | 成功加入選課後 JTable 更新，報表刷新  |
| 衝堂警告 ⚠️     | 顯示衝堂訊息 | 阻止選課                    |
| 報表按鈕 📊     | 查看個人成績 | 開啟 ReportPanel 顯示折線圖與表格 |

TeacherPanel（老師端）
| 欄位 / 按鈕     | 說明            | 互動效果                     |
| ----------- | ------------- | ------------------------ |
| 課程列表 JTable | 顯示老師授課課程      | 點擊課程可查看學生列表              |
| 學生列表 JTable | 顯示已選課學生       | 可輸入分數                    |
| 分數輸入欄 ✏️    | 老師輸入學生分數      | 成績即寫入資料庫，報表刷新            |
| 新增課程按鈕 ➕    | 新增課程資料        | 存入資料庫，刷新課程列表             |
| 編輯課程按鈕 ✏️   | 編輯課程資料        | 更新資料庫，刷新列表               |
| 報表按鈕 📊     | 查看選課統計 & 成績統計 | 開啟 ReportPanel 顯示柱狀圖/圓餅圖 |


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

  



  






