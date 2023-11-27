# Authentication

### What is authentication?

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/803c1552-7787-4a07-8f5f-c6aeafca1a50)

In cyber security, authentication is the process of verifying someone's or something's identity. Authentication usually takes place by checking a password, a hardware token, or some other piece of information that proves identity. Just as an airline worker checks a passport or an identification card to verify a person's identity when they board a plane, computer systems need to be sure a person really is who they say they are. At an airport, this authentication process ensures only people with a ticket get on the plane; for digital systems, this ensures data is viewed and used by the right people.

Authentication does not just apply to verifying human users. Computer systems also need to check servers, software, APIs, and other computers to be sure they are who they "say" they are.

### What is the purpose of authentication?

Authentication is used to verify that you are who you say you are. After a user’s identity is confirmed, for instance with a username and password, that identity may be used in an authorization policy to determine the appropriate access privileges. Organizations today must ensure that the right users are given access to the right resources, whether it is physical or--increasingly--digital.

### How is authentication used in a security context?
Authentication is an important part of identity and access management (IAM), which dictates who can view data and what they can do with it. But it applies to many other areas of security as well, including:

+ TLS: Almost all major websites today support Transport Layer Security (TLS). TLS, among other functions, authenticates the identity of a web server to ensure user devices do not load fake websites.
+ APIs: Most modern web applications rely on APIs in order to function. Properly secured APIs authenticate both endpoints of the API integration in order to prevent attacks directed at those APIs.
+ Email: Emails are authenticated using a process called DomainKey Identified Mail (DKIM). DKIM helps ensure email messages come from servers that are allowed to use the domain (e.g. @cloudflare.com) that the email comes from. Non-authenticated email messages are likely to end up in spam folders.

### How does authentication work?

Because a computer cannot "recognize" a person or another computer the way a human can, the process of authentication relies on objective criteria that a computer can measure. One type of objective criteria involves checking for some quality that the person or computer in question is known to have. Another involves the use of a technology called public key cryptography to prove identity.

#### Verifying identity via authentication factors

This type of authentication involves checking a measurable characteristic of identity against a corresponding digital record. The characteristics that an authentication system will check are called "factors." Three common authentication factors are widely used today:

##### 1. Something the person knows

This authentication factor checks a piece of secret knowledge that only the real person should have. A username-and-password combination is the classic example of this factor. Security questions and PIN codes also are examples.

##### 2. Something the person has

This authentication factor checks if the person possesses a physical item they were issued or are known to have. Many people use this authentication factor every day: they live in a house or an apartment that they can unlock with a metal key. Possession of this key, therefore, proves they are authorized to enter the premises, and enables them to do so.

In digital systems, this authentication factor does not rely on an old-fashioned lock and key. But it uses a similar principle by checking for a physical token. There are two types of tokens: soft tokens and hard tokens.

###### Soft tokens: A soft token involves verifying possession of a device, like a smartphone, by sending a code to that device and asking the user to enter it. The code may be sent as a text message or through an app that generates random codes.

###### Hard tokens: A hard token is a small physical item that connects to a computer or mobile device via Bluetooth, a USB port, or some other port. Users must plug this token into their device to verify their identity.

Some security experts consider hard tokens more secure than soft tokens. An attacker could remotely intercept a code on its way to a user's phone and use that code to impersonate the user. But it is much harder to steal a hard token: the attacker needs to physically access the token in order to do so.

##### 3. Something the person is

This authentication factor assesses a person's inherent qualities. In real life, people do this all the time — two friends may recognize each other by their appearance or manner of speaking, for instance. A computer could do the same by scanning a person's face or retina, verifying their thumbprint, measuring the frequencies of their voice, or checking the results of a blood test (although this last one is more rare).

##### Additional authentication factors

Some members of the security industry have proposed or used additional authentication factors besides the three main ones listed above. Two of these additional factors are location (where a user is) and time (when they are accessing the system).

