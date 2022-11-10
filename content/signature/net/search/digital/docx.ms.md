---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Docx
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Docx with C#

############################# Head ############################
head_title: "Cari tandatangan Digital dalam fail Docx dalam C#"
head_description: "Gunakan .NET untuk mencari tandatangan Digital dalam fail Docx menggunakan beberapa baris kod."

############################# Header ############################
title: "Cari tandatangan Digital dalam fail Docx."
description: "API asli .NET membenarkan untuk mencari tandatangan Digital dalam fail Docx yang telah ditandatangani. Lakukan carian e-tandatangan lanjutan dalam dokumen Docx anda menggunakan beberapa baris kod."
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
    title_left: "Bagaimana untuk mencari tandatangan Digital dalam Docx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) memudahkan pembangun .NET mencari tandatangan Digital dalam fail Docx daripada aplikasi mereka dengan melaksanakan beberapa langkah mudah.
        
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
                
        // Set up input Docx file
        string filePath = "input.docx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Docx document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Cari Digital tandatangan elektronik Demo Langsung"
    content: |
       Cari dokumen untuk pelbagai tandatangan elektronik pada fail Docx sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Cari tandatangan Digital lain menggunakan C#"
    content: |
        "Carian tandatangan elektronik dalam pelbagai dokumen. Cari tandatangan daripada salah satu format fail yang popular seperti yang ditunjukkan di bawah."
    format: 
           
       
back_to_top:
    enable: true
---