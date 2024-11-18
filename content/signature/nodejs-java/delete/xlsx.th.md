



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:20
draft: false
lang: th
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ลบลายเซ็นจาก XLSX ผ่าน JavaScript"
head_description: "การลบลายเซ็นดิจิทัล, บาร์โค้ด, ข้อความ, รูปภาพ, ข้อมูลเมตา จากเอกสาร XLSX ที่เซ็นแล้วสามารถทำได้ด้วย GroupDocs.Signature for Node.js via Java."

############################# Header ############################
title: "ลบลายเซ็นที่วางใน XLSX ได้อย่างไม่มีข้อติดขัด" 
description: "โซลูชันของเราไม่เพียงแค่เซ็นเอกสาร แต่ยังเสนอคุณสมบัติที่แข็งแกร่งใน GroupDocs.Signature for Node.js via Java เพื่อค้นหาและลบลายเซ็นหลากหลายประเภท."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรีของคุณ"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "ค้นพบ GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) เป็นห้องสมุดการเซ็นดิจิทัลที่มีระดับองค์กร ถูกออกแบบมาเพื่อรองรับลายเซ็นประเภทต่าง ๆ รวมถึงข้อความ, รูปภาพ, บาร์โค้ด, ใบรับรองดิจิทัล, และตราประทับ ด้วยความเข้ากันได้กับเอกสารมากกว่า 60 รูปแบบ—เช่น PDFs, ไฟล์ MS Office, รูปภาพ, ZIP archives, และรูปแบบธุรกิจสำคัญอื่น ๆ—เครื่องมือนี้จึงเสนอความยืดหยุ่นที่ไม่มีใครเทียบได้ในกระบวนการเอกสารอิเล็กทรอนิกส์ แพลตฟอร์มนี้ไม่เพียงแค่ช่วยในการฝังลายเซ็นอย่างราบรื่น แต่ยังมอบความสามารถในการค้นหา, ตรวจสอบ, อัปเดต, และลบลายเซ็น เพื่อให้แน่ใจว่ามีการจัดการวงจรชีวิตของกระบวนการเซ็นดิจิทัลในสภาพแวดล้อมขององค์กรอย่างสมบูรณ์.

