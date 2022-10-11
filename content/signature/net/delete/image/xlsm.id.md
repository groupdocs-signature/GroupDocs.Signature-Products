---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Image
fileformat: Xlsm
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Image signature on Xlsm for C#

############################# Head ############################
head_title: "Hapus tanda tangan Image dari file Xlsm melalui C#"
head_description: "Penghapusan tanda tangan Image tertentu dari dokumen Xlsm yang ditandatangani dapat dilakukan dengan mudah dengan kode .NET singkat."

############################# Header ############################
title: "Hapus tanda tangan Image yang ditempatkan di file Xlsm"
description: "Hapus berbagai tanda tangan Image dari dokumen Xlsm. Menghapus tanda tangan Image memerlukan kode C# sederhana."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "Dapatkan informasi tentang GroupDocs.Signature for .NET fitur API"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) API menyediakan banyak cara untuk memproses dokumen Anda menggunakan tanda tangan elektronik. Tanda tangan digital seperti teks, gambar, sertifikat digital, kode batang, kode QR, perangko, atau metadata tersedia. Pelanggan memiliki kemungkinan untuk menambah, menghapus, memperbarui, memverifikasi atau mencari tanda tangan digital di PDF, dokumen MS Word, buku kerja MS Excel, presentasi MS PowerPoint, file Adobe Photoshop dan berbagai format gambar. Sejumlah besar fitur dan pengaturan yang berguna disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Cara menghapus tanda tangan Image dari dokumen Xlsm Anda"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan fitur yang berguna untuk membersihkan dokumen Xlsm dari Image tanda tangan dengan beberapa baris kode.
        
        * Pertama, buat instance objek Signature yang meneruskan jalur ke dokumen Anda sebagai parameter konstruktor.
        * Kemudian, buat objek tanda tangan yang sesuai dan atur pengenal uniknya.
        * Setelah itu, aktifkan metode Hapus dengan melewati objek tanda tangan yang harus dihapus.
        * Terakhir, proses hasil operasi.

    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Signature for .NET dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsm file
        string filePath = "input.xlsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "e3ad0ec7-9abf-426d-b9aa-b3328f3f1470";

                // provide signature features to delete
                // set up particular signature id
                ImageSignature signatureToDelete = new ImageSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dengan Image tanda tangan Demo Langsung"
    content: |
       Tambahkan berbagai tanda tangan elektronik ke file Xlsm sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Hapus tanda tangan Image Anda dengan C#"
    content: |
        "Penghapusan tanda tangan elektronik yang ditambahkan ke berbagai format dokumen. Hapus tanda tangan dengan cepat tanpa kode tambahan."
    format: 
       
       
back_to_top:
    enable: true
---