### Verifying identity via digital certificates

In addition to using the authentication factors described above, known and trusted entities can also be issued digital certificates. A digital certificate is a small digital file that contains information for verifying identity, just as an ID card contains information that verifies a person's identity in real life.

Digital certificates receive a digital signature to prove their authenticity from the authority that issues them, like how a passport, ID card, or piece of paper currency may have a watermark proving it is not counterfeit.

A digital certificate also contains a string of random values called a public key. The public key corresponds to a private key that is stored separately. The entity that has the certificate can digitally sign data with these keys to prove that it possesses the private key and is therefore authentic.

Currently, digital certificates are not often used to verify the identity of individual people. But most people rely on digital certificates every day without realizing it.

Whenever someone loads a website that uses HTTPS, the secure version of HTTP, the TLS protocol uses the website's digital certificate (called an SSL certificate or TLS certificate) to authenticate the website. DKIM, which authenticates email senders, is another example of a technology that uses this method instead of checking authentication factors. DKIM helps email providers sort and block spam emails.

### What are the different authentication protocols?

Network authentication protocols are used to help securely transfer identity credentials for authentication between the subject (user or device) and the authentication server. There are several different authentication protocols for network access control, including:

+ Kerberos
+ Extensible Authentication Protocol (EAP)
+ IEEE 802.1X
+ Remote Authentication Dial-In User Service (RADIUS)
+ Terminal Access Controller Access-Control System (TACACS)

### What is multi-factor authentication (MFA)?

Multi-factor authentication (MFA) is the process of verifying a person’s identity by checking two or more authentication factors, rather than just one. MFA is a stronger type of authentication than single-factor authentication, because it is much harder to fake two of these factors than it is to fake one of them.

An attacker might be able to steal Bob's username and password (perhaps through a phishing attack). But if Bob has to scan his face as well, the attacker will not be able to fake Bob's identity, since their face does not look like Bob's face. Or, if Bob has to plug a hard token into his computer in addition to entering his password, the attacker would have to steal this token as well. While possible, such a theft is much more difficult, making account takeover less likely.

For true MFA, separate factors have to be checked. Assessing multiple instances of one factor is not MFA. For instance, if an application has a user enter a password and answer security questions to authenticate, this is still single-factor authentication. Password entry and security questions both assess the "something you know" factor.

Because of the increased security it offers, MFA is a core principle of Zero Trust security, a security model that requires identity verification for every user and device that accesses a private network.

### What is two-factor authentication (2FA)?

Two-factor authentication (2FA) is what MFA is called when exactly two factors are used. The most common type of two-factor authentication is "something you know" + "something you have." For instance, in addition to entering their passwords, many people have codes sent to their phones before they can access their bank accounts (an example of the "soft token" version of this factor).

Today, many businesses are employing 2FA in order to reduce the impact of phishing attacks. For example, Google was able to eliminate account takeover attacks by using 2FA with hard tokens for authentication.

### What is the difference between authentication and authorization?

While authentication is concerned with verifying identity, authorization is concerned with permissions, or what someone is allowed to do once they gain access to a protected system or resource.

Suppose Bob works in his company's marketing department. Bob enters his password, scans his face, and inserts his hard token to log in to his company's network. At this point, authentication is complete.

After logging in, Bob does not have access to every data file in the company's possession. Authorization determines what Bob can and cannot see. As a marketer, he is authorized to see some data, like a list of potential customers to whom the company will send marketing messages, but not other data, like the company's main codebase or its list of employee salaries.

### What is single sign-on (SSO)?

Modern corporate employees have to authenticate to many different cloud-based applications. This forces those employees to establish many sets of authentication factors — one set for each application — and creates potential security concerns:

+ One application with weak security could enable an attacker to compromise that application, then move laterally, compromise the user's other application accounts, and spread to the rest of the organization.
+ Requiring users to sign in to multiple applications gives them incentive to stop following good security practices. A user may start using weak passwords or the same password for every application, since it can be challenging to memorize multiple randomized 16-digit passwords.

