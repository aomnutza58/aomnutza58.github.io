# What is a denial of service attack (DoS) ?

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/b25ddab1-b7dc-47a4-b0c3-593a37fce6fd)

## What is a denial-of-service attack?

A denial-of-service (DoS) attack is a type of cyber attack in which a malicious actor aims to render a computer or other device unavailable to its intended users by interrupting the device's normal functioning. DoS attacks typically function by overwhelming or flooding a targeted machine with requests until normal traffic is unable to be processed, resulting in denial-of-service to addition users. A DoS attack is characterized by using a single computer to launch the attack.

###### A distributed denial-of-service (DDoS) attack is a type of DoS attack that comes from many distributed sources, such as a botnet DDoS attack.

## How does a DoS attack work?

The primary focus of a DoS attack is to oversaturate the capacity of a targeted machine, resulting in denial-of-service to additional requests. The multiple attack vectors of DoS attacks can be grouped by their similarities.

### DoS attacks typically fall in 3 categories:

#### Buffer overflow attacks

the most common DoS attack. The concept is to send more traffic to a network address than the programmers have built the system to handle. It includes the attacks listed below, in addition to others that are designed to exploit bugs specific to certain applications or networks

#### ICMP flood

leverages misconfigured network devices by sending spoofed packets that ping every computer on the targeted network, instead of just one specific machine. The network is then triggered to amplify the traffic. This attack is also known as the smurf attack or ping of death.

#### SYN flood

sends a request to connect to a server, but never completes the handshake. Continues until all open ports are saturated with requests and none are available for legitimate users to connect to.

Other DoS attacks simply exploit vulnerabilities that cause the target system or service to crash. In these attacks, input is sent that takes advantage of bugs in the target that subsequently crash or severely destabilize the system, so that it can’t be accessed or used.

An additional type of DoS attack is the Distributed Denial of Service (DDoS) attack. A DDoS attack occurs when multiple systems orchestrate a synchronized DoS attack to a single target. The essential difference is that instead of being attacked from one location, the target is attacked from many locations at once. The distribution of hosts that defines a DDoS provide the attacker multiple advantages:

+ He can leverage the greater volume of machine to execute a seriously disruptive attack.
+ The location of the attack is difficult to detect due to the random distribution of attacking systems (often worldwide).
+ It is more difficult to shut down multiple machines than one.
+ The true attacking party is very difficult to identify, as they are disguised behind many (mostly compromised) systems.

Modern security technologies have developed mechanisms to defend against most forms of DoS attacks, but due to the unique characteristics of DDoS, it is still regarded as an elevated threat and is of higher concern to organizations that fear being targeted by such an attack.

## What are some historically significant DoS attacks?

Historically, DoS attacks typically exploited security vulnerabilities present in network, software and hardware design. These attacks have become less prevalent as DDoS attacks have a greater disruptive capability and are relatively easy to create given the available tools. In reality, most DoS attacks can also be turned into DDoS attacks.

A few common historic DoS attacks include:

+ Smurf attack - a previously exploited DoS attack in which a malicious actor utilizes the broadcast address of vulnerable network by sending spoofed packets, resulting in the flooding of a targeted IP address.
+ Ping flood - this simple denial-of-service attack is based on overwhelming a target with ICMP (ping) packets. By inundating a target with more pings than it is able to respond to efficiently, denial-of-service can occur. This attack can also be used as a DDoS attack.
+ Ping of Death - often conflated with a ping flood attack, a ping of death attack involves sending a malformed packet to a targeted machine, resulting in deleterious behavior such as system crashes.

## How can you tell if a computer is experiencing a DoS attack?

While it can be difficult to separate an attack from other network connectivity errors or heavy bandwidth consumption, some characteristics may indicate an attack is underway.

Indicators of a DoS attack include:

+ Atypically slow network performance such as long load times for files or websites
+ The inability to load a particular website such as your web property
+ A sudden loss of connectivity across devices on the same network

