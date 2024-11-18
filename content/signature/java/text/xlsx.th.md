



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: th
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "สร้างลายเซ็นข้อความ XLSX ด้วย Java"
head_description: "ใช้ API Java เพื่อแทรกลายเซ็นข้อความลงในไฟล์ XLSX ประมวลผลรูปแบบเอกสารยอดนิยมเช่น PDF, Word, Excel, การนำเสนอ, รูปภาพ และ ZIP อย่างราบรื่น."

############################# Header ############################
title: "สร้างลายเซ็นข้อความสำหรับ XLSX" 
description: "เพิ่มลายเซ็นข้อความที่กำหนดเองลงในเอกสารธุรกิจของคุณด้วย GroupDocs.Signature for Java ปรับปรุงการจัดการเวิร์กโฟลว์ในองค์กรด้วยตัวเลือกการปรับแต่งลายเซ็น."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "เริ่มใช้งานฟรี"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับโซลูชัน GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) มีลายเซ็นข้อความที่ยืดหยุ่นและสามารถปรับแต่งได้เพื่อนำความสะดวกมาให้กับการจัดการเอกสารของคุณ กำหนดเนื้อหาและการออกแบบของลายเซ็นข้อความและใช้มันบนทุกหน้า เพื่อปรับปรุงการเวิร์กโฟลว์เอกสารขององค์กรของคุณ.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการเพิ่มลายเซ็นข้อความใน XLSX โดยใช้ Java"
    content: |
      [GroupDocs.Signature](/signature/java/) สามารถรวมเข้ากับแอปพลิเคชัน Java เพื่อเพิ่มลายเซ็นข้อความในเอกสาร XLSX นักพัฒนาสามารถปรับปรุงฟังก์ชันของผลิตภัณฑ์ของตนได้อย่างรวดเร็วด้วยโซลูชันของเรา.
      
      1. ใช้เอกสาร XLSX เป็นพารามิเตอร์สำหรับตัวสร้างคลาส Signature.
      2. สร้าง TextSignOptions ด้วยข้อความที่เหมาะสม.
      3. กำหนดตัวเลือกด้านสรีรศาสตร์สำหรับลายเซ็น.
      4. เพิ่มลายเซ็นข้อความไปยังหน้าใดก็ได้ของเอกสาร.
   
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
        // ส่งเส้นทางเอกสารไปยังตัวสร้าง Signature
        Signature signature = new Signature("input.xlsx");

        // สร้าง TextSignOptions ด้วยข้อความลายเซ็น
        TextSignOptions options = new TextSignOptions("Approved");
        
        // ตั้งค่าสีและคุณลักษณะของฟอนต์
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // เพิ่มลายเซ็นข้อความไปยังเอกสาร
        SignResult result = signature.sign("output.xlsx", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "บริหารจัดการลายเซ็นข้อความในเอกสาร"
  description: "ด้วย GroupDocs.Signature for Java คุณสามารถปรับปรุงเวิร์กโฟลว์ของเอกสารในบริษัทของคุณโดยการเพิ่มลายเซ็นข้อความในรูปแบบไฟล์ยอดนิยม ปรับแต่งรูปลักษณ์และเนื้อหาของลายเซ็นได้อย่างง่ายดาย."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "ลายเซ็นเอกสาร"
      content: "สามารถใช้ลายเซ็นข้อความ, รูปภาพ, บาร์โค้ด, รหัส QR หรือประทับตราในหน้าใดก็ได้ของเอกสารที่รองรับ ใช้ข้อมูลเมตาเพื่อฝังเนื้อหาที่ซ่อนอยู่และรักษาความปลอดภัยเอกสารของคุณด้วยใบรับรองดิจิทัล."

    # feature loop
    - title: "การค้นหาและการตรวจสอบลายเซ็น"
      content: "ตรวจสอบความสมบูรณ์ของเอกสารที่ลงนามด้วยเครื่องมือการตรวจสอบลายเซ็นของเรา นอกจากนี้ยังสามารถดึงและค้นหาทุกลายเซ็นที่ฝังอยู่ในเอกสาร."

    # feature loop
    - title: "ปรับเปลี่ยนหรือลบลายเซ็น"
      content: "ปรับเปลี่ยนเนื้อหา ตำแหน่ง และรูปลักษณ์ของลายเซ็นที่เพิ่มเข้ามาก่อนหน้านี้ หรือสามารถลบออกจากเอกสารได้ทั้งหมด."

    # feature loop
    - title: "ลายเซ็นข้อความที่เป็นธรรมชาติ"
      content: "เพิ่มลายเซ็นข้อความเฉพาะเอกสาร เช่น สติ๊กเกอร์ใน PDF หรือลายน้ำในเอกสาร Word เพื่อการปรับแต่งที่เพิ่มขึ้น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ทำเครื่องหมายเอกสารด้วยลายเซ็นข้อความ"
      content: |
        เรียนรู้วิธีแนบข้อมูลข้อความลงในเอกสารธุรกิจเพื่อปรับปรุงกระบวนการทางธุรกิจ.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // เลือกเอกสารที่ต้องการลงนาม
          Signature signature = new Signature("input.xlsx");

          // สร้างตัวเลือกข้อความด้วยข้อความที่ต้องการ
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // ระบุขนาดและตำแหน่งของลายเซ็นบนหน้า
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // ลายเซ็นรองรับการตั้งค่าขอบจากมุมของหน้า
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // สามารถปรับแต่งสีข้อความและรูปแบบฟอนต์ได้
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // ลายเซ็นข้อความสามารถมีกรอบได้
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // การปรับแต่งพื้นหลังยังมีให้บริการ
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // ข้อความสามารถบันทึกเป็นภาพเพื่อความเข้ากันได้
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // บันทึกเอกสารพร้อมลายเซ็นข้อความที่เพิ่มเข้ามา
          SignResult result = signature.sign("output.xlsx", options);
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
            link: "/examples/signature/formats/signature_text.xlsx"
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
    title: "คุณสมบัติหลักและตัวเลือกสำหรับลายเซ็น"
    exclude: "text"
    description: "โซลูชันของเราให้การสนับสนุนการดำเนินการ CRUD เต็มรูปแบบและเพิ่มเติมสำหรับลายเซ็นประเภทต่าง ๆ จำนวนเจ็ดประเภท."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "เพิ่มลายเซ็นข้อความในรูปแบบไฟล์ต่าง ๆ"
    exclude: "XLSX"
    description: "ใช้ API Java เพื่อแทรกลายเซ็นข้อความลงในเอกสาร Office โดยมั่นใจได้ว่าคุณมีการควบคุมเนื้อหาในทุกขั้นตอนของวงจรชีวิตเอกสาร."
    items: 
          
        # format loop 1
        - name: "ลายเซ็นข้อความ PDF"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ลายเซ็นข้อความ DOCX"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ลายเซ็นข้อความ JPEG"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "ลายเซ็นข้อความ PPTX"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "ลายเซ็นข้อความ XLSX"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---