Single sign-on (SSO) is a service that enables users to authenticate only once. Users sign in to the SSO service, which then passes on this authentication to every application by sending a digital authentication message to each application as needed.

SSO also gives IT teams a single point at which to enforce security policies. Not all applications support 2FA, but if the SSO service supports it, then 2FA can be used anyway. IT teams can also enforce requirements for password length and complexity via an SSO service, putting less of a burden on users to remember multiple passwords.

### What is Security Assertion Markup Language (SAML)?

SSO authentication messages use a protocol called Security Assertion Markup Language (SAML). SAML is a standardized method for telling external applications that a user is who they say they are.

A message authenticating a user is called a SAML "assertion." Once an application receives a SAML assertion for a user, it does not need to authenticate the user on its own, because it knows the SSO service has already done this.

### SAML vs. OpenID Connect (OIDC)

OpenID Connect (OIDC) is another authentication protocol that is growing in use by SSO providers. OIDC functions similarly to SAML, but it formats data differently, among other distinctions; while SAML formats data via XML, OIDC uses JSON.

### How do I benefit from a user authentication policy?

A user authentication policy may be used to help ensure that only the intended audience is accessing certain assets in your organization. User authentication policies strive to ensure that the person requesting sensitive information and data is the right person to access that information.

# Authentication คืออะไร

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/d078299c-dd07-412c-ac04-7f71080b7a57)

### Authentication

Authentication คือ ระบบการยืนยันตัวตนที่เมื่อเราจะเข้าใช้งานในเว็บไซต์ แอปพลิเคชั่นหรืออะไรก็ตามบนโลกออนไลน์ พูดง่ายๆก็คือ การ Log- in นั้นเองเช่น การเข้าสู่ระบบ Email, การเข้าสู่ระบบ Internet Banking และการเข้าสู่ระบบ social media ต่างๆ เพื่อเป็นการยืนยันตัวตนว่าเราคือคนๆนี้และกำลังจะใช้บริการต่างๆในฐานะคนนี้ พร้อมทั้งทำการตรวจสอบสิทธิ์ว่าผู้ใช้งานระบบนั้นมีสิทธิ์ใช้ได้และเป็นเจ้าของข้อมูลเหล่านั้นจริงๆ โดยการยืนยันนั้นก็จะมีการใส่ Username และ Password ไม่ว่าจะเป็นแบบที่เรากำหนดตั้งเองหรือแบบที่ระบบกำหนดมาให้เราใช้ตาม มันมีชื่อเรียกสั้นๆว่า AuthN.

#### การทำ Authentication มี 2 แบบ

##### 1. การระบุตัวตน (Identification)

คือผู้ใช้งานนั่นระบุว่าตนเองคือใครผ่านการล็อคอินโดยใช้ username และ password ซึ่งเป็นวิธีพื้นฐานที่หลายๆเว็บไซต์ หลายๆแอปพลิเคชั่นทำกัน

##### 2. การพิสูจน์ตัวตน (Authentication)

คือ ขั้นตอนที่ตรวจสอบหลักฐานเพื่อแสดงว่าเป็นบุคคลที่กล่าวอ้างจริง เป็นการยืนยันตัวตนอีกรอบ ใช้ในเวลาที่เราใช้แอปธนาคารในการทำธุรกรรมทางการเงิน ซึ่งมักจะใช้ในการยืนยันตนที่ต้องการความปลอดภัยขั้นสูง ซึ่งในปัจจุบันนั่นก็มีอีกหลายวิธีมากมายที่จะยืนยันตัวของเราได้อย่างปลอดภัยและมั่นใจว่าจะไม่มีใครเอา username และ password ของเราไปใช้ได้ เช่น การใช้ระบบ Biometric การสแกนลายนิ้วมือ การสแกนใบหน้าหรือรูม่านตาเป็นต้น แต่วิธีที่ดีรับความนิยมมาก การยืนยันการทำรายการโดยการกรอกรหัส OTP (One Time Password) นั่นเอง

