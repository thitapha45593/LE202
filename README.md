## ON OFF digital signal
1 ตัวอักษรเเทนด้วย 4 bit

## voltage (เเรงดันไฟฟ้า)
เป็นเเรงดันระหว่างจุด 2 จุด มี 2 ประเภท
   1. ไฟฟ้ากระเเสสลับ เช่น ไฟบ้าน
   2. ไฟฟ้ากระเเสตรง เช่น ถ่านไฟ อุปกรณ์ computer (สาย USB)

## computer 
-Arduino microcontroller (computer ตัวจิ๋วที่ใช้ในการเชื่อมโยง internet optic)
- มีควสามจุมาก เเละสามารถเชื่อมโยงผ่าน internet ด้วยความเร็วสูง

## internet สามารถโยงเครือข่ายได้ทั่วโลกด้วยการเชื่อมต่อ wifi เเละมีผู้ใช้มากเป็นล้านคน

## program language  
   จะเห็นได้ว่ามีมากมายหลายภาษาเช่น ภาษา C ,java, python
   
 ##microcontroller 
 -สามารถเขียนโปรเเกรมลงบน microcontroller ได้หลากหลายเเบบ เเละวิธีการเขียนโปรเเกรมก็สามารถเขียนได้หลายรูปเเบบ
 - platform io เป็นเครื่องมือหลักในการเขียนโปรเเกรม

## io set 
 จะเป็นการ dowload github
 
 ## run example 1
 - เขียน program ลงใน microcontroller โดยใช้ platform io 
 - การดูผลลัพธ์จาก microcontroller พิมพ์ "pio device monitor" out จะถูกแสดงผลทุกๆ 1 second 
 - ถ้าหากลอง reset microcontroller มันจะเริ่ม reset แล้วเริ่มนับ 1 ใหม่ run ไปทุกๆ 1 second

## run example 2 
 - การเตรียมการ upload program โดย program จะมี 2 ส่วน 
   1. void setup : run ครั้งเดียว
   2. void loop : run วนไปเรื่อยๆ เป็นการแสกนหา wifi

## run example 3 
 - เป็นการใช้ adeptor เสียบผ่าน microcontroller โดย adepter จะต่อสายออกมาเพื่อเป็นสายส่ง out put มีการต่อกับ LED เพื่อให้เปล่งแสง show การรับ output

## run relay
 - ใช้ relay มาเกี่ยวข้องเพื่อเปิดหรือปิด switch 
 - relay จะควบคุมสัญญาณ on-off ทุกๆครึ่งวินาที
 - การจ่ายไฟให้ relay สามารถนำ relay ไปต่อกับ powerbank หรือหัวชาร์จ สามารถใช้ controll switch ไฟบ้านได้

## run example 4 
 - เป็นการเอา program เข้าไป upload ใน microcontroller เมื่อ program run แล้ว จะ read เป็น 1 ตลอดเลย แสดงว่าติดไฟ 
   ถ้า input ขึ้นเป็น 1 = ติดไฟ
   ถ้า input ขึ้นเป็น 0 = ไม่ติดไฟ
 - เมื่อนำไปต่อกับ sensor ที่ต่ออยู่กับตัวต้านทาน
   หากเปิดหน้า sensor ไฟจะสว่าง read ออกมาเป็น 0
   หากปิดหน้า sensor ไฟจะมืด read ออกมาเป็น 1
   
## การสร้าง server ผ่าน wifi
 - เมื่อเขียน program แล้วก็ upload program ลงบน microcontroller (จะเป็นการเชื่อมโยงผ่าน wifi ที่มีอยู่แล้ว)

## run wifi AP
 - ในที่นี้จะเป็นการสร้าง wifi ขึ้นมาเอง ไม่มีความจำเป็นต้องใช้ wifi ที่ต่อไว้แล้ว สามารถใช้ wifi ใหม่จากมือถือของตนเองได้เลย
 - เมื่อเราสร้าง wifi และ upload ลง microcontroller แล้ว เราสามารถค้นหา wifi จากโทรศัพท์มือถือของเราเองได้
