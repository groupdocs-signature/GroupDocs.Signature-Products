---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Dotx
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Dotx with C#

############################# Head ############################
head_title: "Cari tanda tangan Metadata dalam file Dotx di C#"
head_description: "Gunakan .NET untuk mencari tanda tangan Metadata di file Dotx menggunakan beberapa baris kode."

############################# Header ############################
title: "Cari tanda tangan Metadata di file Dotx"
description: ".NET API asli memungkinkan untuk mencari Metadata tanda tangan di file Dotx yang sudah ditandatangani. Lakukan pencarian tanda tangan elektronik lanjutan dalam dokumen Dotx Anda menggunakan beberapa baris kode."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for .NET API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan .NET API untuk memproses dokumen menggunakan berbagai jenis tanda tangan seperti teks, gambar, sertifikat digital, kode batang, kode QR, stempel, atau metadata. Pengguna dapat menambah, menghapus, memperbarui, memverifikasi atau mencari tanda tangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar, dengan dukungan tambahan untuk menyesuaikan properti tanda tangan sesuai kebutuhan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara mencari tanda tangan Metadata di Dotx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memudahkan pengembang .NET untuk mencari tanda tangan Metadata dalam file Dotx dari aplikasi mereka dengan menerapkan beberapa langkah mudah.
        
        * Buat instance baru kelas Signature dan teruskan jalur dokumen sumber sebagai parameter konstruktor.
        * Buat instance objek SearchOptions sesuai dengan kebutuhan Anda dan tentukan opsi pencarian.
        * Panggil metode Pencarian dari instance kelas Signature dan berikan SearchOptions ke sana.
        * Proses pencarian hasil sesuai dengan permintaan Anda.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature for .NET dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // search for Metadata signatures in Dotx document
                List<WordProcessingMetadataSignature> signatures = signature.Search<WordProcessingMetadataSignature>(SignatureType.Metadata);

                // process signatures which were found 
                foreach (WordProcessingMetadataSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Telusuri Metadata tanda tangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk berbagai tanda tangan elektronik ke file Dotx sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tanda tangan Metadata lainnya menggunakan C#"
    content: |
        "Pencarian tanda tangan elektronik di berbagai dokumen. Temukan tanda tangan dari salah satu format file populer seperti yang ditunjukkan di bawah ini."
    format: 
           
       
back_to_top:
    enable: true
---