#### ขั้นตอนการทำงานของ Authentication 

+ Identification เป็นการระบุตัวตนที่บุคคลนำมาแสดงว่าตนเองเป็นใคร เช่น Username, UserID
+ Authentication เมื่อบุคคลทำการแสดงตนว่าเป็นใครแล้ว ก็จะทำการตรวจสอบหลักฐานเพื่อแสดงว่าเป็นบุคคลที่กล่าวอ้างนั้นจริงไหม เช่น Password หรือสิ่งอื่นใดที่สามารถยืนยันตัวบุคคลได้พวก Private Key หรืออัตลักษณ์ของบุคคล

ซึ่งในขั้นตอนของการ Authentication นั้น สำหรับการตรวจสอบหลักฐานเพื่อแสดงว่าเป็นบุคคลที่กล่าวอ้างนั้นจริงนั้นจะประกอบไปด้วยหลายวิธี โดยใช้หลักฐานต่างๆ กันออกไปแล้วแต่วิธีการ โดยส่วนมากในหนังสือหลายๆเล่มระบุไว้ 3 วิธี บ้างที่ก็ 5 วิธี วันนี้ผู้เขียนจะมาอธิบาย 3 ละกันนะครับ เพราะ 3 วิธีนี้มันเป็นวิธีที่เพื่อนน่าจะรู้จัก (Well-Know)และคุ้นชินกับการใช้งานมันดีอยู่แล้ว เพื่อตอนนำไปใช้งานจะได้เข้าใจมากขึ้น

+ Something you know มันคืออะไรที่เรารู้เราจำมันได้ เอ๊ะจำมันได้จริงไม่นะ 555+ ปกติลืมตลอด และเป็นวิธีที่ Basic ทุกระบบ ทุก App จะต้องมีและใช้กันมาจนถึงปัจจุบัน มันก็คือ​ Password​ หรือ​ PIN​ นั้นเอง
+ Something you have มันคือสิ่งที่เรามีและโดยมากจะนึกถึงสิ่งที่เราสามารถพกมันติดตัวได้​ เช่นพวกบัตร Credit, Debit หรือพวก​บัตรประชาชนก็ได้ แต่สิ่งที่ผู้เขียนเองใช้อยู่และและพบเห็นได้บ่อยเลยคือพวก​ Software token และ​ Hardware token ที่ใช้กันอย่างแพร่หลายในการ Authentication
+ Something you are มันก็คือการนำข้อมูลทางชีวภาพ (Biometric) ไม่ว่าจะเป็นลักษณะ เฉพาะทางกายภาพหรือพฤติกรรม มาใช้ในการตรวจสิทธิเพื่อรับรองความถูกต้อง เช่น ลายนิ้วมือ ฝ่ามือ เสียง ม่านตา เรตินา ใบหน้า ดีเอ็นเอ ลายเซ็น​ อะไรก็ตามแต่ที่มันสามารถระบุได้ว่าเป็นตัวเรานั่นเอง​

#### ความสำคัญของการพิสูจน์ตัวตน

โดยในขั้นตอนของการ Authentication ดังที่อธิบายมาทั้ง 3 วิธีนั้นสามารถนำมาใช้พร้อมกันได้เลยนะครับ แต่ทั้งนี้ก็ขึ้นอยู่กับการใช้งานของเราเอง และตัวระบบว่าสามารถรองรับวิธีการไหนนี้ได้บ้าง แต่ขอแนะนำเพื่อนๆว่าไม่ควรนำมาใช้เพียงวิธีใดวิธีหนึ่ง เพราะมันไม่ค่อยมีประสิทธิภาพ คือสมมติถ้าเราใช้แค่ Password อย่างเดียว (Single factor Authentication) ถ้าเกิด Hacker ขโมยหรือเดา Password เราได้เขาก็จะสามารถปลอมเป็นตัวเรา และเข้าไปทำโขมยข้อมูลและเงินของเราได้