## What is the difference between a DDoS attack and a DOS attack?

The distinguishing difference between DDoS and DoS is the number of connections utilized in the attack. Some DoS attacks, such as “low and slow” attacks like Slowloris, derive their power in the simplicity and minimal requirements needed to them be effective.

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/302c71a7-8149-4880-98c1-c22284a6b002)

DoS utilizes a single connection, while a DDoS attack utilizes many sources of attack traffic, often in the form of a botnet. Generally speaking, many of the attacks are fundamentally similar and can be attempted using one more many sources of malicious traffic. Learn how Cloudflare's DDoS protection stops denial-of-service attacks.

# denial-of-service คืออะไร

## การโจมตีแบบ DDoS คือ อะไร

การโจมตีแบบ Distributed denial of service (DDoS) เป็นการโจมที่มีการควบคุมเครื่องผู้ใช้หลายๆ เครื่อง ซึ่งเรียกว่า botnet โจมตีไปยังเป้าหมายพร้อมๆ กัน เพื่อให้เครื่องเซิร์ฟเวอร์หรือเว็บไซต์ปลายทางล่มและไม่สามารถให้บริการผู้ใช้งานคนอื่นได้

การโจมตีแบบ DDoS อาจจะเกิดขึ้นในช่วงระยะเวลาสั้นๆ เช่น 5 นาที ไปจนถึง 40 นาที โดยเฉลี่ย แต่ผลกระทบที่เกิดขึ้นอาจสร้างความเสียหายให้กับองค์กรมากกว่านั้น เนื่องจากส่งผลกระทบต่อการใช้งานของลูกค้า ตลอดจนรายได้ในช่วงที่โดนโจมตี รวมไปถึงความน่าเชื่อถือ และภาพลักษณ์ขององค์กร

## การโจมตี DDoS ทำงานอย่างไร ?

การโจมตี DDoS หรือการโจมตีเป้าหมายจากหลายๆที่พร้อมกัน เป็นประเภทของการโจมตีทางไซเบอร์ที่ใช้ระบบที่ถูกบุกรุกหลายระบบเพื่อกำหนดเป้าหมายการโจมตีเช่น ระบบ, การบริการ หรือแอปพลิเคชัน การโจมตีสามารถทำได้จากคอมพิวเตอร์เครื่องเดียวหรือคอมพิวเตอร์หลายเครื่องที่ทำงานร่วมกัน

### ประเภทการโจมตีของ DDoS

####  Volumetric

การโจมตี DDoS เชิงปริมาตรเป็นประเภทของการโจมตี DDoS ที่ส่งปริมาณการใช้ข้อมูลจำนวนมากไปยังเป้าหมายเพื่อครอบงำทรัพยากรและออฟไลน์ การโจมตีเหล่านี้สามารถป้องกันได้ยากมาก เนื่องจากสามารถส่งปริมาณข้อมูลได้มากกว่าการโจมตี DDoS ประเภทอื่นๆ.

#### Application layer

การโจมตี DDoS ของชั้นแอปพลิเคชันเป็นประเภทของการโจมตี DDoS ที่กำหนดเป้าหมายชั้นแอปพลิเคชันของโครงสร้างพื้นฐานของเหยื่อโดยเฉพาะ การโจมตีประเภทนี้ทำได้ยากกว่าการโจมตี DDoS ประเภทอื่น แต่สามารถสร้างความเสียหายได้มากกว่า เนื่องจากสามารถกำหนดเป้าหมายแอปพลิเคชันและบริการเฉพาะที่มีความสำคัญต่อธุรกิจของเหยื่อ.

#### Flooding

Flooding เป็นชุดเดียวกับการโจมตี DDoS ที่ประสานกันทำงานซึ่งทำให้เป้าหมายรับข้อมูลอย่างท่วมท้นด้วยการรับส่งข้อมูลจำนวนมาก เพื่อทำให้หยุดการทำงาน การโจมตีเหล่านี้มีประสิทธิภาพมากในการทำลายเว็บไซต์และเซิร์ฟเวอร์ และอาจป้องกันได้ยาก.

