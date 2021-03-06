# ภาษาชั้นสูง (high level language)
ความหมายของมันคือเป็นภาษาที่มีลักษณะเหมือนภาษาอังกฤษทั่วๆไป ถูกสร้างมาเพื่อความง่านต่อการเขียน เเละการอ่านโปรเเกรมเเละผู้อ่านไม่จำเป็นต้องมีความรู้ในเรื่องของระบบบฮาร์ดเเวร์ เเต่ก็สามารถอ่านได้

ตัวอย่างของภาษา ได้เเก่ ภาษาฟอร์เทน (fortran), โคบอล(cobal), เบสิก(basic), ปาสคาล(pascal), ซี(C), เอดา(ADA)

เเต่มีข้อจำกัดคือ โปรเเกรมที่ใช้ภาษานี้เขียนจะต้องถูกนำไปเเปรเป็นภาษาเครื่องก่อร วิธีเเปลงนั้นจะเเปลงได้โดยใช้โปรเเกรม compiler หรือ interpreter

เเละมีข้อดีคือ โปรเเกรมนี้สามารถนำไปใช้งานบนเครื่องใดก็ได้เป็น hardware independent คือมีลักษณะที่ไม่ขึ้นอยู่กับเครื่อง เเต่ภาษาที่ได้อาจไม่มีประสิทธิภาพเท่าการเขียนด้วยภาษา assembly โดยตรง

# โปรเซสเซอร์ (Processor,microcontroller)
เป็นหน่วยประมวลผลกลางที่รู้จักกันดีในชื่อ CPU หรือ Processor เป็นองค์ประกอบของคอทพิวเตอร์ทุกชนิด เปรียบเป็นสมองของ computer จะมีวงจรไฟฟ้ามากมายอยู่บนเเผ่นซิลิกอนซิป (มีขนาดเล็กมาก)

## หน้าที่ของ Processor

1. อ่านเเละเเปรคำสั่งที่ถูกเขียนไว้ในโปรเเกรม

2. ประมวลผลคำสั่ง

3. รับส่งข้อมูล

4. ติดต่อรับส่งข้อมูล โดยผ่านหน่วยรับข้อมูลเเละตัวเเสดงผล

5. ย้ายข้อมูล

# ภาษา assembly

เป็นภาษาที่มีการนำสัญลักษณ์ข้อความมาใช้เเทนเลขฐานสอง เพื่อที่จะง่ายต่อการเขียนเเละการจำมากกว่าการเขียนภาษาเครื่อง 

เช่น ADD ------> ADD การบวก

    S  --------> SUBTRACT การลบ
    
    C ----------> CPMPLARE การเปรียบเทียบ
    
    MP ---------> MULTIPLY การคูณ
    
    ST ---------> SRORE การเก็บข้อมูลไว้ในหน่วยความจำ 
    
## ภาษาเครื่อง (Machine language)

เป็นภาษาที่มีระดับต่ำสุดเพราะเป็นการใช้เลขฐานสองเเทนข้อมูลทั้งหมด เเละคำสั่งต่างๆ เเละเเต่ละเครื่องจะมีรูปเเบบคำสั่งเฉพาะของตัวเอง ทำให้การเขียนโปรเเกรมนั้นเกิดความยุ่งยาก 


## ความสัมพันธ์ของภาษา เเละสิ่งข้างต้นที่กล่าวมา 

ภาษาชัั้นสูง (high level language) เเละภาษา assembly คล้ายๆกันตรงที่เวลาจะนำไปใช้งานนั้นต้องเปลี่ยนให้เป็นภาษาเครื่องเสียก่อนที่จะนำไปใช้งานหรือประมวลผล ส่วน processor จะเป็นตัวประมวลผล อ่านเเละเเปล
คำสั่งที่ถูกเขียนไว้ในโปรเเกรม

## เปรียบเทียบความสัมพันธ์ 

example 1 High level language คือ Swift, Processor คือ x86-64 swiftc 5.5 ได้ assembly คือ
<img width="1440" alt="ภาพถ่ายหน้าจอ 2565-04-06 เวลา 21 05 00" src="https://user-images.githubusercontent.com/98943418/161993445-7669ed0c-6f75-4e26-a296-4ff31f01dbce.png">


Machine language คือ
<img width="1440" alt="ภาพถ่ายหน้าจอ 2565-04-06 เวลา 21 11 22" src="https://user-images.githubusercontent.com/98943418/161994710-7c74707a-2ed4-42c3-a2a0-6fbb71196f81.png">

example 2 high level language คือ c++ ,Processor คือ RISC-v rv64gc clang 13.0.1 ได้ assembly คือ
<img width="1440" alt="ภาพถ่ายหน้าจอ 2565-04-06 เวลา 21 13 33" src="https://user-images.githubusercontent.com/98943418/161995470-8f090cf2-0496-4927-b42f-053604c059c3.png">

Machine language คือ
<img width="1440" alt="ภาพถ่ายหน้าจอ 2565-04-06 เวลา 21 16 07" src="https://user-images.githubusercontent.com/98943418/161995648-0182a12d-0f1f-4f71-84ea-7e09ba77084d.png">