ดังนั้นควรนำแต่ละคุณลักษณะมาใช้ร่วมกัน แต่บ้างระบบที่เราใช้อาจจะมีการ Design แบบ Multi-factor Authentication มาให้เราแล้วเช่นพวก App เกี่ยวกับเงินๆๆทองๆ เช่นเมื่อเราอยากโอนเงินให้ใครสักคน App Mobile Banking จะตรวจสอบว่าเบอร์มือถือที่ใช้ตรงกับที่ผูกไว้กับ Userไหม ซึ่งเท่ากับการป้องกันชั้นแรก something you have คือเรามีซิมที่ผูกกับเบอร์มือถือและเมื่อเราจะเข้า App หรือตอนโอนเงิน เราก็ต้องใส่ PIN เป็นชั้นที่สองเรียกว่า something you know หรือบาง App ของธนาคารอาจจะใช้ลายนิ้วมือเป็นชั้นที่สองก็จะเป็น something you are ซึ่งการนำแต่ละลักษณะของการพิสูจน์ตัวตนมาใช้ร่วมกันมากกว่า 1 ลักษณะ จะช่วยเพิ่มประสิทธิภาพในการรักษาความปลอดภัยได้ดียิ่งขึ้นนะครับ

##### ประเภทของการพิสูจน์ตัวตน (Authentication Types)
จากที่ได้กล่าวไปซะยาวก่อนหน้าแล้วว่าการพิสูจน์ตัวตนนั้นถือว่ามีความสำคัญที่สุดกับการเข้าใช้ระบบอย่างไร ถึงตรงนี้เรามาดูต่อกันว่าการพิสูจน์ตัวตนที่เขานิยมใช้กันอยู่ในปัจจุบันมีอะไรบ้างและแต่ละชนิดมีลักษณะอย่างไร​

+ การพิสูจน์ตัวตนโดยใช้รหัสผ่าน (Password-based authentication)
รหัสผ่านเป็นวิธีการพิสูจน์ตัวตนที่ใช้มานานและพบบ่อยที่สุดละ โดยที่รหัสผ่านจะประกอบไปด้วยตัวอักษร ตัวเลขหรืออักขระพิเศษ แต่อย่างไรก็ตามวิธีนี้ก็ถือว่าไม่ค่อยปลอดภัยมากเท่าที่ควร หากนำมาใช้งานแค่รหัสผ่านอย่างเดียวตามที่กล่าวไปแล้วก่อนหน้า เนื่องจากคนทั่วไปมักมี User หลายๆ User ทำให้มีรหัสผ่านจำนวนมากที่ต้องจำ ส่งผลให้หลายคนตั้งรหัสผ่านที่ใกล้ๆตัวเราแทน เช่นชื่อตัวเอง ชื่อแฟน วันเดือนปีเกิด เป็นต้น เพื่อที่จะได้จำได้ง่าย ๆ และก็จะตั้งรหัสผ่านเดียวแล้วใช้กับหลาย ๆ User ด้วยก็จะมีความเสี่ยงขึ้นไปอีก ควรใช้ Password Manager มาจัดการแทนดีกว่าครับ
+ การพิสูจน์ตัวตนโดยใช้ PIN (PIN authentication)
PIN (Personal Identification Number) เป็นรหัสลับส่วนบุคคลที่ใช้เพื่อเข้าสู่ระบบ ซึ่ง PIN โดยมักจะถูกออกแบบมาให้ใช้ประกอบกับ Factor อื่นอยู่เสมอ เพราะตัวมันเองอย่างเดียวจะประกอบไปด้วยตัวเลขไม่กี่ Digit เช่น 4 หรือ 6 เป็นต้น ตัวอย่างการทำธุรกรรมทางด้านธนาคาร โดยนำ PIN ไปใช้ร่วมกับ Factor อื่นเพื่อเพิ่มความปลอดภัยยิ่งขึ้น เช่นบัตร ATM และ Credit Card เป็นต้น
+ การพิสูจน์ตัวตนโดยใช้รหัสผ่านที่ใช้เพียงครั้งเดียว (One-Time Password: OTP)
เป็นรหัสผ่านที่สามารถนำมาใช้ได้เพียง 1 ครั้ง และหลังจากนั้นรหัสผ่านนี้ก็จะไม่สามารถนำมาใช้ได้อีก เช่น OTP แรกที่ได้รับคือ “246810” ในเวลาต่อมาหากมีการทำรายการอีกครั้ง OTP จะเปลี่ยนเป็นเลขอื่นที่ไม่ใช่ “246810” อีกต่อไป ฉะนั้นจึงเป็นการยากต่อผู้อื่นในการที่จะคาดเดาได้ว่า OTP ของเราคือรหัสอะไร และมักจะนำ OTP มาให้ใช้ประกอบกับ Factor อื่นอยู่เสมอเช่นกัน
+ การพิสูจน์ตัวตนโดยอัตลักษณ์ของบุคคล (Biometric authentication)

  ![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/dcedfbc1-e5b4-4ae7-b8ea-c3fffb9da3a3)

