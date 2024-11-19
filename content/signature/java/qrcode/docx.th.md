



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: th
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "สร้าง QR code สำหรับ DOCX ด้วย Java"
head_description: "API ของ GroupDocs.Signature ช่วยให้สามารถสร้าง QR code สำหรับไฟล์ DOCX ได้ สร้าง QR code จากเนื้อหาของคุณและวางลงบนหน้าใดก็ได้."

############################# Header ############################
title: "สร้าง QR codes สำหรับ DOCX" 
description: "สร้างบาร์โค้ด 2 มิติที่มีข้อความและข้อมูลเชิงตัวเลขได้ และวางบนหน้าใดก็ได้ของเอกสารหลายประเภทโดยใช้ GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "เรียนรู้เพิ่มเติมเกี่ยวกับ GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) มีฟีเจอร์ที่หลากหลายในการสร้างและฝังลายเซ็นประเภทต่างๆ ในเอกสารที่สำคัญทั้งหมด รองรับ PDF, เอกสาร Word, สเปรดชีต Excel, งานนำเสนอ PowerPoint และภาพถ่าย เพิ่มความสามารถให้กับเอกสารของคุณด้วย ลายเซ็น Text, Image, Barcode, QR Code, Metadata, Digital และ Stamp.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการสร้างและวาง QR code ที่ตำแหน่งใดก็ได้ใน DOCX"
    content: |
      [GroupDocs.Signature](/signature/java/) สามารถสร้าง QR code ในหลายฟอร์แมตที่เป็นที่นิยมและวางลงบนหน้า DOCX รองรับ QR code มากกว่า 10 ประเภทและสามารถรวมเข้ากับแอปพลิเคชัน Java ได้อย่างรวดเร็ว ใช้ผลิตภัณฑ์ของเราเพื่อทำการลงนามเอกสารด้วย QR codes ที่สร้างขึ้น.
      
      1. รับไฟล์หรือสตรีม DOCX ที่ต้องการลงนามด้วย QR code.
      2. ระบุข้อความสำหรับ QrCodeSignOptions.
      3. ปรับแต่งตัวเลือกทางสายตา เช่น สี ตำแหน่ง ขนาด เป็นต้น.
      4. บันทึกไฟล์ที่มี QR code.
   
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
        // ส่งเอกสารไปยังอินสแตนซ์ใหม่ของ Signature
        Signature signature = new Signature("input.docx");

        // ใช้ QrCodeSignOptions เพื่อเพิ่ม QR code ลงในเอกสาร
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // ระบุประเภทลายเซ็นและตำแหน่งบนหน้า
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // บันทึกไฟล์ที่มี QR code เพิ่มเติม
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มลายเซ็นให้กับเอกสารของคุณ"
  description: "API ของ GroupDocs.Signature for Java รองรับการลงทะเบียนในฟอร์แมตไฟล์ยอดนิยมทั้งหมด สร้าง แก้ไข ค้นหา ตรวจสอบ และลบลายเซ็นประเภทต่างๆ."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "ลงนามเอกสาร"
      content: "GroupDocs.Signature รองรับการลงนามด้วยลายเซ็น Text, Image, Barcode, QR Code และ Stamp วางลายเซ็นในหน้าใดก็ได้ของฟอร์แมตเอกสารที่รองรับ จัดการข้อมูลเมตาของเอกสารด้วยลายเซ็นข้อมูลเมตา และป้องกันเนื้อหาจากการเปลี่ยนแปลงที่ไม่ได้รับอนุญาตโดยใช้ใบรับรองดิจิทัล."

    # feature loop
    - title: "ค้นหาและการตรวจสอบ"
      content: "รับประกันว่าลายเซ็นทั้งหมดในเอกสารนั้นถูกต้องตามขั้นตอนการตรวจสอบ ดึงข้อมูลลายเซ็นทั้งหมดในเอกสารด้วยฟีเจอร์ค้นหาที่สร้างไว้."

    # feature loop
    - title: "แก้ไขลายเซ็น"
      content: "ดำเนินการแก้ไขคุณสมบัติลายเซ็นได้ง่ายหลังจากที่ทำการลงชื่อ ปรับแต่งเนื้อหา ตำแหน่ง สี ขนาด และคุณสมบัติอื่นๆ ตามที่ต้องการ."

    # feature loop
    - title: "ลบลายเซ็น"
      content: "ลบลายเซ็นที่ไม่ต้องการได้อย่างง่ายดาย ลายเซ็นประเภทต่างๆ รวมถึงใบรับรองดิจิทัล สามารถถูกลบออกจากเอกสารได้ทางโปรแกรม."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีการปรับแต่ง QR code ที่สร้างขึ้น"
      content: |
        ใช้ตัวอย่างนี้เพื่อเรียนรู้วิธีวาง QR code ใหม่ลงในหน้า DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // รับเอกสารที่ต้องการลงนามและส่งไปยัง Signature
          Signature signature = new Signature("input.docx");

          // ใช้ตัวเลือก QR code ในการให้ข้อความพร้อมข้อมูลที่ต้องการ
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // ตั้งค่าตำแหน่งสัมพัทธ์ของ QR code บนหน้า
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // ตั้งค่าขอบของลายเซ็น
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // ระบุสีของ QR code
          signOptions.setForeColor(Color.RED);

          // กำหนดตัวเลือกฟอนต์สำหรับข้อความ
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // ปรับแต่งสีพื้นหลังและแปรงของ QR code
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // เพิ่ม QR code ลงในเอกสาร
          SignResult signResult = signature.sign("output.docx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.docx"
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
    title: "ชมข้อเสนอหลักของเรา"
    exclude: "qrcode"
    description: "เรามีการเลือกฟีเจอร์การลงนามและการปฏิบัติการขั้นสูงที่หลากหลาย"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "สร้าง QR codes สำหรับฟอร์แมตไฟล์เพิ่มเติม"
    exclude: "DOCX"
    description: "เพิ่ม QR codes ลงในฟอร์แมตไฟล์ยอดนิยมทั้งหมดด้วย API ของ Java เพิ่มข้อมูลบาร์โค้ด 2 มิติสำหรับการสแกนและการประมวลผลอย่างรวดเร็ว."
    items: 
          
        # format loop 1
        - name: "QR-Code สำหรับ PDF"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "QR-Code สำหรับ DOCX"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "QR-Code สำหรับ JPEG"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "QR-Code สำหรับ PPTX"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "QR-Code สำหรับ XLSX"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---