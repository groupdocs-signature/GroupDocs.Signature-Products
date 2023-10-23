---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Text
fileformat: Tar
productName: Java
lang: ms
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Tar for Java

############################# Head ############################
head_title: "Pengesahan tandatangan Text untuk fail Tar melalui Java"
head_description: "Gunakan hanya beberapa baris kod Java untuk mengesahkan dokumen Tar dan tandatangan Text mereka."

############################# Header ############################
title: "Text pengesahan tandatangan untuk fail Tar."
description: "API untuk Java memberi peluang untuk mengesahkan tandatangan Text pada dokumen Tar. Pengesahan e-tandatangan di dalam dokumen Tar anda mungkin dilakukan dengan cepat dan mudah."
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
    title: "Temui ciri API GroupDocs.Signature for Java baharu"
    content: |
        API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) menyediakan pelbagai cara untuk memproses pelbagai format dokumen dengan menggunakan tandatangan elektronik. Banyak jenis tandatangan digital seperti teks, imej, sijil digital, kod bar, kod QR, setem atau metadata disokong. Pelanggan boleh menambah, mengalih keluar, mengedit, mengesahkan atau mencari tandatangan digital pada PDF, dokumen MS Word, buku kerja MS Excel, persembahan MS PowerPoint, fail Adobe Photoshop dan pelbagai format imej. Terdapat banyak ciri dan tetapan tambahan yang menakjubkan.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Bagaimana untuk mengesahkan tandatangan Text dalam dokumen Tar anda"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) termasuk ciri berguna seperti pengesahan tandatangan Text yang diletakkan pada dokumen Tar. Gunakan peluang ini tanpa melaksanakan kod tambahan.
        
        * Pertama, nyatakan kelas Tandatangan yang menyediakan sebagai laluan parameter pembina kepada dokumen yang sepatutnya disahkan.
        * Kedua, cipta objek VerifyOptions baharu dan sediakan semua sifat yang diperlukan.
        * Akhir sekali, gunakan kaedah Verify objek Tandatangan yang lulus contoh VerifyOptions.
        * Kemudian proses hasil pengesahan.

    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Signature for Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.

        * Sistem pengendalian: Microsoft Windows, Linux, MacOS
        * Persekitaran pembangunan: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Muat turun versi terkini GroupDocs.Signature for Java daripada [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tar file
        String filePath = "input.tar";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        TextVerifyOptions options = new TextVerifyOptions();

        // Process all pages
        options.setAllPages(true);
        // specify text match type
        options.setMatchType(TextMatchType.Exact);
        // specify text pattern to search
        options.setText("Very important signature");
                            
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
    title: "Menandatangani dengan Text tandatangan Demo Langsung"
    content: |
       Tambahkan pelbagai tandatangan elektronik pada fail Tar sekarang dengan melawati tapak web [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Sahkan tandatangan Text lain menggunakan Java"
    content: |
        "Pengesahan tandatangan elektronik yang diletakkan dalam pelbagai dokumen. Semak kualiti tandatangan dalam format fail popular seperti yang didedahkan di bawah."
    format: 
       
       
back_to_top:
    enable: true
---