เป็นการใช้ข้อมูลอัตลักษณ์ทางกายภาพของบุคคลซึ่งเป็นลักษณะเฉพาะและลอกเลียนแบบกันไม่ได้ เช่น ใบหน้า ลายนิ้วมือ หรือพฤติกรรมของผู้ใช้ จึงมีการนำเทคโนโลยีนี้มาช่วยในการพิสูจน์ตัวตน เพื่อเพิ่มความปลอดภัยก่อนเข้าสู่ระบบ เช่น การใช้ควบคู่กับการใช้รหัสผ่านในการเข้าสู่ระบบ

+ Software & Hardware Token ที่ใช้สร้าง รหัสผ่านซึ่งมันจะมีการเปลี่ยนแปลงอยู่ตลอดเป็น​ Dynamics Password โดยแบ่งวิธีการดังนี้​ การพิสูจน์ตัวตนแบบ​ synchronous แบ่งออกเป็น 2 ประเภทตามลักษณะของการใช้งาน คือ
การพิสูจน์ตัวตนแบบ​Event-synchronous Authentication เมื่อเราต้องการที่จะเข้าสู่ระบบ เราก็จะต้องกด Token เพื่อให้ Token มัน​ Generate รหัสผ่านให้ จากนั้นนำรหัสผ่านที่ได้ไปเข้าใช้งานระบบ

การพิสูจน์ตัวตนแบบ​Time-synchronous authentication เป็นวิธีการที่สร้างรหัสผ่านโดยมีการกำหนดช่วงระยะเวลาการใช้งาน โดยปกติแล้วรหัสผ่านจะถูกเปลี่ยนทุกๆ 30​ วินาที การสร้างรหัสผ่านจะเป็นไปอย่างต่อเนื่อง เมื่อผู้ใช้ต้องการเข้าสู่ระบบก็ใส่รหัสผ่าน เพื่อเข้าสู่ระบบ ระบบจะทำการตรวจสอบเวลาและรหัสผ่านที่ผู้ใช้ใส่ลงไป กับ​ Server​ ว่ารหัสผ่านที่ใส่ตรงกับเวลาที่ Token สร้าง และมีอยู่ในเซิร์ฟเวอร์จริง จึงยินยอมให้ผู้ใช้เข้าสู่ระบบ

