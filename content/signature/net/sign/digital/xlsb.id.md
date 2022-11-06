---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: id
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for C#

############################# Head ############################
head_title: "Menambahkan tanda tangan elektronik digital ke file Xlsb dengan C#"
head_description: "Letakkan Tanda Tangan Digital pada file Xlsb untuk .NET menggunakan beberapa baris kode. Gunakan GroupDocs Document Signature API untuk menandatangani lusinan format file."

############################# Header ############################
title: "eSign Xlsb file dengan Digital tanda tangan di C#"
description: "Cara menambahkan tanda tangan Digital dengan beberapa baris kode .NET"
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
    title: "Tentang GroupDocs.Signature for .NET API tanda tangan digital"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) adalah API populer untuk menandatangani dokumen dengan tanda tangan elektronik digital, dengan sertifikat digital. Untuk tanda tangan digital, API menggunakan file sertifikat PFX untuk menandatangani dokumen dengan kunci pribadi dan publik yang dilindungi kata sandi. Tanda tangan digital dapat digunakan untuk mengesahkan dokumen bisnis dengan halaman tertentu eSign PDF, mengesahkan seluruh dokumen Microsoft Office seperti Words, Excel, file Powerpoint, dan dokumen Open Office. Pelanggan dapat dengan mudah memanipulasi tanda tangan seperti mengedit, menghapus, atau menyesuaikan. API menyediakan cara untuk mencari dan memverifikasi tanda tangan. Selain itu, banyak kemampuan untuk kustomisasi tanda tangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Xlsb dengan Digital di C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memberikan kemampuan untuk menandatangani dokumen Xlsb dengan Digital tanda tangan dengan cepat dan mudah.
        
        * Buat instance kelas Signature yang menyediakan file Xlsb yang seharusnya ditandatangani sebagai jalur atau aliran memori
        * Buat instance kelas SignOptions dan atur semua data yang diminta.
        * Aktifkan metode Signature.Sign() dengan meneruskan file Xlsb atau aliran memori

    title_right: " Persyaratan sistem"
    content_right: |
        GroupDocs.Signature for .NET didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan pengembangan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terbaru dari [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Xlsb file
        string filePath = "input.xlsb";
        // Set up output file
        string outputFilePath = "output.xlsb";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Xlsb document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Menandatangani dokumen Xlsb dengan Digital Demo Langsung"
    content: |
       Tanda tangani file Xlsb dengan berbagai tanda tangan sekarang juga dengan mengunjungi situs web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo online gratis menunggu Anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tanda tangan Digital lain yang didukung untuk C#"
    content: |
        "Anda juga dapat menandatangani Xlsb dengan jenis tanda tangan lainnya. Silakan lihat daftarnya di bawah ini."
    format: 
       
       
back_to_top:
    enable: true
---