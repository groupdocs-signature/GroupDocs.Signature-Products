---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Pdf
productName: Java
lang: id
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Pdf for Java

############################# Head ############################
head_title: "Verifikasi tanda tangan Digital untuk file Pdf melalui Java"
head_description: "Gunakan hanya beberapa baris kode Java untuk memverifikasi dokumen Pdf dan tanda tangan Digital mereka."

############################# Header ############################
title: "Digital verifikasi tanda tangan untuk file Pdf"
description: "API untuk Java memberikan kesempatan untuk memverifikasi tanda tangan Digital pada dokumen Pdf. Verifikasi tanda tangan elektronik di dalam dokumen Pdf Anda dapat dilakukan dengan cepat dan mudah."
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
    title: "Temukan fitur API GroupDocs.Signature for Java baru"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API menyediakan berbagai cara untuk memproses berbagai format dokumen dengan menggunakan tanda tangan elektronik. Banyak jenis tanda tangan digital seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata yang didukung. Pelanggan dapat menambah, menghapus, mengedit, memvalidasi atau mencari tanda tangan digital di PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Sejumlah fitur dan pengaturan tambahan yang menakjubkan tersedia.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara memvalidasi tanda tangan Digital di dokumen Pdf Anda"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyertakan fitur berguna seperti verifikasi tanda tangan Digital yang ditempatkan di dokumen Pdf. Gunakan kesempatan ini tanpa menerapkan kode tambahan.
        
        * Pertama, instantiate kelas Signature yang menyediakan jalur parameter konstruktor ke dokumen yang seharusnya diverifikasi.
        * Kedua, buat objek VerifyOptions baru dan atur semua properti yang diperlukan.
        * Terakhir, aktifkan metode Verify objek Signature dengan melewati instance VerifyOptions.
        * Kemudian proses hasil verifikasi.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for Java didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Unduh versi terbaru GroupDocs.Signature for Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Pdf file
        String filePath = "input.pdf";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dengan Digital tanda tangan Demo Langsung"
    content: |
       Tambahkan berbagai tanda tangan elektronik ke file Pdf sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifikasi tanda tangan Digital lainnya menggunakan Java"
    content: |
        "Verifikasi tanda tangan elektronik yang ditempatkan di berbagai dokumen. Periksa kualitas tanda tangan dalam format file populer seperti yang diungkapkan di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---