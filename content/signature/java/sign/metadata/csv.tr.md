---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Csv
productName: Java
lang: tr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Csv for Java

############################# Head ############################
head_title: "Java aracılığıyla Csv belgelerine Meta Veri elektronik imzaları ekleyin"
head_description: "Meta Verileri, birkaç satır Java kodu kullanarak Csv belgelerinizin içinde gizli elektronik imzalar olarak kullanın. İş belgelerinizi ve dosyalarınızı Meta Veri bilgileriyle e-imzalamak için GroupDocs Belge İmza API'sini kullanın."

############################# Header ############################
title: "Java aracılığıyla Csv belgesi için meta veri elektronik imzaları basit ve kullanımı kolaydır!"
description: "Gizli Meta Veri girişleriyle Csv belgelerinizi ve sözleşmelerinizi e-imzalayın. PDF'ler, MS Word belgeleri, MS Excel çalışma kitapları, MS PowerPoint sunumları ve çeşitli görüntü formatları için sorunsuz ve ekstra kodlama olmadan Meta Veriler oluşturun."
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
    title: "GroupDocs.Signature for Java Meta veri imzaları API'si hakkında"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), dijital belge e-imzalama için popüler bir API'dir. Metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi imzalar mevcuttur. İmzalar PDF'lere, MS Word belgelerine, MS Excel çalışma kitaplarına, MS PowerPoint sunumlarına, Adobe Photoshop dosyalarına ve çeşitli görüntü biçimlerine yerleştirilebilir. Müşteriler, belgelerini imzalayabilir ve bu belgelere konan e-imzaları güncelleyebilir, arayabilir, doğrulayabilir, silebilir veya önizleyebilir. Ayrıca, imza özelleştirme için birçok yetenek sağlanmıştır.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java içinde Metadata ile Csv imzalama adımları"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), Csv belgelerini Metadata imzasıyla hızlı ve kolay bir şekilde imzalama olanağı sağlar.
        
        * Yol veya bellek akışı olarak imzalaması gereken Csv dosyasını sağlayan bir Signature sınıfı örneği oluşturun
        * SignOptions sınıfını örnekleyin ve istenen tüm verileri ayarlayın.
        * Çıkış Csv dosyasını veya bellek akışını geçen Signature.Sign() yöntemini çağırın

    title_right: " sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for Java, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * En son GroupDocs.Signature for Java ürününü [Maven}](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) adresinden edinin
         
    code: |
        ```java    
                
        // Set up input Csv file
        String filePath = "input.csv";
        // Set up output file
        String outputFilePath = "output.csv";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // instantiate metadata signing options
        MetadataSignOptions options = new MetadataSignOptions();

        // setup Author property
        SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
        options.getSignatures().add(mdSign_Author);
        // setup document data
        SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", new Date());// Datetime value
        options.getSignatures().add(mdSign_DocData);
        // setup document id
        SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
        options.getSignatures().add(mdSign_DocId);

        // sign Csv document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Csv dokümanı Metadata Canlı Demo ile imzalama"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek çeşitli imzalarla Csv dosyasını imzalayın. Ücretsiz çevrimiçi demo sizi bekliyor.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java için desteklenen diğer Metadata imzaları"
    content: |
        "Csv'ı diğer imza türleriyle de imzalayabilirsiniz. Lütfen aşağıdaki listeye bakın."
    format: 
       
       
back_to_top:
    enable: true
---