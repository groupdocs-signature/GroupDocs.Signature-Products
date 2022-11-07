---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Xlsb
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Xlsb for C#

############################# Head ############################
head_title: "Menambahkan tandatangan elektronik Digital pada fail Xlsb dengan C#"
head_description: "Letakkan Tandatangan Digital pada fail Xlsb untuk .NET menggunakan beberapa baris kod. Gunakan API Tandatangan Dokumen GroupDocs untuk menandatangani berpuluh-puluh format fail."

############################# Header ############################
title: "eSign Xlsb fail dengan Digital tandatangan dalam C#"
description: "Cara menambah tandatangan Digital dengan beberapa baris kod .NET."
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
    title: "Perihal GroupDocs.Signature for .NET API tandatangan digital"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) ialah API popular untuk menandatangani dokumen dengan tandatangan elektronik digital, dengan sijil digital. Untuk API tandatangan Digital menggunakan fail sijil PFX untuk menandatangani dokumen dengan kunci peribadi dan awam yang dilindungi kata laluan. Tandatangan Digital mungkin digunakan untuk mengesahkan dokumen perniagaan dengan halaman tertentu eSign PDF, memperakui keseluruhan dokumen Microsoft Office seperti Words, Excel, fail Powerpoint dan dokumen Open Office. Pelanggan boleh memanipulasi tandatangan dengan mudah seperti mengeditnya, mengalih keluar atau melaraskannya. API menyediakan cara untuk mencari dan mengesahkan tandatangan. Selain itu, banyak kebolehan untuk penyesuaian tandatangan disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Langkah-langkah untuk menandatangani Xlsb dengan Digital dalam C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan keupayaan untuk menandatangani dokumen Xlsb dengan tandatangan Digital dengan cepat dan mudah.
        
        * Buat contoh kelas Tandatangan yang menyediakan fail Xlsb yang sepatutnya ditandatangani sebagai laluan atau aliran memori
        * Segerakan kelas SignOptions dan tetapkan semua data yang diminta.
        * Guna kaedah Signature.Sign() yang menghantar fail keluaran Xlsb atau aliran memori

    title_right: " Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Dapatkan GroupDocs.Signature for .NET terkini daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
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
       Tandatangani fail Xlsb dengan pelbagai tandatangan sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demo dalam talian percuma menanti anda.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Tandatangan Digital lain yang disokong untuk C#"
    content: |
        "Anda juga boleh menandatangani Xlsb dengan jenis tandatangan lain. Sila lihat senarai di bawah."
    format: 
       
       
back_to_top:
    enable: true
---