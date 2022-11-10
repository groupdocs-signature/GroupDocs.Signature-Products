---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Text
fileformat: Dotx
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Dotx for Java

############################# Head ############################
head_title: "Hapus tanda tangan Text dari file Dotx melalui Java"
head_description: "Penghapusan tanda tangan Text tertentu dari dokumen Dotx yang ditandatangani dapat dilakukan dengan mudah dengan kode Java singkat."

############################# Header ############################
title: "Hapus tanda tangan Text yang ditempatkan di file Dotx"
description: "Hapus berbagai tanda tangan Text dari dokumen Dotx. Menghapus tanda tangan Text memerlukan kode Java sederhana."
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
    title: "Dapatkan informasi tentang GroupDocs.Signature for Java fitur API"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API menyediakan banyak cara untuk memproses dokumen Anda menggunakan tanda tangan elektronik. Tanda tangan digital seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata tersedia. Pelanggan memiliki kemungkinan untuk menambah, menghapus, memperbarui, memverifikasi atau mencari tanda tangan digital di PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Sejumlah besar fitur dan pengaturan yang berguna disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara menghapus tanda tangan Text dari dokumen Dotx Anda"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan fitur yang berguna untuk membersihkan dokumen Dotx dari Text tanda tangan dengan beberapa baris kode.
        
        * Pertama, buat instance objek Signature yang meneruskan jalur ke dokumen Anda sebagai parameter konstruktor.
        * Kemudian, buat objek tanda tangan yang sesuai dan atur pengenal uniknya.
        * Setelah itu, aktifkan metode Hapus dengan melewati objek tanda tangan yang harus dihapus.
        * Terakhir, proses hasil operasi.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Unduh versi terbaru GroupDocs.Signature for Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Dotx file
        String filePath = "input.dotx";
        // Set up output file
        String outputFilePath = "output.dotx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

        // provide signature features to delete
        TextSignature signatureToDelete = new TextSignature(id);

        // delete signature
        Boolean deleteResult = signature.delete(outputFilePath, signatureToDelete);

        // process deletion result
        if (deleteResult)
        {
                System.out.println("Signature was deleted successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dengan Text tanda tangan Demo Langsung"
    content: |
       Tambahkan berbagai tanda tangan elektronik ke file Dotx sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Hapus tanda tangan Text Anda dengan Java"
    content: |
        "Penghapusan tanda tangan elektronik yang ditambahkan ke berbagai format dokumen. Hapus tanda tangan dengan cepat tanpa kode tambahan."
    format: 
       
       
back_to_top:
    enable: true
---