**Probabilistic Surrounding Keyboard Layout (PSKL)**

A precise solution to touchscreen typing errors that shifts the focus from predicting words using large linguistic dictionaries to calculating physical probability around the pressed key coordinates.

### An 8-Direction Surrounding Probability Framework for Reducing Touchscreen Typing Errors

A structural solution to touchscreen typing errors that focuses on local spatial probability around the target key, rather than relying solely on heavy global word-prediction dictionaries.

## Core Concept
* **Local Focus:** Minimizes computing overhead by analyzing only the "8 surrounding keys" of the target coordinate to eliminate spatial noise.
* **Weight Distribution:** Assigns maximum probability weight to the "left and right horizontal keys," where fat-finger errors from thumb-typing occur most frequently.
* **Universal Framework:** Built as a mathematical model applicable across all 8 major worldwide keyboard layouts (including QWERTY, Thai Kedmanee, Cyrillic, etc.) using the same core sensor logic.

### ระบบลดการพิมพ์ผิดด้วยหลักความน่าจะเป็นจากอักษรล้อมรอบ 8 ทิศทาง

แนวคิดการแก้ปัญหาการพิมพ์ผิดบนหน้าจอสัมผัส (Touchscreen) ที่ตรงจุด โดยเปลี่ยนจากการเดาคำล่วงหน้าในคลังคำศัพท์ขนาดใหญ่ มาเป็นการคำนวณความน่าจะเป็นเชิงกายภาพรอบปุ่มกด

## หลักการทำงาน (Core Concept)
* **Local Focus:** ระบบจะโฟกัสที่ "อักษรล้อมรอบ 8 ทิศทาง" ของปุ่มเป้าหมาย เพื่อตัดสัญญาณรบกวนเชิงพื้นที่
* **Weight Distribution:** ให้น้ำหนักความน่าจะเป็นสูงสุดกับ "2 อักษรในแนวระนาบ ซ้ายและขวา" เนื่องจากเป็นทิศทางที่นิ้วเกิดอาการนิ้วเบียดมากที่สุด
* **Spatial Correction:** เมื่อมีการกดเยื้องพิกัด ระบบจะคำนวณค่าน้ำหนัก (Weight) ระหว่างปุ่มหลักกับปุ่มล้อมรอบทันที ทำให้การตรวจจับความตั้งใจของผู้พิมพ์แม่นยำขึ้นโดยไม่ต้องพึ่งพาคำเดาที่ซับซ้อน
* **Universal Framework:** ระบบนี้สามารถนำไปประยุกต์ใช้กับแป้นพิมพ์มาตรฐานโลกทั้ง 8 ชุดได้อย่างสมบูรณ์ โดยใช้ Algorithm ชุดเดิม แต่อ้างอิงพิกัดล้อมรอบตามเลย์เอาต์นั้นๆ:
1. **Latin Layouts (3 ชุด):** QWERTY, AZERTY, QWERTZ (เน้นการลดสัญญาณรบกวนในแนวนอน)
2. **Phonetic Layout (1 ชุด):** Input คีย์บอร์ดซอฟต์แวร์ที่ใช้ฐานข้อมูลละติน
3. **Specific Scripts (4 ชุด):** ระบบอักษรไทย (เกษมณี/ปัตตะโชติ), เกาหลี (Hangul), รัสเซีย (Cyrillic), และ อาหรับ (Arabic)

* ## เจ้าของแนวคิด (Author)
* พัฒนาและคิดค้นโดยคุณ (Lovephet@gmail.com)
