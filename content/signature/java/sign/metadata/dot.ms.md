---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Dot
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Dot for Java

############################# Head ############################
head_title: "Tambahkan tandatangan elektronik Metadata pada dokumen Dot melalui Java"
head_description: "Gunakan Metadata sebagai tandatangan elektronik tersembunyi di dalam dokumen Dot anda menggunakan beberapa baris kod Java. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani dokumen dan fail perniagaan anda dengan maklumat Metadata."

############################# Header ############################
title: "Tandatangan elektronik metadata untuk dokumen Dot melalui Java adalah mudah dan mudah untuk digunakan!"
description: "eTandatangani dokumen dan kontrak Dot anda dengan entri Metadata tersembunyi. Jana Metadata untuk PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint dan pelbagai format imej tanpa masalah dan pengekodan tambahan."
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
    title: "Perihal GroupDocs.Signature for Java API tandatangan metadata"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) ialah API popular untuk tandatangan elektronik dokumen digital. Tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata tersedia. Tandatangan mungkin diletakkan pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Pelanggan boleh menandatangani dokumen mereka dan mengemas kini, mencari, mengesahkan, memadam atau pratonton e-tandatangan yang diletakkan pada dokumen tersebut. Selain itu, banyak kebolehan untuk penyesuaian tandatangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Dot dengan Metadata dalam Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan keupayaan untuk menandatangani dokumen Dot dengan tandatangan Metadata dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Dot yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Dot atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terkini daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";
        // Set up output file
        String outputFilePath = "output.dot";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        WordProcessingMetadataSignature mdSign_Author = new WordProcessingMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        WordProcessingMetadataSignature mdSign_DocData = new WordProcessingMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        WordProcessingMetadataSignature mdSign_DocId = new WordProcessingMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Dot document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Dot dengan Metadata Demo Langsung"
    content: |
       Tandatangani fail Dot dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Metadata lain yang disokong untuk Java"
    content: |
        "Anda juga boleh menandatangani Dot dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
       
       
back_to_top:
    enable: true
---