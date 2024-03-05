---
############################# Static ############################
layout: "landing"
date: 2024-03-05T08:14:01
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: tr
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, Bulut API'leri ve Çevrimiçi Belge İmza Uygulamaları"
head_description: ".NET, Java ve bulut tabanlı uygulamalar için hepsi bir arada belge e-imza çözümü edinin. Basit sürükle ve bırak özelliğini kullanarak yaygın belge biçimlerini çevrimiçi olarak imzalayın"

############################# Header ############################
title: "Belgeleri imzalamak<br>Java API'si aracılığıyla"
description: "Programcılar ve son kullanıcılar için esnek API'lerimizi ve uygulama tabanlı çözümlerimizi kullanarak herhangi bir platformda dijital belgeleri ve görüntüleri imzalayın."
words:
  for: "için"

actions:
  main: "Ücretsiz Maven İndir"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Lisanslama"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "başlamaya hazır mısın?"
  description: "GroupDocs.Signature özelliklerini ücretsiz deneyin veya lisans isteyin"

release:
  title: "Sürüm {0} yayınlandı"
  notes: "Yenilikleri görün"
  downloads: "İndirilenler"

code:
  title: "PDF dosyalarını Java'da imzalayın"
  more: "Daha fazla örnek"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // PDF belgesini seçin
    Signature signature = new Signature("sample.pdf");
    
    // Metin sağlayın
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Belgeyi imzalayın ve dosyaya kaydedin
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature'a Genel Bakış"
  description: "Java uygulamalarında belge imzalama ve ilgili işlemleri gerçekleştirmek için API"
  features:
    # feature loop
    - title: "Java'da dijital imzalarla geliştirilmiş iş belgeleri"
      content: "Hızlı ve özelleştirilebilir imzalama: GroupDocs.Signature for Java, PDF'ler, resimler ve Office belgeleri için çok çeşitli dijital imza seçenekleri sunar. Metin, barkod, QR kodları, dijital sertifikalar, resimler veya gizli meta verileri kullanabilirsiniz. Belge işleme hızlı ve etkilidir."

    # feature loop
    - title: "İmzalı belgeleri işleme"
      content: "Gelişmiş belge işleme, GroupDocs.Signature for Java kullanılarak imzalanmış belgeler üzerinde güçlü işlemler içerir. Çeşitli faydalı kriterleri kullanarak iş belgelerine eklenen imzaları arayabilir ve doğrulayabilirsiniz. Ayrıca belge hakkında detaylı bilgilere ulaşabilir veya sayfalarının ön izleme görsellerini alabilirsiniz."

    # feature loop
    - title: "Çeşitli çıktı seçenekleri"
      content: "Güçlü imzalama seçenekleri, GroupDocs.Signature for Java ile imzalanan belgelerin çıktısını özelleştirmenize olanak tanır. Herhangi bir imzayı herhangi bir belge sayfasında tam olarak konumlandırabilir ve görünümünü çeşitli şekillerde yapılandırabilirsiniz. Java API, imzalanmış iş belgelerinin çok sayıda desteklenen formatta kaydedilmesini destekler ve bunların parolalarla güvenliğinin sağlanmasına yönelik seçenekler sunar."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform bağımsızlığı"
  description: "GroupDocs.Signature for Java aşağıdaki işletim sistemlerini, çerçeveleri ve paket yöneticilerini destekler"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Desteklenen dosya formatları"
  description: |
    GroupDocs.Signature for Java, aşağıdaki [dosya formatlarıyla](https://docs.groupdocs.com/signature/java/supported-document-formats/) yapılan işlemleri destekler.
  groups:
    # group loop
    - color: "green"
      content: |
        ### Microsoft Office formatları
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Görseller ve Diğer Formatlar
        * **Taşınabilir:** PDF
        * **Görüntüler:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Diğer ofis formatları:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Diğer formatlar
        * **ağ:** HTML, MHTML
        * **Arşivler:** ZIP, TAR, 7Z
        * **Sertifikalar:** PFX

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Signature özellikleri"
  description: "PDF'leri, Office Belgelerini ve görüntüleri dijital imzalarla imzalama"

  items:
    # feature loop
    - icon: "sign"
      title: "İmza Ekleme"
      content: "Dijital imzayı herhangi bir sayfada herhangi bir konuma tam olarak yerleştirerek, desteklenen çeşitli imza türlerini kullanarak bir belgeyi imzalayın."

    # feature loop
    - icon: "custom"
      title: "Sonuçları özelleştirme"
      content: "İstenilen sonucu elde etmek için rengi, yazı tipini, kenarlığı, döndürmeyi ve diğer özellikleri ayarlayarak imza görünümünü özelleştirin."

    # feature loop
    - icon: "password"
      title: "Belgeleri şifreyle koruma"
      content: "Desteklenen birçok belge türü için imzalı belgeyi bir parolayla koruyabilirsiniz."

    # feature loop
    - icon: "protect"
      title: "Yetkisiz değişikliklerin önlenmesi"
      content: "Dijital sertifikayla imzalanmış önemli iş belgelerini yetkisiz değişikliklere karşı koruyun."

    # feature loop
    - icon: "convert"
      title: "İstenilen formatlarda sonuçların elde edilmesi"
      content: "Desteklenen herhangi bir formattaki imzalı sonuç dosyalarını kolayca edinin. Ayrıca MS Word belgelerini zahmetsizce PDF'ye dönüştürebilirsiniz."

    # feature loop
    - icon: "preview"
      title: "Belge önizlemesi"
      content: "Gelecekteki işlemler için belgenin herhangi bir sayfasını görüntü olarak kaydedin."

    # feature loop
    - icon: "search"
      title: "İmza aranıyor"
      content: "Belirli belgelerde daha önce eklenen imzalar hakkında bilgi almak mümkündür."

    # feature loop
    - icon: "validate"
      title: "Belgeleri doğrulama"
      content: "İmzalı herhangi bir belgedeki imzaların doğruluğunu doğrulayın."

    # feature loop
    - icon: "update"
      title: "İmzaları yönetme"
      content: "İmza bir belge sayfasına yerleştirildikten sonra gerektiğinde silinebilir, taşınabilir veya güncellenebilir."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kod örnekleri"
  description: "Java işlemleri için tipik GroupDocs.Signature'ın bazı kullanım durumları"
  items:
    # code sample loop
    - title: "PDF belgesini QR koduyla zenginleştirin"
      content: |
        PDF belgelerinin belirli sayfalarına [QR kodları](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) ekleyerek iş süreçlerini geliştirmek değerli olabilir. GroupDocs.Signature for Java kullanılarak QR kodunun nasıl ekleneceğine dair bir örnek bulunmaktadır.
        {{< landing/code title="PDF belgesini QR koduyla zenginleştirin">}}
        ```java {style=abap}
        // İmzalanacak belgeyi yükleyin
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Önceden tanımlanmış metinle QR kodu seçenekleri oluşturun
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR kodu kodlama türünü ve sayfadaki konumunu yapılandırın
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Belgeyi imzalayın ve sonuç dosyası olarak kaydedin
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX'i korumak için dijital imza kullanma"
      content: |
        Dijital sertifikalar olarak saklanan kişisel veya kurumsal imzaları kullanarak [Bir Belgeyi Koruyun](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) yapabilirsiniz. Sertifika ile güvence altına alınan belgelerde imza geçersiz kılınmadan değişiklik yapılamaz.
        {{< landing/code title="DOCX'i korumak için dijital imza kullanma">}}
        ```java {style=abap}   
        // Dijital olarak imzalanacak belgeyi yükleyin
        Signature signature = new Signature("file_to_sign.docx");
        
        // Dijital imzalama seçeneklerini belirtin ve sertifika dosyasının yolunu belirtin
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Sertifika şifresini ayarlayın
        options.setPassword("1234567890");

        // Belgeyi imzalayın ve istediğiniz yola kaydedin
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
