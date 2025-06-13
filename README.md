# HR_Analytics_Dashboard
## Project Objective 
The objective of this project is to analyze and visualize workforce data using Power BI to provide actionable insights to Human Resources and business stakeholders. The main aim is to track key workforce metrics, identify patterns in attrition, salaries, roles, and department-wise trends, and help in formulating strategies for improving retention and optimizing human resources.

## Dashboard

![Screenshot 2025-06-13 190945](https://github.com/mayurpatil4103/HR_Analytics_Dashboard/blob/main/Screenshot%202025-06-13%20190945.png )

## Dataset Used
- <a href="https://github.com/mayurpatil4103/HR_Analytics_Dashboard/blob/main/HR_Analytics.csv">HR_Analytics

## KPIs

- ✅ **Total Employees** – Overall number of employees currently in the organization.  
- ✅ **Attrition Rate** – The percentage of employees who have left.  
- ✅ **Average Age** – Average age of employees.  
- ✅ **Average Salary** – Mean salaries across the workforce.  
- ✅ **Average Company Experience** – Average years of service in the company.  
- ✅ **Attrition by Age, Role, Department, Experience, Salary Slab** – To identify patterns.  
- ✅ **Job Roles with Higher Attrition** – To pinpoint roles contributing to turnover.  
- ✅ **Departments with Higher Attrition** – To aid department-specific intervention.  
- ✅ **Educational Background Distribution** – To observe workforce composition.  
- ✅ **Gender Distribution** – To check for gender balance and turnover trends.


## Process 


---

### **🔹 Step 1: Data Collection**  
📌 The data was sourced from the company’s HR database or CSV files (such as employment details, salaries, roles, department, education).

---

### **🔹 Step 2: Data Cleaning & Preparation**  
📌 Use **Power Query (ETL Process)**:  
- ✅ Remove duplicates & null values  
- ✅ Transformed data types (Dates, Numbers)  
- ✅ Calculated additional fields like attrition rate and average salaries  

---


### **🔹 Step 3: Create Key Performance Indicators (KPIs)**  
📌 Use **DAX (Data Analysis Expressions)** for calculated measures:  

- ✅ **Total Employees:**  
```DAX
COUNT(Employee[Employee_ID])
```

- ✅ **Attrition Rate:**  
```DAX
 DIVIDE(COUNT(Leavers), [Total Employees]) * 100
```

- ✅ **Average Salary:**  
```DAX
AVERAGE(Employee[Salary])
```

- ✅ **Average  Age:**  
```DAX
AVERAGE(Employee[Age])
```


---

### **🔹 Step 4: Visualizations**  
📌 **Choose appropriate visuals:**  
- ✅ **KPI Cards** – Display **Total employees, Attrition rate, Average age, Salaries**  
- ✅ **Bar Charts** – attrition by department, age group, job role
- ✅ **Pie chart** – Education, gender distribution
- ✅ **Column charts** – salaries by department, attrition by experience
- ✅ **Tables & Filters** –To present detailed, row-wise data, allowing stakeholders to view attributes for each department or role.

---

### **🔹 Step 5: Dashboard Customization**  
📌 **Improve user experience** by:  
- ✅ Applying **themes & color schemes** for readability  
- ✅ Adding **filters & slicers** (Job Role, Department, Experience, Location)  

---

### **🔹 Step 6: Deployment & Access**  
- ✅ The final Power BI Dashboard was published to Power BI service
- ✅ Access controls were set to allow view and collaboration for HR and stakeholders
- ✅ Scheduled refresh daily to keep data up-to-date
---


### **📊 Project Insights**  

**This HR Analytics Dashboard provides a comprehensive view of workforce trends.
Some key points include:**

- ✅ Higher Attrition in Younger Age Groups (26–35) — Suggests a need for retention strategies tailored toward younger employees.
- ✅ Job Roles with Higher Attrition: Laboratory Technician, Sales Executive, and Research Scientist — May need special incentives or career path programs.
- ✅ Departments Affected: Research & Development and Sales — Suggests department-specific strategies might be required.
- ✅ Major Attrition Cluster: Among salaries <= ₹5K — May indicate dissatisfaction with pay.
- ✅ Experience: Mostly in first 5 years — Suggests onboarding and engagement initiatives could help retain these employees
---

## **✅ Conclusion**  

- ✅ The Research & Development department and Sales team are experiencing the highest turnover.
- ✅ Lab Technicians and Research Scientists are particularly prone to leave, possibly due to limited growth opportunities or salaries.
- ✅ The younger workforce (< 35) and those in their first 5 years with the company show higher attrition, suggesting a need for enhanced engagement, mentoring, and clear career progression plans.
- ✅ To tackle this, the company should focus on retention strategies tailored to these groups, offering incentives, training, and clear promotion paths.
- ✅ Furthermore, salaries at the lower range (< ₹5K) may need to be reassessed to match industry standards and reduce turnover.

