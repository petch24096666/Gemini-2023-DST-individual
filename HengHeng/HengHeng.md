﻿Member 022 , 063 , 076 , 081 , 085

functional requirement

1. Astronomer
- Software ต้องมี programing environment ที่เพียงพอเพื่อให้สามารถดำเนินการได้
- สามารถเข้าถึง Programming Environment ได้ทั้งส่วนพัฒนา ทดสอบและปรับโปรแกรม
- ระบบต้องมี user interface ที่สามารถเก็บข้อมูล ผลลัพธ์ข้อมูล และสามารถประเมินข้อมูลได้
- ระบบ observe program ต้องเป็น Automate ทั้งหมด โดย interact กับ มนุษย์ให้น้อยที่สุด
- มีระบบ telescope simulator เพื่อสามารถ ทดสอบ program
- ระบบ telescope simulator ควรทำงานภายใน virtual telescope environment
- control software ต้อง support การใช้ระบบ simulator ใน virtual telescope
- ซอฟต์แวร์ต้องสามารถพิจารณาตําแหน่งเป้าหมายสภาพอากาศและกําหนดค่าเครื่องมือได้
- ระบบสามารถ access live view ได้
- ระบบต้องสนับสนุนการสังเกตจากระยะไกลในรูปแบบที่ผู้ใช้สามารถเลือกแสดงข้อมูลที่ต้องการ
- ระบบมีความสามารถในการตรวจสอบการทำงานของโทรทรรศน์จากระยะไกลโดยให้ข้อมูลในรูปแบบที่ผู้ใช้สามารถเลือกได้
- ระบบต้องมีความสามารถในการเก็บรักษาข้อมูลจากตัวตรวจในวิธีที่มีประสิทธิภาพที่สุดตามที่เทคโนโลยีที่ใช้งานอยู่อนุญาต
- ระบบต้องสนับสนุนการอ่านข้อมูลจากตัวตรวจในเวลาที่รองรับได้สูงสุดโดยที่ไม่ทำให้การเข้าถึงดิสก์และเวลาถ่ายโอนข้อมูลเกิดความเสียหาย
- ระบบต้องสนับสนุนการเข้าถึงข้อมูลพร้อมกันจากหลายแหล่งต่าง ๆ
- เครื่องตรวจจับแสงขนาดใหญ่(Mosaicked) จะต้องอ่านค่าเครื่องตรวจจับอย่างครบถ้วน
- ระบบต้องอนุญาตให้ส่งภาพได้อย่างรวดเร็ว


2. Science observer

- มีหน้าที่ในการ อนุมัติ science plan ต่างๆได้
- ระบบควรจะเป็นรูปเเบบ automated เพื่อทำให้การใช้งานสะดวกมากยิ่งขึ้น
- สามารถตรวจเช็คเเละทดสอบ science plan ได้ว่าสามารถใช้งานได้จริงหรือไม่
- มีระบบ observing program โดยนำข้อมูลมาจาก science planเเละเพิ่มเติมข้อมูลทางเทคนิคเพิ่มเข้าไปในprogram เช่น ข้อมูลของเลนส์ต่างๆ เงื่อนไขในการใช้งานอุปกรณ์
- สามารถเก็บ Data ที่ได้จากการถ่ายทอดดวงดาวได้ เพื่อใช้ในการตรวจสอบความถูกต้องของข้อมูล
- สามารถจัดการเกี่ยวกับข้อมูล Astronomer ได้ เช่นการ ลบ/เเชร์/ปรับเปลี่ยนข้อมูล
- สามารถควบคุมระบบ Telescope ได้
- สามารถสั่งใช้งาน science plan เพื่อใช้งานระบบได้
- User ควรสามารถสั่งใช้งาน ผ่าน user interface ได้เลย
- ระบบสามารถเเนะนำเเเละปรับเปลี่ยน Function ตามสถานการณ์ที่ผู้ใช้งานต้องการ 