############################# Steps ############################
steps:
    enable: true
    title: "แนวทางการลบลายเซ็นดิจิทัลจาก XLSX โดยใช้ JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) ช่วยให้นักพัฒนา Node.js via Java สามารถลบลายเซ็นอิเล็กทรอนิกส์ในไฟล์ XLSX ได้อย่างมีประสิทธิภาพ โดยการปฏิบัติตามขั้นตอนที่เรียบง่าย.
      
      1. ระบุเส้นทางไฟล์ XLSX ให้กับอินสแตนซ์ของคลาส Signature.
      2. ใช้วิธีการค้นหาเพื่อระบุลายเซ็นทั้งหมดในเอกสาร.
      3. ลบลายเซ็นที่ระบุหนึ่งหรือมากกว่า.
      4. ตรวจสอบผลลัพธ์ของการประมวลผลเอกสาร.
   
    code:
      platform: "nodejs-java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "ตัวอย่างลายเซ็น"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // ส่งเอกสารที่มีลายเซ็นไปยังอินสแตนซ์ของ Signature
        const signature = new signatureLib.Signature('input.xlsx');

        // ลบลายเซ็นบาร์โค้ดทั้งหมด
        const options = new signatureLib.DigitalSearchOptions();
        const signatures = signature.search(signatureLib.DigitalSignature.class, options);

        // ลบลายเซ็นดิจิทัลที่ตรวจพบแรก
        if(signatures.size() > 0)
        {
            const digitalSignature = signatures[0];
            const result = signature.delete('output.xlsx', digitalSignature);

            // จัดการผลลัพธ์ของการลบ
            if(result)
            {
                console.log(`\n XLSX digital signature deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เพิ่มความปลอดภัยของเอกสารด้วยเครื่องมือเซ็นชื่อ"
  description: "GroupDocs.Signature for Node.js via Java ถูกสร้างขึ้นมาเพื่อทำให้การเซ็นและการจัดการรูปแบบไฟล์ธุรกิจเป็นไปอย่างราบรื่น ช่วยให้คุณสามารถเพิ่ม, แก้ไข, ยืนยัน, หรือทำการลบลายเซ็นได้อย่างแม่นยำ."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "สำรวจความสามารถที่ครอบคลุมของ GroupDocs.Signature"
  features:
    # feature loop
    - title: "การเซ็นเอกสาร"
      content: "เพิ่มลายเซ็นประเภทข้อความ, รูปภาพ, บาร์โค้ด, QR code, หรือตราประทับไปยังหน้าใดก็ได้ของเอกสารที่รองรับได้อย่างราบรื่น ใช้ข้อมูลเมตาที่ซ่อนอยู่เช่น EXIF ในรูปภาพ หรือรักษาความถูกต้องของเอกสารด้วยใบรับรองดิจิทัลเพื่อป้องกันการเปลี่ยนแปลงที่ไม่ได้รับอนุญาต."

    # feature loop
    - title: "การค้นหาและตรวจสอบลายเซ็น"
      content: "เครื่องมือของเราเปิดโอกาสให้ตรวจสอบลายเซ็นในเอกสารอย่างละเอียด เพื่อให้แน่ใจในความถูกต้องของลายเซ็น ทำการค้นหาอย่างกว้างขวางเพื่อดึงลายเซ็นทั้งหมดในเอกสารของคุณ ช่วยเพิ่มการควบคุมเอกสาร."

    # feature loop
    - title: "แก้ไขลายเซ็นที่มีอยู่"
      content: "ปรับเปลี่ยนลายเซ็นที่เพิ่มเข้ามาก่อนหน้านี้ได้อย่างง่ายดาย โดยการปรับข้อความ, เปลี่ยนตำแหน่ง, หรือเปลี่ยนสีเพื่อตอบสนองความต้องการเฉพาะของคุณ."

    # feature loop
    - title: "ลบลายเซ็นที่ไม่ต้องการ"
      content: "ด้วยความสามารถในการจัดการ CRUD อย่างเต็มรูปแบบ โซลูชันของเราช่วยให้สามารถลบลายเซ็นหลากหลายประเภทจากเอกสารได้อย่างมีประสิทธิภาพ เพื่อให้ความยืดหยุ่นและการควบคุม."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ลบลายเซ็นบาร์โค้ดทั้งหมด"
      content: |
        เรียนรู้ขั้นตอนในการกำจัดลายเซ็นบาร์โค้ดทั้งหมดที่ฝังอยู่ในเอกสาร.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // ระบุเอกสารที่มีลายเซ็นบาร์โค้ด
          const signature = new signatureLib.Signature('input.xlsx');

          // ลบลายเซ็นบาร์โค้ดทั้งหมด
          const result = await signature.delete('output.xlsx', signatureLib.SignatureType.Barcode);
          if (result.getSucceeded().size() > 0) {

              // ตรวจสอบผลลัพธ์ของการลบ
              console.log('Following XLSX barcode signatures were deleted:');
              let number = 1;
              result.getSucceeded().toArray().forEach((o) => {
                    const temp = o;
                    console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                    Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
              });
          }
          ```
        platform: "nodejs-java"
        copy_title: "คัดลอก"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นใช้งานหรือยัง?"
  description: "ลองฟีเจอร์ของ GroupDocs.Signature ฟรี หรือขอรับใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "การออกใบอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "สำรวจคุณสมบัติที่เรามีให้"
    exclude: "delete"
    description: "ค้นพบขอบเขตของโซลูชันและการดำเนินการลายเซ็นที่มีอยู่ในระบบของเรา"
    items: 
          
        # operation loop 1
        - name: "ลายเซ็นอิเล็กทรอนิกส์"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "เพิ่มลายเซ็นประเภทต่าง ๆ ในรูปแบบไฟล์ที่รองรับ"

        # operation loop 2
        - name: "เพิ่มข้อความในเอกสาร"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "ปรับปรุงเนื้อหาเอกสารด้วยลายเซ็นข้อความที่ปรับแต่งได้"

        # operation loop 3
        - name: "ลายเซ็นภาพ"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "วางภาพใด ๆ ในตำแหน่งใด ๆ ภายในเอกสาร"

        # operation loop 4
        - name: "สร้างบาร์โค้ด"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "สร้างและแทรกบาร์โค้ดต่าง ๆ ลงในเอกสารที่รองรับ"

        # operation loop 5
        - name: "สร้าง QR Code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "สร้าง QR Codes รวมถึง QR codes สำหรับการลงชื่อในเอกสาร"
          
        # operation loop 6
        - name: "ใบรับรองดิจิตอล"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "รักษาความปลอดภัยในการทำธุรกิจและลงชื่อในเอกสารด้วยใบรับรองดิจิตอล"

        # operation loop 7
        - name: "ลายเซ็นประทับตรา"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "ใช้ Stamp Constructor เพื่อสร้างประทับตรากลมหรือสี่เหลี่ยมที่กำหนดเอง"
          
        # operation loop 8
        - name: "ค้นหาลายเซ็น"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "ค้นหาลายเซ็นที่เพิ่มไว้ในเอกสาร"
          
        # operation loop 9
        - name: "การตรวจสอบลายเซ็น"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "ตรวจสอบความถูกต้องของลายเซ็นหลังจากที่ได้ถูกใช้"
          
        # operation loop 10
        - name: "แก้ไขลายเซ็น"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "แก้ไขลายเซ็นที่หลากหลายภายในเอกสาร"
          
        # operation loop 11
        - name: "ลบลายเซ็น"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "ลบลายเซ็นที่ได้ถูกใช้มาก่อนหน้านี้"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ลบลายเซ็นจากรูปแบบไฟล์ต่าง ๆ"
    exclude: "XLSX"
    description: "โซลูชัน GroupDocs.Signature for Node.js via Java ของเราเชี่ยวชาญในการลบลายเซ็นจากไฟล์มากกว่า 60 รูปแบบ ทำให้มีความเข้ากันได้และฟังก์ชันการทำงานอย่างกว้างขวาง."
    items: 
          
        # format loop 1
        - name: "ลบลายเซ็น PDF"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "รูปแบบเอกสารพกพาของ Adobe"
          
        # format loop 2
        - name: "ลบลายเซ็น DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 3
        - name: "ลบลายเซ็น PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"
          
        # format loop 4
        - name: "ลบลายเซ็น XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "แผ่นงาน Microsoft Excel Open XML"


          

---