#### SYN floods

Syn Floods เป็นการโจมตีประเภทหนึ่งของ Denial of Service (DoS) ซึ่งผู้โจมตีส่งแพ็คเก็ต SYN จำนวนมากไปยังระบบเป้าหมาย ระบบเป้าหมายตอบสนองโดยส่งแพ็คเก็ต SYN-ACK กลับไปยังผู้โจมตี แต่เนื่องจากผู้โจมตีปลอมแปลงที่อยู่ IP ต้นทางสำหรับแต่ละแพ็คเก็ต ระบบเป้าหมายจึงไม่สามารถระบุได้ว่าแพ็คเก็ต SYN-ACK ใดถูกต้อง และอันใดไม่ใช่ เป็นผลให้ระบบเป้าหมายใช้ทรัพยากรทั้งหมดตอบสนองต่อแพ็คเก็ต SYN ปลอม และการรับส่งข้อมูลที่ถูกต้องไม่สามารถรับการตอบกลับได้.

#### UDP floods

UDP Floods เป็นการโจมตีที่ส่งแพ็คเก็ต User Datagram Protocol (UDP) จำนวนมากไปยังระบบของเป้าหมาย ทำให้ผู้ใช้ทั่วไปไม่สามารถเข้าถึงการให้บริการหรือทรัพยากรได้ยาก UDP Floods ยังสามารถใช้เพื่อโอเวอร์โหลดแบรนด์สวิดท์เครือข่ายของระบบเป้าหมายเพื่อหวังผลให้หยุดการทำงาน.

#### ICMP floods

ICMP floods เป็นการโจมตี Denial of Service (DoS) ที่ใช้แพ็คเกต Internet Control Message Protocol (ICMP) จำนวนมากไปยังเป้าหมายด้วยข้อมูลที่ไม่ครบองค์ประกอบหรือไม่พึ่งประสงค์ เพื่อทำให้ระบบเป้าหมายขัดข้องหรือไม่สามารถใช้งานได้ การโจมตีชนิดนี้เป็นการโจมตี DOS ประเภทหนึ่งที่ใช้ระบบของผู้ใช้หลายระบบเพื่อให้เป้าหมายรับข้อมูลทราฟฟิกมากเกินไป ทำให้ไม่สามารถใช้งานได้กับผู้ใช้งานทั่วไป.

#### HTTP floods

การโจมตี http flood DDoS เป็นการโจมตีทางไซเบอร์ประเภทหนึ่งที่ใช้ปริมาณการรับส่งข้อมูลอย่างล้นหลามเพื่อทำลายเว็บไซต์หรือเซิร์ฟเวอร์ โดยปกติแล้ว การรับส่งข้อมูลจะถูกส่งผ่านอุปกรณ์ที่ถูกไฮแจ็กจำนวนมาก เช่น คอมพิวเตอร์ สมาร์ทโฟน หรืออุปกรณ์ IoT.

#### DNS floods

DNS floods เป็นประเภทของการโจมตี DDoS ที่โอเวอร์โหลดเซิร์ฟเวอร์ DNS พร้อมคำขอ DNS ป้องกันไม่ให้ตอบสนองต่อการรับส่งข้อมูลที่ถูกต้อง สามารถใช้เพื่อทำให้เว็บไซต์ออฟไลน์หรือเพื่อขโมยข้อมูลจากผู้ใช้ที่พยายามเข้าถึง

## วิธีระบุการโจมตี DDoS

มีหลายวิธีในการระบุการโจมตี DDoS แต่บางวิธีที่พบบ่อยที่สุดคือการตรวจสอบการใช้แบรนด์วิธ การสูญเสียแพ็คเก็ต และเวลาแฝง หากคุณสังเกตเห็นความผิดปกติใดๆ เหล่านี้ เป็นไปได้ว่าคุณอยู่ภายใต้การโจมตี DDoS.

