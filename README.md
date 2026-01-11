# Fast Food Nutrition Analysis – Data Analyst Project

 ผู้บริโภคจำนวนมากรับประทานอาหารฟาสต์ฟู้ดเป็นประจำ แต่ยังขาดข้อมูลที่ชัดเจนเกี่ยวกับคุณค่าทางโภชนาการของเมนูแต่ละรายการ เช่น ปริมาณแคลอรี ไขมัน น้ำตาล และโปรตีน ซึ่งการขาดข้อมูลเหล่านี้ทำให้การตัดสินใจเลือกอาหารที่ดีต่อสุขภาพเป็นเรื่องยาก

---

โครงการนี้มีวัตถุประสงค์เพื่อวิเคราะห์ข้อมูลโภชนาการของอาหารฟาสต์ฟู้ด โดยมีเป้าหมายเพื่อ
- ระบุเมนูที่มีปริมาณแคลอรีและไขมันสูงที่สุด 
- เปรียบเทียบค่าโภชนาการเฉลี่ยของเมนูจากบริษัทฟาสต์ฟู้ดแต่ละราย  
- สรุป Insight ที่สามารถนำไปใช้ได้จริงสำหรับผู้บริโภคที่ใส่ใจสุขภาพ

---

## Objective
- วิเคราะห์ข้อมูลโภชนาการของเมนูอาหารฟาสต์ฟู้ด
- แสดงรูปแบบและความสัมพันธ์ของข้อมูลด้วยการทำ Visualization
- สรุป Insight สำคัญที่สามารถใช้เป็นแนวทางในการเลือกอาหารที่ดีต่อสุขภาพ หรือช่วยในการวางแผนเมนู

---

## Dataset
**Fast Food Nutrition Dataset : https://www.kaggle.com/datasets/joebeachcapital/fast-food**  
- ประกอบด้วยตัวอย่างข้อมูลเมนูอาหารฟาสต์ฟู้ดประมาณ 9 รายการ (สามารถขยายเป็นชุดข้อมูลจริงที่มีมากกว่า 50 รายการได้)
- ตัวแปรที่ใช้ในการวิเคราะห์ ได้แก่
  - บริษัท/แบรนด์ (เช่น McDonald’s, KFC, Starbucks)
  - ชื่อเมนู 
  - พลังงาน (Calories)  
  - พลังงานจากไขมัน (Calories from Fat)  
  - ปริมาณไขมันทั้งหมด ไขมันอิ่มตัว และไขมันทรานส์ (Total Fat, Saturated Fat, Trans Fat)
  - คอเลสเตอรอล และโซเดียม (Cholesterol, Sodium)
  - คาร์โบไฮเดรต ใยอาหาร และน้ำตาล (Carbohydrates, Fiber, Sugars)
  - โปรตีน (Protein)
  - คะแนน Weight Watchers

**Sample Data:**

| Company      | Item                  | Calories | Total_Fat | Protein |
|-------------|----------------------|---------|-----------|---------|
| McDonald's  | Big Mac              | 550     | 30        | 25      |
| McDonald's  | Fries Large          | 500     | 26        | 7       |
| KFC         | Fried Chicken        | 450     | 30        | 35      |
| Subway      | Turkey Sandwich      | 280     | 7         | 18      |
| Starbucks   | Caffe Latte          | 190     | 8         | 12      |

---

## Tools & Skills
- Python (pandas, numpy)  
- Data Visualization (matplotlib, seaborn)  
- Exploratory Data Analysis (EDA)  
- Data Cleaning & Preprocessing  
- Business Insight & Data Storytelling  

---

## Analysis Workflow
1. โหลดข้อมูลและตรวจสอบภาพรวมของชุดข้อมูล
2. ทำความสะอาดและเตรียมข้อมูล  
   - ปรับชื่อคอลัมน์ให้สอดคล้องและเข้าใจง่าย 
   - แปลงข้อมูลตัวเลขให้อยู่ในรูปแบบที่ถูกต้อง 
3. วิเคราะห์ข้อมูลเชิงสำรวจ (Exploratory Data Analysis: EDA))  
   - การกระจายของพลังงาน (Calories)
   - ค่าเฉลี่ยพลังงานแยกตามบริษัท  
   - วิเคราะห์ความสัมพันธ์ระหว่างสารอาหารด้วย Correlation Matrix  
4. แสดงผลข้อมูลของเมนูที่มีแคลอรีสูงด้วยกราฟ  
5. สรุป Insight สำคัญและข้อเสนอแนะที่สามารถนำไปใช้ได้จริง

---

## Model Performance / Visualization (Example Graphs)

**Calories Distribution**

![Calories Distribution](images/calories_distribution.png)
แคลอรีของเมนูฟาสต์ฟู้ดโดยรวม กระจายตัวอย่างไร
- เมนูส่วนใหญ่อยู่ช่วงแคลอรีต่ำหรือสูง
- มีเมนูที่แคลอรีสูงมากผิดปกติหรือไม่
สิ่งที่เจอ (Result)


**Average Calories by Company**

![Average Calories by Company](images/avg_calories_company.png)

**Correlation Matrix of Nutritional Values**

![Correlation Matrix](images/correlation_matrix.png)

**Top 10 Highest Calorie Items**

![Top 10 Highest Calorie Items](images/top_calories.png)

---

## Key Insights
1. Menu items with the highest calories usually come from **McDonald's and Pizza Hut**.  
2. Companies with higher average calories typically serve more **fast food items**.  
3. Calories are strongly correlated with **Total Fat**, meaning high-fat items tend to be high-calorie.  
4. Salad and beverage items generally have low calories and are better options for calorie-conscious consumers.  

---

## Business / Practical Recommendations
- Promote healthier menu options by highlighting low-calorie items (e.g., salads, beverages)  
- Reformulate menu items to reduce fat while maintaining flavor  
- Educate consumers with clear nutritional information to guide choices  
- Use insights to design marketing campaigns for healthier options

---

## Conclusion
This project demonstrates how **data analysis and visualization** can be applied to understand nutritional content in fast food.  
The insights can help businesses design healthier menus and guide consumers to make informed choices, ultimately promoting better health outcomes.

---

## Author
**Dolthida**  
Computer Science Student | Aspiring Data Analyst
