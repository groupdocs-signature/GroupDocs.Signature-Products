---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Docx
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Docx for Java

############################# Head ############################
head_title: "Kemas kini tandatangan Text yang diletakkan pada fail Docx dengan Java"
head_description: "Gunakan kod Java yang ringkas dan mudah untuk kemas kini tandatangan Text dalam dokumen Docx yang ditandatangani."

############################# Header ############################
title: "Edit dan kemas kini tandatangan Text yang diletakkan pada fail Docx."
description: "API untuk Java menyediakan kefungsian untuk tandatangan Text mengemas kini pada dokumen Docx. Kemas kini e-tandatangan di dalam dokumen Docx anda dengan beberapa baris kod Java dengan cepat dan mudah."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Ketahui tentang ciri API GroupDocs.Signature for Java."
    content: |
        Kefungsian API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) mengandungi banyak pilihan cara untuk memproses dalam format dokumen permintaan dengan menggunakan tandatangan elektronik. Spektrum luas e-tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata disokong. Pelanggan boleh menambah, mengalih keluar, mengedit, mengesahkan atau mencari tandatangan digital pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Banyak ciri dan tetapan berguna tersedia.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara menukar tandatangan Text dalam dokumen Docx anda"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) termasuk ciri berguna seperti pengemaskinian tandatangan Text yang diletakkan pada dokumen Docx. Ia memungkinkan untuk menukar ciri tandatangan tanpa kod tambahan.
        
        * Sebagai permulaan, buat objek Tandatangan yang lulus sebagai laluan parameter pembina ke dokumen yang sepatutnya dikemas kini.
        * Kemudian, nyatakan objek tandatangan tertentu yang sesuai dan sediakan pengecam dan sifatnya yang perlu diubah.
        * Akhir sekali, panggil kaedah Kemas Kini Tandatangan yang menghantar objek tandatangan tertentu.
        * Proses mengemas kini keputusan kepada notis anda.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Muat turun versi terkini GroupDocs.Signature for Java daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";
        // Set up output file
        String outputFilePath = "output.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Mengemas kini tandatangan Text pada halaman dokumen - Demo Langsung"
    content: |
       Edit pelbagai tandatangan elektronik dokumen Docx sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Kemas kini pelbagai tandatangan Text melalui Java"
    content: |
        "Mengedit tandatangan digital yang diletakkan dalam pelbagai format dokumen. Kemas kini data tandatangan tanpa kod tambahan."
    format: 
       
       
back_to_top:
    enable: true
---