###### การพิสูจน์ตัวตนแบบอะซิงโครนัส หรือเรียกอีกอย่างหนึ่งว่า “challenge-response” ถูกพัฒนาขึ้น เป็นลำดับแรกๆ ของระบบการใช้ “รหัสผ่านซึ่งเปลี่ยนแปลงได้” ซึ่งถือได้ว่าเป็นการป้องกันการจู่โจมที่ปลอดภัยที่สุด เพราะเนื่องจากว่าเมื่อผู้ใช้ต้องการจะเข้าสู่ระบบ ผู้ใช้จะต้องทำการร้องของไปยัง​ Server​ จากนั้นจะได้รับ challenge string มาเพื่อให้ผู้ใช้ใส่ลงใน Token จากนั้น Token จะทำการคำนวณรหัสผ่านออกมาให้ผู้ใช้ ผู้ใช้จึงสามารถนำรหัสผ่านเพื่อเข้าสู่ระบบได้

+ การพิสูจน์ตัวตนโดยการเข้ารหัสโดยใช้กุญแจสาธารณะ (Public-key cryptography)

  ![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/989020b7-02d8-4585-87b7-a6abcb5ceaeb)

เป็นการแสดงความเป็นเจ้าของข้อมูล เพราะข้อความใดก็ตามที่สร้างโดย Private Key ของคนๆนั้น จะถอดได้โดยใช้ Public Key ของคนๆนั้นเท่านั้น ดังนั้นหากเรายืนยันได้ว่า Public Key ที่นำมาใช้ถอดรหัสเป็นของคนนั้นจริง และสามารถถอดรหัสได้ เราก็สามารถยืนยันได้ว่าข้อความนั้นมาจากคนๆนั้นจริง​ ซึ่งวิธีนี้จะแบ่ง Key​ ออกเป็น 2 ชนิด ที่ต้องใช้ควบคู่กันเสมอในการเข้ารหัสและถอดรหัสคือ

###### กุญแจสาธารณะ (public key) เป็นกุญแจที่เปิดเผยให้ชาวโลกรู้ได้
###### กุญแจส่วนตัว (private key) เป็นกุญแจที่เราเก็บไว้ใช้เองโดยไม่เปิดเผยให้คนอื่นรู้

+ การพิสูจน์ตัวตนโดยใช้การถาม-ตอบ (zero-knowledge proofs)

  ![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/c627d728-51c3-4407-b020-7980b5a26675)

เป็นวิธีการพิสูจน์ตัวตนโดยใช้การถาม-ตอบ​ถ้าให้เห็นภาพง่ายๆ​ ว่ามีการนำไปใช้อย่างไร​ เช่นตอนที่เราโทรหา​ Call​ Center ก่อนที่พนักงานจะให้ข้อมูลกับเราเขาก็จะข้อมูลเราก่อนเช่นชื่อ​-นามสกุล​ วันเดือนปีเกิดหรือเลขบัตรประชาชน​ เพื่อเป็นการพิสูจน์​ตัวตนว่าเป็นเราจริงๆ​

Source : https://www.cloudflare.com/learning/access-management/what-is-authentication/

Source : https://www.cisco.com/c/en/us/products/security/identity-services-engine/what-is-user-authentication-policy.html#~how-authentication-works

แหล่งข้อมูล : <a href="https://medium.com/@suttipongsrimangmat/%E0%B8%A1%E0%B8%B2%E0%B8%A7%E0%B9%88%E0%B8%B2%E0%B8%81%E0%B8%B1%E0%B8%99%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2%E0%B9%80%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%81%E0%B8%B2%E0%B8%A3-authentication-%E0%B9%83%E0%B8%99%E0%B8%A3%E0%B8%B9%E0%B8%9B%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B8%95%E0%B9%88%E0%B8%B2%E0%B8%87%E0%B9%86%E0%B8%81%E0%B8%B1%E0%B8%99%E0%B8%99%E0%B8%B0%E0%B8%84%E0%B8%A3%E0%B8%B1%E0%B8%9A-5875ef8f2c19
">medium </a>
แหล่งข้อมูล : https://monsterconnect.co.th/authentication-vs-authorization/