สัญญาณที่พบบ่อยที่สุดที่รอการของการโจมตี DDoS 

+ แพ็คเก็ตสูญหายเพิ่มขึ้นอย่างกะทันหัน
+ เวลาในการตอบสนองเพิ่มขึ้นอย่างกะทันหัน
+ โฮสต์ที่ไม่สามารถเข้าถึงได้เพิ่มขึ้นอย่างกะทันหัน
+ การสืบค้น DNS เพิ่มขึ้นอย่างกะทันหัน
+ แพ็คเก็ตเพิ่มขึ้นอย่างกะทันหันด้วยที่อยู่ต้นทางปลอม

## วิธีป้องกันการโจมตี DDoS

มีหลายวิธีในการป้องกันการโจมตี DDoS แต่ที่พบบ่อยที่สุดคือการใช้ไฟร์วอลล์ ไฟร์วอลล์คือโปรแกรมที่ตรวจสอบการรับส่งข้อมูลทั้งหมดที่เข้าและออกจากคอมพิวเตอร์ของคุณ มันสามารถบล็อกการรับส่งข้อมูลบางประเภทหรือหยุดทั้งหมด คุณยังสามารถใช้โปรแกรมที่เรียกว่าระบบตรวจจับการบุกรุก ซึ่งจะตรวจสอบคอมพิวเตอร์ของคุณเพื่อหากิจกรรมที่ผิดปกติ หากตรวจพบบางสิ่ง ระบบจะแจ้งเตือนคุณเพื่อให้คุณสามารถดำเนินการได้.

+ ใช้ไฟร์วอลล์
+ กรองทราฟฟิกขาเข้า
+ ใช้ Content Delivery Network - Free Cloudflare plan
+ เพิ่มความแข็งแกร่งให้เซิร์ฟเวอร์ของคุณ
+ ตรวจสอบการรับส่งข้อมูลเครือข่ายของคุณ

## จุดประสงค์ของการโจมตีแบบ DDoS

แฮกเกอร์ที่โจมตีด้วย DDoS มายังเครื่องเซิร์ฟเวอร์ปลายทาง มีจุดประสงค์หลายๆ อย่างด้วยกัน คือ

+ โจมตีเนื่องจากไม่เห็นด้วยกับนโยบายต่างๆ ขององค์กรหรือเพื่อต่อต้าน หรือแสดงความไม่พอใจ
+ กลุ่มคนที่ต้องการแสดงความสามารถ ต้องการแสดงความสนใจต่อคนรอบข้าง
+ การข่มขู่หรือบังคับเพื่อต้องการเรียกร้องสิ่งใดสิ่งหนึ่ง
+ การแข่งขันทางด้านธุรกิจ ที่ต้องการสร้างความเสียหายให้กับคู่แข่ง
+ สงครามไซเบอร์ระหว่างภาครัฐและหน่วยงานที่เกี่ยวข้อง หรือระหว่างประเทศ ซึ่งอาจะได้รับการสนับสนุนจากพันธมิตรที่อยู่ในฝ่ายเดียวกันในการโจมตีฝ่ายตรงข้าม

## เปรียบเทียบการโจมตีแบบ DoS กับ DDoS

ข้อแตกต่างของการโจมตีแบบ DoS กับ DDoS คือ ปริมาณการโจมตี โดยการโจมตีด้วย DoS ธรรมดานั้น แฮกเกอร์จะใช้เครื่อง client เพียงเครื่องเดียวโจมตีผ่านทางช่องโหว่ของเครื่องปลายทาง หรือ flood เครื่องปลายทางด้วย request ปลอมจำนวนมากๆ เพื่อทำให้ resource ของเครื่องปลายทางไม่เพียงพอต่อการให้บริการผู้ใช้งานคนอื่นๆ เช่น RAM, CPU เป็นต้น

