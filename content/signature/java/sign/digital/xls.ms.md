---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xls
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xls for Java

############################# Head ############################
head_title: "Menambahkan tandatangan elektronik Digital pada fail Xls dengan Java"
head_description: "Letakkan Tandatangan Digital pada fail Xls untuk Java menggunakan beberapa baris kod. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani berpuluh-puluh format fail."

############################# Header ############################
title: "eSign Xls fail dengan Digital tandatangan dalam Java"
description: "Cara menambah tandatangan Digital dengan beberapa baris kod Java."
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
    title: "Perihal GroupDocs.Signature for Java API tandatangan digital"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ialah API popular untuk menandatangani dokumen dengan tandatangan elektronik digital, dengan sijil digital. Untuk API tandatangan Digital menggunakan fail sijil PFX untuk menandatangani dokumen dengan kunci peribadi dan awam yang dilindungi kata laluan. Tandatangan Digital mungkin digunakan untuk mengesahkan dokumen perniagaan dengan halaman tertentu eSign PDF, memperakui keseluruhan dokumen Microsoft Office seperti Words, Excel, fail Powerpoint dan dokumen Open Office. Pelanggan boleh memanipulasi tandatangan dengan mudah seperti mengeditnya, mengalih keluar atau melaraskannya. API menyediakan cara untuk mencari dan mengesahkan tandatangan. Selain itu, banyak kebolehan untuk penyesuaian tandatangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Xls dengan Digital dalam Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan keupayaan untuk menandatangani dokumen Xls dengan tandatangan Digital dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Xls yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Xls atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terkini daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xls file
        String filePath = "input.xls";
        // Set up output file
        String outputFilePath = "output.xls";
        // Provide digital certificate
        String certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        DigitalSignOptions options = new DigitalSignOptions(certificateFilePath);

        // set certificate password
        options.setPassword("1234567890");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xls document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Xls dengan Digital Demo Langsung"
    content: |
       Tandatangani fail Xls dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Digital lain yang disokong untuk Java"
    content: |
        "Anda juga boleh menandatangani Xls dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
       
       
back_to_top:
    enable: true
---