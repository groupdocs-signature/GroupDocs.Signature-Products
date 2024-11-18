



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: th
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "เพิ่มตราประทับลงใน PDF โดยใช้ Java"
head_description: "ใช้ GroupDocs.Signature และ Java เพื่อสร้างตราประทับที่กำหนดเองและวางลงในเอกสาร PDF ทุกหน้า."

############################# Header ############################
title: "เพิ่มตราประทับที่กำหนดเองลงใน PDF" 
description: "ออกแบบและใช้ตราประทับกลมหรือสี่เหลี่ยมในทุกส่วนของเอกสารของคุณโดยใช้ GroupDocs.Signature for Java โซลูชันของเรามีตัวเลือกการปรับแต่งที่หลากหลายเพื่อตอบสนองทุกความต้องการทางธุรกิจของคุณ."
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
       [GroupDocs.Signature for Java](/signature/java/) เป็นเครื่องมือที่ทรงพลังที่ช่วยให้คุณเพิ่มลายเซ็นตราประทับที่หลากหลายลงในเอกสาร มันรองรับรูปแบบไฟล์มากกว่า 60 รูปแบบ รวมถึง PDF, Word, Excel, รูปภาพ และไฟล์ ZIP คุณสามารถใช้ลายเซ็นข้อความ รูปภาพ บาร์โค้ด เมตาดาทา ใบรับรองดิจิตอล และลายเซ็นตราประทับ นอกจากนี้ยังสามารถค้นหา ตรวจสอบ แก้ไข และลบลายเซ็นได้.

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการเพิ่มตราประทับลงใน PDF โดยใช้ Java"
    content: |
      [GroupDocs.Signature](/signature/java/) มีคอนสตรัคเตอร์ตราประทับที่สามารถเป็นประโยชน์มากสำหรับแอปพลิเคชัน Java ใช้เพื่อสร้างตราประทับที่ปรับแต่งได้ดีสำหรับหน้าเอกสารของคุณ.
      
      1. จัดเตรียมเอกสาร PDF ที่ต้องการตราประทับ.
      2. ใช้ StampSignOptions เพื่อกำหนดพารามิเตอร์ที่จำเป็นทั้งหมด.
      3. เพิ่มจำนวนบรรทัดตามที่ต้องการ.
      4. นำตราประทับไปใช้และบันทึกเอกสาร.
   
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
        // ใช้เส้นทางเอกสารร่วมกับอ็อบเจ็กต์ Signature
        Signature signature = new Signature("input.pdf");

        // สร้างอ็อบเจ็กต์ StampSignOptions ด้วยข้อความลายเซ็นที่ต้องการ
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // เพิ่มหนึ่งหรือหลายบรรทัดตราประทับ
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // บันทึกเอกสารที่มีตราประทับ
        SignResult result = signature.sign("output.pdf", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "ปกป้องเนื้อหาเอกสารของคุณด้วยลายเซ็น"
  description: "ห้องสมุด GroupDocs.Signature for Java ถูกออกแบบมาเพื่อใช้ในการลงลายเซ็นและจัดการลายเซ็นทั่วรูปแบบไฟล์ยอดนิยม เพิ่ม แก้ไข ตรวจสอบ หรือ ลบตราประทับและลายเซ็นประเภทอื่นได้โดยง่าย."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "ลายเซ็นตราประทับด้วย GroupDocs.Signature"
  features:
    # feature loop
    - title: "ลงลายเซ็นในเอกสารของคุณ"
      content: "ใช้ลายเซ็นที่ปรับแต่งได้ในทุกส่วนของเอกสารของคุณ เลือกจากลายเซ็นประเภทต่างๆ เช่น ข้อความ รูปภาพ บาร์โค้ด รหัส QR และตราประทับ นอกจากนี้ยังสามารถเพิ่มหรือแก้ไขเมตาดาทาที่ซ่อนอยู่เพื่อเพิ่มความปลอดภัยให้กับเอกสาร."

    # feature loop
    - title: "ค้นหาและตรวจสอบลายเซ็น"
      content: "เมื่อเอกสารได้รับการลงลายเซ็นแล้ว ใช้เครื่องมือการตรวจสอบของเราเพื่อให้แน่ใจว่าข้อมูลลายเซ็นนั้นถูกต้อง ค้นหาและดึงคืนรายชื่อทั้งหมดของลายเซ็นเพื่อการประมวลผลเพิ่มเติม."

    # feature loop
    - title: "ปรับปรุงลายเซ็นตามต้องการ"
      content: "แก้ไขลายเซ็นที่หลากหลายที่ถูกใช้ในเอกสารได้โดยไม่ยุ่งยาก ปรับปรุงคุณสมบัติเช่น ขนาด สี ตำแหน่ง เนื้อหา และอื่น ๆ."

    # feature loop
    - title: "ลบลายเซ็น"
      content: "ต้องการลบลายเซ็นออกจากเอกสารหรือไม่? API ของเราสนับสนุนการลบลายเซ็นอย่างเต็มที่ ทำให้การจัดการเอกสารของคุณมีประสิทธิภาพ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "เพิ่มตราประทับที่กำหนดเองลงในเอกสารโดยใช้ลายเซ็นพิเศษ"
      content: |
        เรียนรู้วิธีการสร้างและเพิ่มตราประทับที่กำหนดเองซึ่งมีข้อมูลข้อความสำคัญลงในเอกสารของคุณ.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // จัดเตรียมเอกสารที่จะตราประทับ
          Signature signature = new Signature("input.pdf");

          // สร้างอ็อบเจ็กต์ตัวเลือกตราประทับ
          StampSignOptions options = new StampSignOptions();

          // กำหนดขนาดและตำแหน่งบนหน้า
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // เพิ่มบรรทัดกลมภายนอกหนึ่งหรือหลายบรรทัดพร้อมกับข้อความ
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // เพิ่มบรรทัดสี่เหลี่ยมภายในหนึ่งหรือหลายบรรทัด
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // บันทึกเอกสารที่มีตราประทับ
          SignResult result = signature.sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "สำรวจฟีเจอร์หลักของเรา"
    exclude: "stamp"
    description: "ใช้ตัวเลือกที่หลากหลายสำหรับการเพิ่ม จัดการ และลบลายเซ็น."
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "เพิ่มตราประทับในรูปแบบไฟล์หลายประเภท"
    exclude: "PDF"
    description: "API GroupDocs.Signature สนับสนุนการสร้างตราประทับในเอกสารกว่า 60 รูปแบบ วางตราประทับในทุกหน้า หรือพื้นที่ใดก็ได้เพื่อปรับปรุงการจัดการและการปรับแต่งเอกสาร."
    items: 
          
        # format loop 1
        - name: "ประทับตรา PDF"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ประทับตรา DOCX"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ประทับตรา JPEG"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "ภาพ JPEG"
          
        # format loop 4
        - name: "ประทับตรา PPTX"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 5
        - name: "ประทับตรา XLSX"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---