เมื่อเปรียบเทียบกับ DDoS ซึ่งจะเป็นการโจมตีจะมาจากเครื่อง client หลายๆ เครื่องกระจายอยู่ตามพื้นที่ต่างๆ และเป็นการยากที่จะเข้าไปแก้ไขหรือตรวจสอบในแต่ละเครื่อง เนื่องจากปริมาณการโจมที่ที่เยอะ

จุดแตกต่างอีกอย่างหนึ่งก็คือ การโจมตีแบบ DoS โดยส่วนใหญ่เป็นการใช้เครื่องมือหรือสคริปต์ในการสร้างทราฟฟิกปลอมเพื่อโจมตีไปยังปลายทาง ในขณะที่ การโจมตีแบบ DDoS นั้น เป็นการโจมตีจาก botnet ซึ่งเป็นเครื่องที่ติดมัลแวร์และกระจายอยู่ตามพื้นที่ต่างๆ และสามารถควบคุมการโจมตีจากแฮกเกอร์ได้

## ประเภทของการโจมตีแบบ DDoS

การโจมตีแบบ DDoS สามารถแบ่งออกได้เป็น 2 กลุ่มหลักๆ คือ การโจมตีในระดับ Application Layer และการโจมตีในระดับ Network Layer

+ การโจมตีในระดับ Network Layer หรือการโจมตีด้วยปริมาณ (Volumetric Attack) เป็นการโจมตีในระดับ Layer 3 – Layer 4 เช่น UDP flood, SYN flood, NTP amplification, DNS amplification เป็นต้น โดยสามารถตรวจจับได้จากการสังเกตเห็นว่ามีทราฟฟิกปริมาณมากผิดปกติ ที่ไม่มีเคยมาก่อน
+ การโจมตีในระดับ Application Layer เป็นการโจมตีในระดับ application ที่มีการใช้งาน โดยเน้นการโจมตีไปยังเซิร์ฟเวอร์โดยส่งคำร้องขอเป็นปริมาณที่มาก เพื่อทำให้ระบบทำงานช้าลง หรือหยุดทำงาน ไม่สามารถให้บริการได้ เช่น HTTP flood, DNS query flood เป็นต้น

## วิธีรับมือและป้องกันการโจมตีแบบ DDoS

เราไม่สามารถหยุดยั้งการโจมตีแบบ DDoS ไม่ให้เกิดขึ้นได้ เพราะเราไม่สามารถควบคุม botnet ที่แฮกเกอร์ใช้ได้ทั้งหมด แต่เราสามารถป้องกันไม่ให้การโจมตีนั้นสร้างความเสียหายให้กับ

+ ตรวจสอบและ monitor ทราฟฟิกอย่างต่อเนื่อง หากพบความผิดปกติ เช่น มีปริมาณทราฟฟิกเพิ่มมากขึ้นผิดปกติ หรือมี IP ที่มาจากต่างประเทศที่ไม่เคยมีประวัติการใช้งานมาก่อนเป็นจำนวนมาก อาจเป็นสัญญาณที่ระบบภายในองค์กรกำลังถูกโจมตีด้วย DDoS อยู่
+ ตรวจสอบและ update ข้อมูลข่าวสารทางด้าน Security อย่างสม่ำเสมอ ซึ่งอาจจะมีข้อมูลที่เกี่ยวข้องกับการโจมตีตลอดจนแนวโน้มต่างๆ ในธุรกิจที่เรากำลังดำเนินงานอยู่
+ พิจารณาใช้โซลูชันจำลองทดสอบการโจมตี เพื่อทดสอบ IT Infrastructure ขององค์กรว่าสามารถป้องกันการโจมตีได้หรือไม่
+ พิจารณาใช้โซลูชันป้องกันการโจมตีด้วย DDoS จาก NSFocus ที่สามารถตรวจสอบและป้องกันการโจมตีด้วย DDoS ได้อัตโนมัติโดยส่งผลกระทบต่อผู้ใช้งาน

