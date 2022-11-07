---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Docm
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Docm for Java

############################# Head ############################
head_title: "Padamkan tandatangan Qrcode daripada fail Docm melalui Java"
head_description: "Pemadaman tandatangan Qrcode tertentu daripada dokumen Docm yang ditandatangani mungkin dilakukan dengan mudah dengan kod Java pendek."

############################# Header ############################
title: "Alih keluar tandatangan Qrcode yang diletakkan dalam fail Docm."
description: "Padamkan pelbagai tandatangan Qrcode daripada dokumen Docm. Mengalih keluar tandatangan Qrcode memerlukan kod Java yang mudah."
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
    title: "Dapatkan maklumat tentang ciri API GroupDocs.Signature for Java."
    content: |
        API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan banyak cara untuk memproses dokumen anda menggunakan tandatangan elektronik. Tandatangan digital seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata tersedia. Pelanggan mempunyai kemungkinan untuk menambah, memadam, mengemas kini, mengesahkan atau mencari tandatangan digital pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Sebilangan besar ciri dan tetapan berguna disediakan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mengalih keluar tandatangan Qrcode daripada dokumen Docm anda"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan ciri berguna untuk mengosongkan Docm dokumen daripada Qrcode tandatangan dengan beberapa baris kod.
        
        * Pertama, nyatakan laluan laluan objek Tandatangan ke dokumen anda sebagai parameter pembina.
        * Kemudian, cipta objek tandatangan yang sesuai dan sediakan pengecam uniknya.
        * Selepas itu, gunakan kaedah Padam menghantar objek tandatangan yang mesti dipadamkan.
        * Akhirnya, hasil operasi proses.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Muat turun versi terkini GroupDocs.Signature for Java daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";
        // Set up output file
        String outputFilePath = "output.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be deleted
        // such Id may be obtained as result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to delete
        QrCodeSignature signatureToDelete = new QrCodeSignature(id);

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
    title: "Menandatangani dengan Qrcode tandatangan Demo Langsung"
    content: |
       Tambahkan pelbagai tandatangan elektronik pada fail Docm sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Padamkan tandatangan Qrcode anda dengan Java"
    content: |
        "Pemadaman e-tandatangan yang telah ditambahkan pada pelbagai format dokumen. Alih keluar tandatangan dengan cepat tanpa kod tambahan."
    format: 
       
       
back_to_top:
    enable: true
---