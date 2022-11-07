---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Barcode
fileformat: Rtf
productName: .NET
lang: ms
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Rtf for C#

############################# Head ############################
head_title: "Padamkan tandatangan Barcode daripada fail Rtf melalui C#"
head_description: "Pemadaman tandatangan Barcode tertentu daripada dokumen Rtf yang ditandatangani mungkin dilakukan dengan mudah dengan kod .NET pendek."

############################# Header ############################
title: "Alih keluar tandatangan Barcode yang diletakkan dalam fail Rtf."
description: "Padamkan pelbagai tandatangan Barcode daripada dokumen Rtf. Mengalih keluar tandatangan Barcode memerlukan kod C# yang mudah."
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
    title: "Dapatkan maklumat tentang ciri API GroupDocs.Signature for .NET."
    content: |
        API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan banyak cara untuk memproses dokumen anda menggunakan tandatangan elektronik. Tandatangan digital seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata tersedia. Pelanggan mempunyai kemungkinan untuk menambah, memadam, mengemas kini, mengesahkan atau mencari tandatangan digital pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Sebilangan besar ciri dan tetapan berguna disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mengalih keluar tandatangan Barcode daripada dokumen Rtf anda"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) menyediakan ciri berguna untuk mengosongkan Rtf dokumen daripada Barcode tandatangan dengan beberapa baris kod.
        
        * Pertama, nyatakan laluan laluan objek Tandatangan ke dokumen anda sebagai parameter pembina.
        * Kemudian, cipta objek tandatangan yang sesuai dan sediakan pengecam uniknya.
        * Selepas itu, gunakan kaedah Padam menghantar objek tandatangan yang mesti dipadamkan.
        * Akhirnya, hasil operasi proses.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for .NET disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Muat turun versi terkini GroupDocs.Signature for .NET daripada [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Rtf file
        string filePath = "input.rtf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "07f83369-318b-41ad-a843-732417b912c2";

                // provide signature features to delete
                // set up particular signature id
                BarcodeSignature signatureToDelete = new BarcodeSignature(id);

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
    title: "Menandatangani dengan Barcode tandatangan Demo Langsung"
    content: |
       Tambahkan pelbagai tandatangan elektronik pada fail Rtf sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Padamkan tandatangan Barcode anda dengan C#"
    content: |
        "Pemadaman e-tandatangan yang telah ditambahkan pada pelbagai format dokumen. Alih keluar tandatangan dengan cepat tanpa kod tambahan."
    format: 
       
       
back_to_top:
    enable: true
---