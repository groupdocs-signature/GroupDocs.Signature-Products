---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Otp
productName: Java
lang: tr
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Otp for Java

############################# Head ############################
head_title: "Java içinde Interleaved2of5 Barkodlu eSign Otp belgesi"
head_description: "Interleaved2of5 Barkod İmzası oluşturun ve birkaç satır kod kullanarak Java ile Otp belgesine koyun. Çeşitli dosya biçimlerini imzalamak için GroupDocs Belge İmza API'sini kullanın."

############################# Header ############################
title: "Java içinde Otp belgesi için Interleaved2of5 Barkod imzası oluşturun"
description: "Otp iş belgelerinizi Interleaved2of5 Barkod ile e-imzalayın. İmzalama seçeneklerini ayarlamak için birkaç satır kodla hızlı ve kolay bir şekilde Barkod imzası oluşturun."
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
    title: "GroupDocs.Signature for Java Barkod imzaları API'si hakkında."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN gibi Barkod türlerini kullanarak dijital belge e-imzalamayı yönetmek için hızlı ve kolay bir API'dir. , ITF14 ve diğerleri. Müşteriler kolayca gerekli metni sağlayan Barkodlar oluşturabilir ve bunları PDF, Microsoft Office Words Belgeleri, Microsoft Office Excel çalışma kitapları, MS PowerPoint sunumları, Adobe Photoshop dosyaları ve çeşitli görüntü biçimlerine koyabilir. Belgelere yerleştirilen barkodlar güncellenebilir, aranabilir, doğrulanabilir, silinebilir veya ön izleme yapılabilir. Ayrıca, barkodların özelleştirilmesi desteklenmektedir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java içinde Barcode ile Otp imzalama adımları"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/), Otp belgelerini Barcode imzasıyla hızlı ve kolay bir şekilde imzalama olanağı sağlar.
        
        * Yol veya bellek akışı olarak imzalaması gereken Otp dosyasını sağlayan bir Signature sınıfı örneği oluşturun
        * SignOptions sınıfını örnekleyin ve istenen tüm verileri ayarlayın.
        * Çıkış Otp dosyasını veya bellek akışını geçen Signature.Sign() yöntemini çağırın

    title_right: " sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for Java, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * En son GroupDocs.Signature for Java ürününü [Maven}](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature) adresinden edinin
         
    code: |
        ```java    
                
        // Set up input Otp file
        String filePath = "input.otp";
        // Set up output file
        String outputFilePath = "output.otp";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Otp document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Otp dokümanı Barcode Canlı Demo ile imzalama"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek çeşitli imzalarla Otp dosyasını imzalayın. Ücretsiz çevrimiçi demo sizi bekliyor.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5 (ITF), rakamları kodlayan sürekli iki genişlikli bir barkod sembolojisidir. Ticari olarak 135 film üzerinde, ITF-14 barkodları için ve bazı ürünlerin kartonlarında kullanılırken, içindeki ürünler UPC veya EAN ile etiketlenmiştir.
          characterset: |
             Sayısal rakamlar (0-9).
          textcapacity: |
             Değişken uzunluk.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java için desteklenen diğer Barcode imzaları"
    content: |
        "Otp'ı diğer imza türleriyle de imzalayabilirsiniz. Lütfen aşağıdaki listeye bakın."
    format: 
        
       
back_to_top:
    enable: true
---