3. Telescope Operator
- สามารถ validate of serving program ได้
- สามารถติดตั้ง Physical service เพิ่มได้ เช่น เพิ่ม lens
- สามารถที่จะออกคำสั่งโดยตรงไปยัง Telescope Control System (TCS) ได้ แม้จะอยู่ในการควบคุมของ planned observing program
- มีหน้าที่รับผิดชอบในการรักษาความสมบูรณ์และถูกต้องของ function ในระบบ
- สามารถดูภาพรวมของ Gemini 8m Telescopes operation ได้
- สามารถควบคุม Gemini 8m Telescopes ทางตรง(directly) ผ่าน command line เป็นคำสั่งใช้งานผ่าน OCS (การทำงานหลักของ commands อยู่ใน OCS)
- สามารถควบคุม Gemini 8m Telescopes ทางอ้อม(indirectly) ผ่าน scheduler program
- สามารถตรวจสอบประสิทธิภาพทั่วไปได้ และ รับรองความปลอดภัยระหว่างการทำงาน telescope operations
- มีสิทธิในการเข้าถึงทุก commands และ maintenance procedures ทั้งหมดในกรณีที่เกิดปัญหาขึ้น รวมทั้งการควบคุมโดยตรง physical units
- ในการทำงานปกติจะไม่อนุญาติให้เข้าถึง subsystems หากจำเป็นต้องเข้าถึงจะต้องกำหนดค่าใหม่(reconfiguration procedures)ที่เหมาะสม 
- เมื่ออยู่ใน update mode สามารถเข้าถึง operation tables ได้
- สามารถเปลี่ยน operational status ของ units ตามผลการทดสอบประสิทธิภาพของ units นั้นๆ
- ระบบสามารถใช้ remote control function เพื่อออกคำสั่งควบคุม telescope จากตำแหน่งอื่นที่ไม่ใช่ในพื้นที่ Telescope Operator's site ได้
- สามารถเปิดใช้งานการดำเนินการแบบโต้ตอบโดยตรงได้ แต่จะไม่ถือเป็นโหมดการทำงานปกติ
- มีสิทธิในการเปลี่ยนแปลง environment โดยการเลือกใช้เครื่องมือที่เหมาะสมร่วมกัน


4. Support 
- มี Built-in Tests ที่ verify การทำงานของ Gemini 8m Telescopes system, software ซึ่งประกอบไปด้วย 
  1. Modules ที่ทดสอบ normal operation of releases
  2. Executable self-test sequences 
  3. Regression Tests  
- Remote Software & On-Site Software ควรทำงานเหมือนกัน
- Gemini Software มี Flexible Scheduling 
- มี Offline data reduction packages เช่น ADAM, IRAF, Midas, IDL, Khoros
- Quick-Look Analysis จะถูกทำผ่าน PV-Wave / IDL
- Data storage & Transport จะอยู่ใน format ของ FITS
- Online access จะใช้ STARCAT
- Self-Check levels ต่อไปนี้จะต้องใช้ sub-system software
     1. Monitor Level
     2. Self-test Level
     3. System Level
- Maintenance at Organizational Level จะต้องถูกทำด้วย situ ในช่วงที่มีการทำ observing session และมีการใช้ unit replacement, module replacement
- Maintenance at Intermediate Level จะถูกทำที่ Base Facility และมีการใช้ module replacement
- Maintenance at Depot Level จะถูกทำที่ Base Facility ละมีการใช้ module repair
- Maintenance at Contractor จะถูกทำที่ Contractor / Vendors และมีการ repair / replace


5. Administrator
- ระบบจะต้องควบคุม high level function
- ระบบต้องสามารถกำหนด และจัดการผู้ใช้ User management.                 
- ระบบต้องสามารถกำหนดระดับของการทำงาน (operation Level)
- ระบบจะต้องสามารถบริหารจัดการ observation value ได้
- ระบบต้องสามารถบำรุงรักษาตามกำหนดเวลา (Scheduled Maintenance Tasks ) \* (เวลาที่ไม่ได้ทำการสังเกตการณ์)
- ระบบต้องสามารถรับข้อมูลและส่งข้อมูล (Data input/output)
- ระบบต้องสามารถกำหนดเวลาที่ระบบจะถูกรีเซ็ตหรือปิดระบบ (Shutdown time)
- ระบบต้องสามารถกำหนดเวลาที่จะทำการบำรุงรักษา (maintenance down-time)
- ระบบต้องสามารถกำหนดเวลาที่ระบบจะเปิด-ปิด
- ระบบต้องสามารถทำการวิเคราะห์และแก้ปัญหาที่เกิดขึ้นในระบบ (system Diagnostics)
- ระบบต้องสามารถแสดงสถานะของอุปกรณ์ที่ใช้งาน
- ระบบต้องสามารถแสดงสถานะทั่วไปของระบบ
- ระบบต้องสามารถให้เข้าถึงระดับผู้ดูแลระบบ(Maintenance level)
- ระบบต้องมีความสามารถในการทำการบำรุงรักษาทางไกล (Remote Maintenance Capability)
- ระบบจะต้องสามารถควบคุมการสังเกตการณ์ช่วงเวลานั้นๆ ณ ปัจจุบัน (Real-time Observation Control)
- ระบบจะต้องสามารถปรับเปลี่ยนระบบได้ (system modifications)
- ผู้ใช้จะต้องสามารถสอบถามข้อมูลเกี่ยวกับระบบได้



non-functional requirement

