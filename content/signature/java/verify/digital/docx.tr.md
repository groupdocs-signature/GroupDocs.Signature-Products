---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Docx
productName: Java
lang: tr
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Docx for Java

############################# Head ############################
head_title: "Docx dosyaları için Digital imzalarının Java aracılığıyla doğrulanması"
head_description: "Docx belgelerini ve bunların Digital imzalarını doğrulamak için yalnızca birkaç satır Java kodu kullanın."

############################# Header ############################
title: "Docx dosyaları için Digital imza doğrulaması"
description: "Java için API, Docx belgelerinde Digital imzalarını doğrulama fırsatı sunar. Docx belgelerinizdeki e-imzaların doğrulanması hızlı ve kolay bir şekilde gerçekleştirilebilir."
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
    title: "Yeni GroupDocs.Signature for Java API özelliklerini keşfedin"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API, elektronik imzalar kullanarak çok sayıda belge biçimini işlemek için çok çeşitli yollar sunar. Metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi birçok dijital imza türü desteklenir. Müşteriler, PDF'lerde, MS Word belgelerinde, MS Excel çalışma kitaplarında, MS PowerPoint sunumlarında, Adobe Photoshop dosyalarında ve çeşitli görüntü formatlarında dijital imza ekleyebilir, kaldırabilir, düzenleyebilir, doğrulayabilir veya arayabilir. Şaşırtıcı sayıda ek özellik ve ayar mevcuttur.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Docx belgenizdeki Digital imzalarını nasıl doğrularsınız?"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), Docx belgelerine yerleştirilen Digital imzalarının doğrulanması gibi faydalı özellikler içerir. Ekstra kod uygulamadan bu fırsatı kullanın.
        
        * İlk olarak, doğrulanması gereken bir belgeye yapıcı parametre yolu sağlayan Signature sınıfını örnekleyin.
        * İkinci olarak, yeni bir VerifyOptions nesnesi oluşturun ve gerekli tüm özellikleri ayarlayın.
        * Son olarak, VerifyOptions örneğini geçen Signature'ın nesne Verify yöntemini çağırın.
        * Ardından doğrulama sonuçlarını işleyin.

    title_right: "sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for Java, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * GroupDocs.Signature for Java ürününün en son sürümünü [Maven}](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) adresinden indirin
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
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
    title: "Digital imzalarıyla imzalama Canlı Demo"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek Docx dosyasına çeşitli elektronik imzalar ekleyin.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java kullanarak diğer Digital imzalarını doğrulayın"
    content: |
        "Çeşitli belgelere yerleştirilen elektronik imzaların doğrulanması. Aşağıda açıklandığı gibi popüler dosya formatlarındaki imzaların kalitesini kontrol edin."
    format: 
       
       
back_to_top:
    enable: true
---