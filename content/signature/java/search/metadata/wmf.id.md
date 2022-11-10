---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Wmf
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Wmf with Java

############################# Head ############################
head_title: "Cari tanda tangan Metadata dalam file Wmf di Java"
head_description: "Gunakan Java untuk mencari tanda tangan Metadata di file Wmf menggunakan beberapa baris kode."

############################# Header ############################
title: "Cari tanda tangan Metadata di file Wmf"
description: "Java API asli memungkinkan untuk mencari Metadata tanda tangan di file Wmf yang sudah ditandatangani. Lakukan pencarian tanda tangan elektronik lanjutan dalam dokumen Wmf Anda menggunakan beberapa baris kode."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for Java API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan Java API untuk memproses dokumen menggunakan berbagai jenis tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, stempel, atau metadata. Pengguna dapat menambah, menghapus, memperbarui, memverifikasi atau mencari tanda tangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar, dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara mencari tanda tangan Metadata di Wmf"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) memudahkan pengembang Java untuk mencari tanda tangan Metadata dalam file Wmf dari aplikasi mereka dengan menerapkan beberapa langkah mudah.
        
        * Buat instance baru kelas Signature dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek SearchOptions sesuai dengan kebutuhan Anda dan tentukan opsi pencarian.
        * Panggil metode Pencarian dari instance kelas Signature dan berikan SearchOptions ke sana.
        * Proses pencarian hasil sesuai dengan permintaan Anda.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Unduh versi terbaru GroupDocs.Signature for Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
        
        // Set up input Wmf file
        String filePath = "input.wmf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Wmf document
        List<ImageMetadataSignature> signatures = signature.search(ImageMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Telusuri Metadata tanda tangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk berbagai tanda tangan elektronik ke file Wmf sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tanda tangan Metadata lainnya menggunakan Java"
    content: |
        "Pencarian tanda tangan elektronik di berbagai dokumen. Temukan tanda tangan dari salah satu format file populer seperti yang ditunjukkan di bawah ini."
    format: 
           
       
back_to_top:
    enable: true
---