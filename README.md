# LegalCase-ManagementSystem
The proposed Database Management System (DBMS) for legal case management stands out 
as an invaluable tool by not only centralizing information but also significantly enhancing the 
overall utility of the data. Its relational database structure not only facilitates seamless 
integration and retrieval but also promotes data consistency and accuracy, reducing the
likelihood of discrepancies in legal records. 
 
The interlinked tables provide a holistic view of case information, enabling legal teams to draw 
meaningful correlations between client history, court proceedings, and attorney details. This 
comprehensive approach not only streamlines workflows but also fosters a collaborative 
environment where real-time data sharing can lead to more informed and strategic decision- 
making. Ultimately, the proposed DBMS emerges as a powerful and indispensable tool, 
significantly improving the utility, accessibility, and security of case-related information, and 
thereby contributing to more successful legal outcomes. 

# ER Diagram 
![image](https://github.com/user-attachments/assets/93157841-0151-474d-9e06-4ddde34785a9)

# Schema
1. client files(client_id , first_name ,last_name) 
2. clientnew(client_id ,contact) 
3. attorney(attorney_id,first_name ,last_name ,assigned_cases,client_id) 
4. attorneynew(attorney_id,contact) 
5. worksfor(client_id , attorney_id) 
6. court(court_id, location ,assigned_judges ,name) 
7. case conductedin(case_id ,court_id ,client_id,attorney_id ,title) 
8. casenew(case_id,hearning_dates) 
9. hearing includes(log_id, case_id ,court_id) 
10. evidence presentedwith(evidence_id, description ,photo,video ,date_obtained ,case_id) 
11. documents submittedwith(doc_id , case_id ,contents ,evidence_id) 
12. can_alsobe(doc_id ,evidence_id) 
13. appeal on(appeal_id , case_id ,status) 
14. grounds on(id, terms, appeal_id) 
15. verdict leadsto(settlement ,settlement_details ,verdict_date ,log_id)

# Frontend 
The program features a login window for users to enter their credentials, leading to a data 
entry window upon successful login. This window facilitates the input of various legal case 
details, submitted to a MySQL database. GUI components are styled using tkinter for a modern 
appearance. The application allows for efficient management of legal case information. 

![image](https://github.com/user-attachments/assets/cf45739d-cbe6-49ba-9867-c4a0fd87cdfa)

![image](https://github.com/user-attachments/assets/2c8dcf61-c618-41b4-8788-597d555f80b9)









    