- ระบบควรมีประสิทธิภาพ (Performance) ความต้องการให้ระบบมีประสิทธิภาพสูงเพื่อดำเนินการทุกประการโดยมีประสิทธิภาพ
- ระบบควรมีความเชื่อถือและความพร้อมใช้งาน (Reliability and Availability) การต้องการให้ระบบมีความเชื่อถือสูงและพร้อมใช้งานตลอดเวลา
- ระบบควรมีความสามารถในการบำรุงรักษา (Maintainability) ความต้องการให้ระบบมีความสามารถในการบำรุงรักษาและอัปเกรดอย่างง่าย
- ระบบควรมีความสามารถในการทดสอบ (Testability)ความต้องการให้ระบบมีความสามารถในการทดสอบอย่างง่าย
- ระบบควรมีความสามารถในการขยายขนาด (Expandability) ความต้องการให้ระบบมีความสามารถในการขยายขนาดตามความต้องการเพิ่มเติม
- ระบบควรมีการทำงานพร้อมกัน (Concurrency) ความต้องการให้ระบบสามารถทำงานพร้อมกันได้

1. Astronomer
- ระบบควรมีการตอบสนองของ interface ที่ทำให้ผู้ใช้งานพึงพอใจ
- Software ควรที่จะใช้งานง่าย
- สามารถเข้าถึง Programming environment ได้ทั้งพร้อมกันและไม่พร้อมกัน
- Programming environment ควรสามารถรองรับข้อความพิเศษ คำสั่ง และความคิดเห็นที่อาจใช้เทคนิคหลายอย่าง
- ระบบ Simulation ควรที่จะบอกเงื่อนไขของระบบ telescope ของจริงเพื่อให้การทดสอบแม่นยำ
- การส่งภาพต้องตรงกับความละเอียดดั้งเดิมโดยต้องใช้เวลาน้อยกว่า 20 วินาที
- เวลาที่รองรับสูงสุดสำหรับการอ่านข้อมูลจากตัวตรวจสำหรับการโฟกัสและกิจกรรมที่เกี่ยวข้องประมาณ 0.1 วินาที
- การถ่ายโอนข้อมูลระหว่างระบบ virtual telescope และเครื่องมือที่เชื่อมต่อต้องมีความต้องการในการถ่ายโอนที่สูงถึง 20-40 Mbits/second


2. Science observer
- ระบบสามารถเข้าถึงการใช้งานได้ง่าย เข้าใจง่ายเเละ ไม่ซับซ้อนในการใช้งาน
- ระบบสามารถให้ผู้ใช้งานเเสดงความคิดเห็นได้ เพื่อนำคำติชมไปพัฒนาระบบในอนาคต
- ระบบสามารถสลับfunction ระหว่าง กลางวันเเละกลางคืนได้
- ระบบมีความเสถียรในระหว่างการใช้งาน
- ระบบที่ช่วยในการทำงานควรใช้ได้ทั้งใน เเละนอกสถานที่
  

3. Telescope Operator
- ระบบควรควบคุมง่าย และตอบสนองอย่างรวดเร็วในสถานการณ์ที่ไม่ปลอดภัย 
- ระบบสามารถตรวจสอบระบบย่อยทั้งหมดได้ตามต้องการ
- สามารถเข้าถึงระบบได้หลากหลาย modes พร้อมกันผ่าน observer, monitor และ operator modes
- ผู้ใช้งานควรเป็นผู้ที่มีประสบการณ์สูง
- ระบบควรกำหนด single point of control และความรับผิดชอบ ในสิทธิ์การเข้าถึงของ operations staff
- ควรมีการตรวจสอบตัวเลือกสำหรับระบบอัตโนมัติในแต่ละ instance ของฟังก์ชัน
- การเข้าถึงคำสั่งการควบคุมจากระยะไกลควรได้รับอนุญาต โดยมีมาตรการความปลอดภัยเฉพาะจากเจ้าหน้าที่ เช่น การมีปุ่ม "หยุด" ที่เชื่อมต่อแบบสาย, วิดีโอและเสียงแบบเรียลไทม์, และการควบคุมกล้องโทรทรรศน์
- operations staff มีเจ้าหน้าที่ส่วน 'night assistants' และ 'operations group' รวมอยู่ด้วย

  
4. Support 
- ระบบควรมี downtime จากการ maintenance ให้น้อยที่สุด
- ระบบควรมีข้อผิดพลาดที่เกิดจากการ maintenance ให้น้อยที่สุด
- Workstations ควรเป็นแบบ State-of-the-art system ที่ scalable 
- Workstations ควร match กับ software standards


5. Administrator
- ระบบต้องง่ายต่อการใช้งานจะต้องนำเสนอข้อมูลสถานะในรูปแบบที่ทำให้ผู้ดูแลเข้าใจได้ง่ายและชัดเจน
- ความปลอดภัย (Security) ต้องให้ระบบมีมาตรการความปลอดภัยที่เหมาะสมเพื่อปกป้องข้อมูลและการเข้าถึงที่ไม่ได้รับอนุญาต

