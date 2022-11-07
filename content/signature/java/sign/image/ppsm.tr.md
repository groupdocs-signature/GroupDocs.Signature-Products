---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Image
fileformat: Ppsm
productName: Java
lang: tr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Image signature on Ppsm for Java

############################# Head ############################
head_title: "Java ile Ppsm dosyasına Image imza ekleme"
head_description: "Birkaç satır kod kullanarak Java için Ppsm dosyasına Image İmza koyun. Düzinelerce dosya biçimini imzalamak için GroupDocs Belge İmza API'sini kullanın."

############################# Header ############################
title: "Ppsm dosyalarını Image imzasıyla Java içinde imzalayın"
description: "Birkaç satır Java koduyla Image İmzası nasıl eklenir"
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
    title: "GroupDocs.Signature for Java Resim imzaları API'si hakkında"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), dijital belge e-imzalama için popüler bir API'dir. Metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi imzalar mevcuttur. İmzalar PDF'lere, MS Word belgelerine, MS Excel çalışma kitaplarına, MS PowerPoint sunumlarına, Adobe Photoshop dosyalarına ve çeşitli görüntü biçimlerine yerleştirilebilir. Müşteriler, belgelerini imzalayabilir ve bu belgelere konan e-imzaları güncelleyebilir, arayabilir, doğrulayabilir, silebilir veya önizleyebilir. Ayrıca, imza özelleştirme için birçok yetenek sağlanmıştır.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java içinde Image ile Ppsm imzalama adımları"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), Ppsm belgelerini Image imzasıyla hızlı ve kolay bir şekilde imzalama olanağı sağlar.
        
        * Yol veya bellek akışı olarak imzalaması gereken Ppsm dosyasını sağlayan bir Signature sınıfı örneği oluşturun
        * SignOptions sınıfını örnekleyin ve istenen tüm verileri ayarlayın.
        * Çıkış Ppsm dosyasını veya bellek akışını geçen Signature.Sign() yöntemini çağırın

    title_right: " sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for Java, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * En son GroupDocs.Signature for Java ürününü [Maven}](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) adresinden edinin
         
    code: |
        ```java    
                
        // Set up input Ppsm file
        String filePath = "input.ppsm";
        // Set up output file
        String outputFilePath = "output.ppsm";
        // Provide image file
        String imageFilePath = "image.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        ImageSignOptions options = new ImageSignOptions(imageFilePath);

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ppsm document
        SignResult result = signature.sign(outputFilePath, options);
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Ppsm dokümanı Image Canlı Demo ile imzalama"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek çeşitli imzalarla Ppsm dosyasını imzalayın. Ücretsiz çevrimiçi demo sizi bekliyor.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java için desteklenen diğer Image imzaları"
    content: |
        "Ppsm'ı diğer imza türleriyle de imzalayabilirsiniz. Lütfen aşağıdaki listeye bakın."
    format: 
       
       
back_to_top:
    enable: true
---