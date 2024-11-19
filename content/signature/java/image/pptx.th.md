



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:09
draft: false
lang: th
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "การเพิ่มลายเซ็นรูปภาพไปยังไฟล์ PPTX ด้วย Java"
head_description: "ใส่ลายเซ็นรูปภาพลงในไฟล์ PPTX สำหรับ Java โดยใช้โค้ดเพียงไม่กี่บรรทัด ใช้ API GroupDocs.Signature for Java เพื่อเพิ่มรูปภาพ."

############################# Header ############################
title: "ลงนามไฟล์ PPTX ด้วยลายเซ็นรูปภาพ" 
description: "ใช้ GroupDocs.Signature for Java ในการแทรกรูปภาพลงในรูปแบบเอกสารสำนักงานต่างๆ รวมถึง PDF, Word, Excel และไฟล์รูปภาพ รูปภาพที่มีลายเซ็นของหัวหน้าสามารถเพิ่มความน่าเชื่อถือได้อย่างน่าประทับใจ!"
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "ค้นพบ GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) มีความสามารถในการเพิ่มลายเซ็นรูปภาพในทุกหน้าและตำแหน่งภายในเอกสารธุรกิจ ปรับปรุงกระบวนการทำงานของคุณโดยการเพิ่มรูปภาพใน PDF, เอกสาร Word, สเปรดชีต Excel, งานนำเสนอ PowerPoint และรูปแบบภาพที่เป็นที่นิยม.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการเพิ่มรูปภาพในตำแหน่งใดก็ได้ของไฟล์ PPTX ผ่าน Java"
    content: |
      [GroupDocs.Signature](/signature/java/) ช่วยเพิ่มความสามารถให้กับแอปพลิเคชัน Java ในการเพิ่มลายเซ็นไปยังทุกหน้าในเอกสาร PPTX ได้อย่างแม่นยำ ปรับปรุงฟังก์ชันการทำงานของผลิตภัณฑ์ของคุณด้วยการรวมไลบรารีของเรา.
      
      1. สร้างอินสแตนซ์ของ Signature พร้อมกับเอกสาร PPTX.
      2. ใช้ ImageSignOptions เพื่อกำหนดรูปภาพลายเซ็น.
      3. วางรูปภาพในตำแหน่งใดก็ได้ของหน้าใดก็ได้.
      4. บันทึกเอกสารที่ลงนามไปยังตำแหน่งใหม่.
   
    code:
      platform: "java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "ตัวอย่างลายเซ็น"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // สร้างอินสแตนซ์ของ Signature พร้อมกับเส้นทางเอกสาร
        Signature signature = new Signature("input.pptx");

        // สร้าง ImageSignOptions โดยใช้รูปภาพสำหรับลายเซ็น
        ImageSignOptions options = new ImageSignOptions("company_logo.jpg");

        // วางรูปภาพในมุมซ้ายบนของทุกหน้า
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);

        // บันทึกเอกสารที่ลงนาม
        SignResult result = signature.sign("output.pptx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "โซลูชันการลงนามเอกสารที่ครบถ้วน"
  description: "API ของเรารองรับคุณสมบัติการลงนามที่หลากหลาย ทำให้คุณสามารถเพิ่ม แก้ไข ลบ ค้นหา และตรวจสอบประเภทลายเซ็นหลายประเภท รวมถึงลายเซ็นรูปภาพ."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "การลงนามด้วยรูปภาพ"
  features:
    # feature loop
    - title: "แทรกรูปภาพลงในเอกสารสำนักงาน"
      content: "วางลายเซ็นรูปภาพในตำแหน่งใดก็ได้ในเอกสารได้อย่างไม่ยุ่งยาก เสริมเนื้อหาของคุณด้วยข้อความ รูปภาพ บาร์โค้ด ข้อมูลเมตา และใบรับรองดิจิทัล."

    # feature loop
    - title: "ค้นหาและตรวจสอบลายเซ็น"
      content: "ตรวจสอบความถูกต้องของลายเซ็นในเอกสารที่ลงนามได้อย่างง่ายดาย รับรายการลายเซ็นทั้งหมดภายในเอกสารและตรวจสอบข้อมูลรายละเอียดเกี่ยวกับแต่ละลายเซ็น."

    # feature loop
    - title: "แก้ไขลายเซ็น"
      content: "อัปเดตเนื้อหา ลักษณะ ขนาด หรือที่ตั้งของลายเซ็นที่ได้เพิ่มไว้ในเอกสารก่อนหน้านี้ API ของเราช่วยให้การปรับเปลี่ยนลายเซ็นเป็นเรื่องง่ายและมีประสิทธิภาพ."

    # feature loop
    - title: "ลบลายเซ็นที่ไม่จำเป็น"
      content: "API ของเรารองรับการทำงาน CRUD เต็มรูปแบบสำหรับลายเซ็นส่วนใหญ่ คุณสามารถลบลายเซ็นจากเอกสารที่รองรับได้เกือบทั้งหมดเมื่อจำเป็น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นรูปภาพ"
      content: |
        เรียนรู้วิธีการเพิ่มรูปภาพลงในเอกสารธุรกิจเพื่อให้ข้อมูลเพิ่มเติม.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เลือกเอกสารที่จะลงนาม
          Signature signature = new Signature("input.pptx");

          // สร้างตัวเลือกของรูปภาพด้วยเส้นทางที่ไปยังรูปภาพ
          ImageSignOptions options = new ImageSignOptions("manager_signature.jpg");

          // ตั้งค่าขนาดของลายเซ็นรูปภาพ
          options.setWidth(100);
          options.setHeight(100);

          // วางรูปภาพในมุมล่างขวา
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);

          // ใช้พื้นที่ว่างจากมุมหน้าเพจถ้าจำเป็น
          Padding padding = new Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // เพิ่มกรอบที่กำหนดเองให้กับรูปภาพหากต้องการ
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // หมุนลายเซ็นเพื่อตรงกับแนวที่ดีกว่า
          options.setRotationAngle(45);

          // บันทึกเอกสารที่อัปเดตไปยังตำแหน่งใดก็ได้
          SignResult result = signature.sign("output.pptx", options);

          ```
        platform: "java"
        copy_title: "คัดลอก"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/signature/formats/signature_image.pptx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นใช้งานหรือยัง?"
  description: "ลองฟีเจอร์ของ GroupDocs.Signature ฟรี หรือขอรับใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "มาดูคุณสมบัติหลักของเรา"
    exclude: "image"
    description: "เรายินดีที่จะแนะนำเครื่องมือและการทำงานของลายเซ็นที่หลากหลาย."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "เพิ่มรูปภาพในรูปแบบไฟล์อื่นๆ"
    exclude: "PPTX"
    description: "ด้วย API Java คุณสามารถแทรกรูปแบบรูปภาพที่รองรับลงในเอกสารต่างๆ ได้อย่างง่ายดาย ปรับขนาด เลือกตำแหน่ง และเพิ่มลายเซ็นรูปภาพในเอกสารของคุณ."
    items: 
          
        # format loop 1
        - name: "ลงชื่อ PDF ด้วยภาพ"
          format: "PDF"
          link: "/signature/java/image/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ลงชื่อ DOCX ด้วยภาพ"
          format: "DOCX"
          link: "/signature/java/image/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ลงชื่อ JPEG ด้วยภาพ"
          format: "JPEG"
          link: "/signature/java/image/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "ลงชื่อ PPTX ด้วยภาพ"
          format: "PPTX"
          link: "/signature/java/image/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "ลงชื่อ XLSX ด้วยภาพ"
          format: "XLSX"
          link: "/signature/java/image/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---