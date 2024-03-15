---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: tr
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Dijital İmza API'si - GroupDocs.Signature"
head_description: "Node.js uygulamalarına güvenli e-imzaları GroupDocs.Signature ile entegre edin. Belge imzalama iş akışlarını kolay ve verimli bir şekilde kolaylaştırın."

############################# Header ############################
title: "Belgeleri imzalamak<br>Node.js API'si ile"
description: "Programcılar ve son kullanıcılar için esnek API'lerimizi ve uygulama tabanlı çözümlerimizi kullanarak herhangi bir platformda dijital belgeleri ve görüntüleri imzalayın."
words:
  for: "için"

actions:
  main: "NPM'den indirin"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Lisanslama"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "başlamaya hazır mısın?"
  description: "GroupDocs.Signature özelliklerini ücretsiz deneyin veya lisans isteyin"

release:
  title: "Sürüm {0} yayınlandı"
  notes: "Yenilikleri görün"
  downloads: "İndirilenler"

code:
  title: "PDF'leri Node.js ile imzalama"
  more: "Daha fazla örnek"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // PDF belgesini seçin
    let signature = new Signature("sample.pdf");
    
    // Metin sağlayın
    let options = new TextSignOptions("John Smith");
    
    // Rengi ayarla
    options.ForeColor = Color.Red;
    
    // Belgeyi imzalayın ve dosyaya kaydedin
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature'a Genel Bakış"
  description: "Node.js uygulamalarında kullanıma hazır belge imzalama kitaplığı"
  features:
    # feature loop
    - title: "Node.js ile İş Belgeleri için Dijital İmza Çözümü"
      content: "GroupDocs.Signature for Node.js via Java, PDF, Office belgeleri ve görselleri için kapsamlı bir dizi dijital imza seçeneği sunar. Metin, barkodlar, resimler, dijital sertifikalar ve meta veriler mevcuttur. Kolaylaştırılmış belge işleme verimliliği sağlar."

    # feature loop
    - title: "İmzalı Belgelerin Gelişmiş Düzenlemesi"
      content: "GroupDocs.Signature imzalı belgeleri işlemenize olanak sağlar. Çeşitli kriterleri kullanarak imzaları arayın ve doğrulayın. Ayrıca ayrıntılı belge bilgilerini çıkarın veya sayfaların önizleme görüntülerini oluşturun."

    # feature loop
    - title: "Çeşitli Çıktı Formatları"
      content: "Çözümümüz imzalı belgelerin çıktı formatı üzerinde kapsamlı kontrol sağlar. İmzaları herhangi bir sayfaya tam olarak konumlandırın ve görünümlerini özelleştirin. İmzalı belgeleri desteklenen çok sayıda formatta kaydedin ve isteğe bağlı olarak bunları parolalarla koruyun."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform bağımsızlığı"
  description: "GroupDocs.Signature for Node.js via Java, çeşitli işletim sistemleriyle belge işleme gerçekleştirir"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Desteklenen dosya formatları"
  description: |
    GroupDocs.Signature for Node.js via Java, [popüler dosya biçimleri](https://docs.groupdocs.com/signature/java/supported-document-formats/) için işlemleri kolaylaştırır.
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
  title: "GroupDocs.Signature Özellikleri"
  description: "PDF'leri, Office belgelerini ve görüntüleri dijital imzalarla imzalayın"

  items:
    # feature loop
    - icon: "sign"
      title: "İşletme İmzaları"
      content: "Belgeleri imzalamak için çeşitli imza türlerini kullanın. Dijital imzaları herhangi bir sayfa konumuna tam olarak yerleştirin."

    # feature loop
    - icon: "custom"
      title: "İmza Görünümünü Özelleştirme"
      content: "İstediğiniz sonuca ulaşmak için rengi, yazı tipini, kenarlıkları, döndürmeyi ve daha fazlasını ayarlayarak imzaların görsel yönlerini uyarlayın."

    # feature loop
    - icon: "password"
      title: "Parola Korumalı Belgeler"
      content: "Desteklenen birçok belge biçiminde, ek güvenlik için imzalı belgeleri bir parolayla koruyun."

    # feature loop
    - icon: "protect"
      title: "Yetkisiz Değişikliklerin Önlenmesi"
      content: "Dijital sertifikalarla imzalanmış önemli iş belgelerini yetkisiz değişikliklere karşı koruyun."

    # feature loop
    - icon: "convert"
      title: "İstenilen Çıkış Formatları"
      content: "Desteklenen herhangi bir formatta imzalanmış belgeleri zahmetsizce alın. MS Word belgelerini kolaylıkla PDF formatına dönüştürün."

    # feature loop
    - icon: "preview"
      title: "Belgeleri Önizleme"
      content: "Gelecekteki ihtiyaçlar için ayrı ayrı belge sayfalarını resim olarak kaydedin."

    # feature loop
    - icon: "search"
      title: "İmza Arama"
      content: "Belgelerinize önceden eklenen imzalar hakkında bilgi alın."

    # feature loop
    - icon: "validate"
      title: "Belge Doğrulaması"
      content: "Herhangi bir belgede sunulan imzaların gerçekliğini doğrulayın."

    # feature loop
    - icon: "update"
      title: "İmza Yönetimi"
      content: "Herhangi bir belge sayfasına yerleştirilen imzaları silin, yerini değiştirin veya değiştirin."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kod örnekleri"
  description: "Tipik GroupDocs.Signature for Node.js via Java işlemlerini gösteren açıklayıcı örnekler"
  items:
    # code sample loop
    - title: "PDF'yi QR Kodlarıyla İşaretleyin"
      content: |
        [Barkodları](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) belirli PDF belge sayfalarına eklemek iş süreçlerini kolaylaştırabilir. Bu bölümde, GroupDocs.Signature for Node.js via Java kullanarak QR kodu eklemeye ilişkin bir örnek verilmektedir.
        {{< landing/code title="QR kodunu PDF'ye nasıl yerleştiririm?">}}
        ```javascript {style=abap}
        // İmzalanacak belgeyi yükleyin
        let signature = new Signature("file_to_sign.pdf");
        
        // Önceden tanımlanmış metinle QR kodu seçenekleri oluşturun
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // QR kodu kodlama türünü ve sayfadaki konumunu yapılandırın
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Belgeyi imzalayın ve sonuç dosyası olarak kaydedin
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX'i Dijital İmzayla Koruma"
      content: |
        [Belgelerinizi koruyun](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) dijital sertifikalara dayalı imzalarla. Dijital imza, iş belgelerinizi içerik değişikliklerine karşı korur.
        {{< landing/code title="Belge bütünlüğünün nasıl sağlanacağı aşağıda açıklanmıştır.">}}
        ```javascript {style=abap}   
        // Dijital olarak imzalanacak belgeyi yükleyin
        let signature = new Signature("file_to_sign.docx");
        
        // Dijital imzalama seçeneklerini belirtin ve sertifika dosyasının yolunu belirtin
        let options = new DigitalSignOptions("certificate.pfx");

        // Sertifika şifresini ayarlayın
        options.Password = "1234567890";

        // Belgeyi imzalayın ve istediğiniz yola kaydedin
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
