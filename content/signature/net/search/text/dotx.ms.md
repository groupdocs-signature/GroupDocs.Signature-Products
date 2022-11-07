---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Dotx
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Dotx with C#

############################# Head ############################
head_title: "Cari tandatangan Text dalam fail Dotx dalam C#"
head_description: "Gunakan .NET untuk mencari tandatangan Text dalam fail Dotx menggunakan beberapa baris kod."

############################# Header ############################
title: "Cari tandatangan Text dalam fail Dotx."
description: "API asli .NET membenarkan untuk mencari tandatangan Text dalam fail Dotx yang telah ditandatangani. Lakukan carian e-tandatangan lanjutan dalam dokumen Dotx anda menggunakan beberapa baris kod."
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
    title: "Mengenai API GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan API .NET untuk memproses dokumen menggunakan pelbagai jenis tandatangan seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata. Pengguna boleh menambah, memadam, mengemas kini, mengesahkan atau mencari tandatangan elektronik dalam PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej, dengan sokongan tambahan untuk menyesuaikan sifat tandatangan mengikut keperluan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mencari tandatangan Text dalam Dotx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memudahkan pembangun .NET mencari tandatangan Text dalam fail Dotx daripada aplikasi mereka dengan melaksanakan beberapa langkah mudah.
        
        * Buat contoh baharu kelas Tandatangan dan lulus laluan dokumen sumber sebagai parameter pembina.
        * Segerakan objek SearchOptions mengikut keperluan anda dan tentukan pilihan carian.
        * Panggil kaedah Carian contoh kelas Tandatangan dan berikan SearchOptions kepadanya.
        * Proses hasil carian mengikut permintaan anda.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Muat turun versi terkini GroupDocs.Signature for .NET daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                TextSearchOptions options = new TextSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // specify text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature"
                };

                // search for Text signatures in Dotx document
                List<TextSignature> signatures = signature.Search<TextSignature>(options);

                // process signatures which were found                
                foreach (TextSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cari Text tandatangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk pelbagai tandatangan elektronik pada fail Dotx sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tandatangan Text lain menggunakan C#"
    content: |
        "Carian tandatangan elektronik dalam pelbagai dokumen. Cari tandatangan daripada salah satu format fail yang popular seperti yang ditunjukkan di bawah."
    format: 
           
       
back_to_top:
    enable: true
---