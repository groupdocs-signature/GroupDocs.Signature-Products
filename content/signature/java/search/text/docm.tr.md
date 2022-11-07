---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Text
fileformat: Docm
productName: Java
lang: tr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Search Text signatures at Docm with Java

############################# Head ############################
head_title: "Java içinde Docm dosyasında Text imzasını arayın"
head_description: "Birkaç satır kod kullanarak Docm dosyalarında Text imzasını aramak için Java kullanın."

############################# Header ############################
title: "Docm dosyasında Text imzasını arayın"
description: "Java yerel API'si, önceden imzalanmış Docm dosyalarında Text imzalarının aranmasına olanak tanır. Birkaç satır kod kullanarak Docm belgelerinizde gelişmiş e-imza araması yapın."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API'si hakkında"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi çeşitli imza türlerini kullanan belgeleri işlemek için Java API'si sağlar. Kullanıcılar, imza özelliklerini gerektiği gibi özelleştirmek için ek destekle birlikte PDF'ler, MS Word belgeleri, MS Excel çalışma kitapları, MS PowerPoint sunumları, Adobe Photoshop dosyaları ve çeşitli görüntü biçimleri içindeki elektronik imzaları ekleyebilir, silebilir, güncelleyebilir, doğrulayabilir veya arayabilir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Docm içinde Text imzası nasıl aranır?"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), Java geliştiricilerinin birkaç kolay adımı uygulayarak Docm dosyalarında Text imzalarını aramasını kolaylaştırır.
        
        * Signature sınıfının yeni bir örneğini oluşturun ve kaynak belge yolunu yapıcı parametresi olarak iletin.
        * SearchOptions nesnesini gereksinimlerinize göre somutlaştırın ve arama seçeneklerini belirleyin.
        * Signature sınıfı örneğinin Arama yöntemini çağırın ve buna SearchOptions iletin.
        * Arama sonuçlarını taleplerinize göre işleyin.

    title_right: "sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for Java, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * GroupDocs.Signature for Java ürününün en son sürümünü [Maven}](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) adresinden indirin
         
    code: |
        ```java    
                
        // Set up input Docm file
        String filePath = "input.docm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        TextSearchOptions options = new TextSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
                            
        // search for Text signatures in Docm document
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Text elektronik imza arayın Canlı Demo"
    content: |
       Şu anda [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek belgede Docm dosyalarına yönelik çeşitli elektronik imzaları arayın.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java kullanarak diğer Text imzalarını arayın"
    content: |
        "Elektronik imzalar çeşitli belgelerde arama yapar. Aşağıda gösterildiği gibi popüler dosya biçimlerinden birindeki imzaları bulun."
    format: 
           
       
back_to_top:
    enable: true
---