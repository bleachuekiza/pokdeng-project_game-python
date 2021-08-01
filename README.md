# pokdeng-project_game-python

![GitHub Logo](https://shields.io/badge/Python-3-blue)

โปรเจคนี้เขียนขึ้นเพื่อเป็นการฝึกการเขียนโปรแกรมภาษา Python

# Updatelog
![GitHub Logo](https://shields.io/badge/Version-1.0-green)
 - ก๊อปปี้ข้อมูลเด็คมาจากต้นแบบ เพื่อไม่ให้กระทบกับเด็คหลักเมื่อผู้เล่นสุ่มหยิบไพ่
 - สุ่มไพ่ให้ผู้เล่น 2 ใบ และ บอท 2 ใบ สุ่มจากเด็คที่สร้างใหม่ และไม่สามารถได้ใบซ้ำกัน
 - เช็คแต้มของกาด, เอาไพ่ทั้งสองบวกกันและหาร 10 โดย 10 J Q K มีแต้มไพ่ท่ากับ 0
 - เช็คแต้มของผู้เล่น และบอท ว่าใครแต้มเยอะกว่าและเป็นผู้ชนะ หรือแต้มเสมอกัน และหากแต้มมากกว่าหรือเท่ากับ 8 จะถือว่าเป็นป็อก
 
 ![GitHub Logo](https://shields.io/badge/Version-1.1-green)
 - เพิ่มการสุ่มไพ่ใบที่ 3 ของผู้เล่นและบอท ถ้าหากไม่มีใครป็อกจะให้เลือกว่าจะสุ่มไพ่เพิ่มหรือไม่สุ่ม
 - เช็คป็อกเด้ง
 - แต้ม 8-9 จากไพ่ 3 ใบไม่ถือว่าเป็นป็อก ( 9 จากรวมแต้ม 3 ใบ แพ้ 9 จากรวมแต้ม 2 ใบ )
 
 ![GitHub Logo](https://shields.io/badge/Version-1.2-green)
- เช็คเด้ง(2-3), เรียงฟลัช, เรียง, สามเหลือง, ตอง

<!-- # Coming Soon
![GitHub Logo](https://shields.io/badge/NextUpdate->>>-orange) -->

# Rule Game
ประเภทไพ่ในมือ | จำนวนไพ่ | แต้ม | เด้ง | ไพ่ในมือ | แต้ม | เด้ง | ไพ่ในมือ | แต้ม | เด้ง | หมายเหตุ
------|------|------|------|------|------|------|------|------|------|------
ป๊อก | 2 | 8-9 | 1-2 | J♦ 9♥ | 9 | 1 | 9♠ 9♦ | 8 | 2
ตอง | 3 | - | 5 | 7♠ 7♥ 7♣ | 1 | 5 | K♣ K♦ K♥ | 0 | 5
เรียงฟลัช | 3 | - | 5 | 5♦ 6♦ 7♦ | 8 | 5 | 2♥ 3♥ 4♥ | 9 | 5 | Q♠ K♠ A♠<br>ไม่นับเป็นเรียง
เรียง | 3 | - | 3 | 2♠ 3♦ 4♣ | 9 | 3 | 7♣ 8♣ 9♥ | 4 | 3 | Q♣ K♠ A♥<br>ไม่นับเป็นเรียง
สามเหลือง | 3 | 0 | 3 | Q♣ J♣ J♦ | 0 | 3 | J♠ J♦ K♠ | 0 | 3 | K♣ K♠ A♥<br>ไม่นับเป็นสามเหลือง
ปกติ | 2-3 | 0-9 | 1-3 | A♣ 4♣ 5♣ | 9 | 3 | 5♥ 7♥ 7♠ | 9 | 1