### Cloudflare DDoS protection ทำงานอย่างไร?

Cloudflare ให้บริการป้องกัน DDoS ที่ช่วยบรรเทาผลกระทบจากการโจมตี DDoS ต่อเว็บไซต์ บริการนี้ทำงานโดยกำหนดเส้นทางการรับส่งข้อมูลทั้งหมดผ่านเครือข่ายทั่วโลกของ Cloudflare ซึ่งติดตั้งกลไกการป้องกัน DDoS ที่ซับซ้อน กลไกเหล่านี้รวมถึงเครือข่าย Anycast ทั่วโลก ซึ่งกระจายการรับส่งข้อมูลทั่วทั้งศูนย์ข้อมูลของ Cloudflare และระบบบรรเทา DDoS อัจฉริยะที่สามารถตรวจจับและบล็อกการรับส่งข้อมูลที่เป็นอันตราย.

##### วิธีหยุดการโจมตี DDoS

ไม่มีวิธีใดที่จะหยุดยั้งการโจมตีจาก DDoS ได้ เนื่องจากผู้กระทำผิดสามารถคิดค้นวิธีใหม่ๆ ในการทำให้เป้าหมายท่วมท้นด้วยการรับส่งข้อมูลจำนวนมหาศาล  อย่างไรก็ตาม มีบางขั้นตอนที่สามารถทำได้เพื่อลดทอนผลกระทบจากการโจมตี และหวังว่าจะหยุดมันก่อนที่จะสร้างความเสียหายมากเกินไป.

ขั้นตอนหนึ่งที่สามารถทำได้คือการเพิ่มแบนด์วิดท์ที่พร้อมใช้งานสำหรับไซต์เป้าหมาย ช่วยให้มั่นใจได้ว่าไซต์สามารถรองรับปริมาณการทราฟฟิคข้อมูลที่เพิ่มขึ้นและไม่หยุดให้บริการภายใต้ความกดดัน นอกจากนี้ยังสามารถใช้ไฟร์วอลล์และมาตรการรักษาความปลอดภัยอื่นๆ เข้าไปได้.

##### จะทำอย่างไรถ้าเว็บไซต์ของคุณอยู่ภายใต้การโจมตี DDOS

+ หากคุณกำลังประสบกับการโจมตีแบบ Distributed Denial of Service (DDoS) สิ่งแรกที่คุณต้องทำคือกำหนขอบเขตของการโจมตี
+ พยายามระบุแหล่งที่มาของการโจมตี ซึ่งอาจเป็นเรื่องยาก แต่สิ่งสำคัญคือต้องพยายามทำเพื่อหยุดการโจมตี
+ วางแผนการรับมือล่วงหน้าและทำตามขั้นตอนเพื่อปกป้องเว็บไซต์ของคุณจากการโจมตี ซึ่งอาจรวมถึงการเสริมความแข็งแกร่งให้กับมาตรการรักษาความปลอดภัยของคุณ หรือการใช้บริการ DDoS mitigation service.

เมื่อคุณกำหนดขอบเขตของการโจมตีได้แล้ว คุณสามารถเริ่มดำเนินการเพื่อลดการโจมตีได้ วิธีหนึ่งในการทำเช่นนี้คือการบล็อกการรับส่งข้อมูลที่มาจากที่อยู่ IP ที่ละเมิด คุณยังสามารถใช้เครื่องมือเช่น Cloudflare เพื่อช่วยปกป้องเว็บไซต์ของคุณจาก DDoS

Source : <a href="https://www.paloaltonetworks.com/cyberpedia/what-is-a-denial-of-service-attack-dos">paloaltonetworks</a>, <a href="https://www.cloudflare.com/learning/ddos/glossary/denial-of-service/">cloudflare</a>, <a href="https://www.techtalkthai.com/ddos-protection-from-nsfocus-by-nextwave/">techtalkthai</a>, <a href="https://www.bitdefender.co.th/post/ddos/">bitdefender</a>
