---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Pps
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Pps for Java

############################# Head ############################
head_title: "Tambahkan tanda tangan elektronik Metadata ke dokumen Pps melalui Java"
head_description: "Gunakan Metadata sebagai tanda tangan elektronik tersembunyi di dalam dokumen Pps Anda menggunakan beberapa baris kode Java. Gunakan API Tanda Tangan Dokumen GroupDocs untuk menandatangani dokumen dan file bisnis Anda secara elektronik dengan informasi Metadata."

############################# Header ############################
title: "Tanda tangan elektronik metadata untuk dokumen Pps melalui Java sederhana dan mudah digunakan!"
description: "eSign dokumen dan kontrak Pps Anda dengan entri Metadata tersembunyi. Hasilkan Metadata untuk PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint dan berbagai format gambar tanpa masalah dan pengkodean tambahan."
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
    title: "Tentang GroupDocs.Signature for Java Metadata signatures API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) adalah API populer untuk penandatanganan elektronik dokumen digital. Tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata tersedia. Tanda tangan dapat ditempatkan pada PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Pelanggan dapat menandatangani dokumen mereka dan memperbarui, mencari, memverifikasi, menghapus, atau melihat pratinjau tanda tangan elektronik yang diletakkan pada dokumen tersebut. Selain itu, banyak kemampuan untuk kustomisasi tanda tangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Pps dengan Metadata di Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) memberikan kemampuan untuk menandatangani dokumen Pps dengan Metadata tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Pps yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Pps atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Dapatkan GroupDocs.Signature for Java terbaru dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pps file
        String filePath = "input.pps";
        // Set up output file
        String outputFilePath = "output.pps";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        PresentationMetadataSignature mdSign_Author = new PresentationMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        PresentationMetadataSignature mdSign_DocData = new PresentationMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        PresentationMetadataSignature mdSign_DocId = new PresentationMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Pps document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Pps dengan Metadata Demo Langsung"
    content: |
       Tanda tangani file Pps dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Metadata lain yang didukung untuk Java"
    content: |
        "Anda juga dapat menandatangani Pps dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---