---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Xlsm
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Xlsm for Java

############################# Head ############################
head_title: "Buat tanda tangan elektronik Teks ke file Xlsm dengan Java"
head_description: "Letakkan Text eSignature pada file Xlsm untuk Java menggunakan beberapa baris kode. Gunakan GroupDocs Document Signature API untuk menandatangani lusinan format file."

############################# Header ############################
title: "Tanda tangani file Xlsm dengan tanda tangan Text di Java"
description: "Cara menambahkan Tanda Tangan Text dengan beberapa baris kode Java"
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
    title: "Tentang GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) adalah API populer untuk penandatanganan elektronik dokumen digital. Tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata tersedia. Tanda tangan dapat ditempatkan pada PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Pelanggan dapat menandatangani dokumen mereka dan memperbarui, mencari, memverifikasi, menghapus, atau melihat pratinjau tanda tangan elektronik yang diletakkan pada dokumen tersebut. Selain itu, banyak kemampuan untuk kustomisasi tanda tangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Xlsm dengan Text di Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) memberikan kemampuan untuk menandatangani dokumen Xlsm dengan Text tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Xlsm yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Xlsm atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terbaru dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Xlsm file
        String filePath = "input.xlsm";
        // Set up output file
        String outputFilePath = "output.xlsm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Xlsm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Xlsm dengan Text Demo Langsung"
    content: |
       Tanda tangani file Xlsm dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Text lain yang didukung untuk Java"
    content: |
        "Anda juga dapat menandatangani Xlsm dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---