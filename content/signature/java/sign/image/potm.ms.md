---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Potm
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Potm for Java

############################# Head ############################
head_title: "Menambahkan tandatangan Image pada fail Potm dengan Java"
head_description: "Letakkan Image Tandatangan pada fail Potm untuk Java menggunakan beberapa baris kod. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani berpuluh-puluh format fail."

############################# Header ############################
title: "Tandatangani fail Potm dengan tandatangan Image dalam Java"
description: "Bagaimana untuk menambah Image Tandatangan dengan beberapa baris kod Java."
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
    title: "Perihal GroupDocs.Signature for Java API tandatangan imej"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ialah API popular untuk tandatangan elektronik dokumen digital. Tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata tersedia. Tandatangan mungkin diletakkan pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Pelanggan boleh menandatangani dokumen mereka dan mengemas kini, mencari, mengesahkan, memadam atau pratonton e-tandatangan yang diletakkan pada dokumen tersebut. Selain itu, banyak kebolehan untuk penyesuaian tandatangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Potm dengan Image dalam Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan keupayaan untuk menandatangani dokumen Potm dengan tandatangan Image dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Potm yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Potm atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terkini daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";
        // Set up output file
        String outputFilePath = "output.potm";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Potm document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Potm dengan Image Demo Langsung"
    content: |
       Tandatangani fail Potm dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Image lain yang disokong untuk Java"
    content: |
        "Anda juga boleh menandatangani Potm dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
       
       
back_to_top:
    enable: true
---