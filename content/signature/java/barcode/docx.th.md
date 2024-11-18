



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:05
draft: false
lang: th
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "เพิ่มบาร์โค้ดในไฟล์ DOCX ด้วย Java"
head_description: "สร้างและแทรกบาร์โค้ดลงในเอกสาร DOCX ด้วย Java โดยใช้ GroupDocs.Signature ที่รองรับการผสมผสานลายเซ็นที่หลากหลายสำหรับหลายรูปแบบ."

############################# Header ############################
title: "สร้างบาร์โค้ดสำหรับ DOCX" 
description: "เพิ่มบาร์โค้ดในรูปแบบที่เป็นที่นิยม ณ จุดใดก็ได้ในเอกสารธุรกิจของคุณด้วย GroupDocs.Signature for Java โซลูชันของเราเสนอทางเลือกมากมายเพื่อปรับแต่งบาร์โค้ดลายเซ็น."
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
    title: "เกี่ยวกับ GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) เป็นโซลูชันการลงนามที่ทันสมัยที่รองรับประเภทลายเซ็นที่หลากหลาย คุณสามารถลงนามเอกสารด้วยข้อความ, รูปภาพ, บาร์โค้ด, ใบรับรองดิจิทัล, แสตมป์ และอื่น ๆ อีกกว่า 60 รูปแบบไฟล์ รวมถึง PDF, MS Office, รูปภาพ, ไฟล์ ZIP และรูปแบบธุรกิจยอดนิยมอื่น ๆ นอกจากนี้ ลายเซ็นในเอกสารที่เซ็นแล้วยังสามารถค้นหา, ตรวจสอบ, แก้ไข หรือ ลบได้ในทุกเวลา.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนการสร้างและเพิ่มบาร์โค้ดในไฟล์ DOCX"
    content: |
      [GroupDocs.Signature](/signature/java/) สามารถสร้างบาร์โค้ดในรูปแบบที่เป็นที่นิยมต่าง ๆ และวางไว้ในหน้า DOCX ด้วยการสนับสนุนประเภทบาร์โค้ดมากกว่า 60 ประเภท แอปพลิเคชัน Java สามารถเพิ่มความสามารถในการลงนามด้วยบาร์โค้ดได้อย่างง่ายดายโดยการรวมไลบรารีของเรา.
      
      1. จัดเตรียมไฟล์ DOCX หรือสตรีมที่ต้องการการประมวลผล.
      2. ส่งข้อความบาร์โค้ดไปยังอินสแตนซ์ BarcodeSignOptions.
      3. ปรับแต่งตัวเลือกบาร์โค้ด เช่น ตำแหน่ง, ขนาด, ฯลฯ.
      4. บันทึกไฟล์พร้อมกับบาร์โค้ดที่เพิ่มเข้ามาใหม่.
   
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
        // สร้างอินสแตนซ์ Signature ใหม่พร้อมกับเส้นทางเอกสาร
        Signature signature = new Signature("input.docx");

        // ใช้ BarcodeSignOptions เพื่อเพิ่มบาร์โค้ดลงในเอกสาร
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // ตั้งค่าประเภทบาร์โค้ดและคุณสมบัติอื่น ๆ
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // บันทึกไฟล์ที่ลงนาม
        signature.sign("output.docx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เสริมหรือปกป้องเนื้อหาเอกสารด้วยลายเซ็น"
  description: "ไลบรารี GroupDocs.Signature for Java ถูกออกแบบมาเพื่อการลงนามและการประมวลผลไฟล์รูปแบบยอดนิยมอย่างรวดเร็ว เพิ่ม, แก้ไข, ตรวจสอบ, หรือ ลบลายเซ็นประเภทต่าง ๆ ได้อย่างมีประสิทธิภาพ."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "คุณสมบัติต่าง ๆ ของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "การลงนามเอกสาร"
      content: "ลงนามในหน้าใด ๆ ของเอกสารที่รองรับด้วยข้อความ, รูปภาพ, บาร์โค้ด, โค้ด QR หรือ แสตมป์ เพิ่มข้อมูลเมตาดาต้าที่ซ่อนอยู่เช่น EXIF ในรูปภาพหรือปกป้องเนื้อหาเอกสารจากการเปลี่ยนแปลงที่ไม่ได้รับอนุญาตโดยใช้ใบรับรองดิจิทัล."

    # feature loop
    - title: "การค้นหาและตรวจสอบลายเซ็น"
      content: "คุณสามารถทำอะไรได้มากกว่าการตรวจสอบเอกสารที่เซ็นแล้ว เราเสนอการตรวจสอบลายเซ็นเพื่อให้แน่ใจว่าทุกอย่างเป็นไปตามที่คาดหวัง นอกจากนี้คุณยังสามารถดึงรายการลายเซ็นทั้งหมดในเอกสารได้ผ่านการค้นหา."

    # feature loop
    - title: "แก้ไขลายเซ็น"
      content: "ลายเซ็นที่เพิ่มเข้ามาส่วนใหญ่สามารถแก้ไขได้ แก้ไขข้อความ, ปรับตำแหน่ง หรือ เปลี่ยนสีได้อย่างง่ายดาย."

    # feature loop
    - title: "ลบลายเซ็น"
      content: "โซลูชันของเราให้การสนับสนุนการดำเนินการ CRUD เต็มรูปแบบสำหรับลายเซ็น หลายประเภทของลายเซ็นสามารถลบออกจากเอกสารได้ตามความจำเป็น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "วิธีสร้างลายเซ็นบาร์โค้ด"
      content: |
        ตัวอย่างนี้แสดงให้เห็นว่าคุณจะวางบาร์โค้ดที่ปรับแต่งได้ในหน้าเอกสาร DOCX ได้อย่างไร.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // จัดเตรียมเอกสารที่ต้องการลงนาม
          Signature signature = new Signature("input.docx");

          // สร้างตัวเลือกการลงนามด้วยข้อความที่ต้องการ
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // ตั้งค่าตำแหน่งสัมพัทธ์ของบาร์โค้ดบนหน้า
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // ตั้งค่าช่องว่างบาร์โค้ดจากขอบหน้า
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // กำหนดสีของบาร์
          signOptions.setForeColor(Color.RED);

          // กำหนดรูปแบบฟอนต์ข้อความ
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // ระบุตำแหน่งข้อความ
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // ลงนามและบันทึกเอกสาร
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
            link: "/examples/signature/formats/signature_barcode.docx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

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
    title: "ค้นพบความสามารถหลักของเรา"
    exclude: "barcode"
    description: "เรานำเสนอความหลากหลายที่กว้างขวางของลายเซ็นและฟังก์ชันที่รองรับ."
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
    title: "ลงนามในเอกสารในรูปแบบอื่น ๆ"
    exclude: "DOCX"
    description: "มากกว่า 60 รูปแบบสามารถลงนามได้โดยใช้ API Java ของเรา ใช้ลายเซ็นที่หลากหลายไปยังหน้าใดก็ตามหรือภายในเอกสาร."
    items: 
          
        # format loop 1
        - name: "เพิ่มบาร์โค้ดใน PDF"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "เพิ่มบาร์โค้ดใน DOCX"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "เพิ่มบาร์โค้ดใน JPEG"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "เพิ่มบาร์โค้ดใน PPTX"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "เพิ่มบาร์โค้ดใน XLSX"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---