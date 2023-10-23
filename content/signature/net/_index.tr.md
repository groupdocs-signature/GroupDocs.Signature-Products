---
############################# Static ############################
layout: "landing"
date: 2023-10-23T14:58:10
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
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Bulut API'leri ve Çevrimiçi Belge İmza Uygulamaları"
head_description: ".NET, Java ve bulut tabanlı uygulamalar için hepsi bir arada belge e-imza çözümü edinin. Basit sürükle ve bırak özelliğini kullanarak yaygın belge biçimlerini çevrimiçi olarak imzalayın"

############################# Header ############################
title: "Belgeleri imzalamak<br>.NET API aracılığıyla"
description: "Programcılar ve son kullanıcılar için esnek API'lerimizi ve uygulama tabanlı çözümlerimizi kullanarak herhangi bir platformda dijital belgeleri ve görüntüleri imzalayın."
words:
  for: "için"

actions:
  main: "Ücretsiz NuGet İndirme"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "Lisanslama"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "başlamaya hazır mısın?"
  description: "GroupDocs.Signature özelliklerini ücretsiz deneyin veya lisans isteyin"

release:
  title: "Sürüm {0} yayınlandı"
  notes: "Yenilikleri görün"
  downloads: "İndirilenler"

code:
  title: "C#'ta PDF dosyalarını imzalayın"
  more: "Daha fazla örnek"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // PDF belgesini seçin
    using (Signature signature = new Signature("sample.pdf"))
    {
        // Metin sağlayın
        var options = new TextSignOptions("John Smith")
        {
            // Rengi ayarla
            ForeColor = Color.Red
        };
        // Belgeyi imzalayın ve dosyaya kaydedin
        signature.Sign("signed.pdf", options);
    }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Signature'a Genel Bakış"
  description: ".NET uygulamalarında belge imzalama ve ilgili işlemleri gerçekleştirmek için API"
  features:
    # feature loop
    - title: "C#'ta iş belgelerine imza ekleme"
      content: "Belge imzalama: GroupDocs.Signature for .NET ile PDF ve Office belgelerine metin, resim, barkod ve dijital sertifika gibi çeşitli imza türlerini ekleyebilirsiniz. Bu API, belgelerinizi gizli meta veriler de dahil olmak üzere neredeyse her türlü veri türüyle imzalamanıza olanak tanır."

    # feature loop
    - title: "İmzalı belgelerin işlenmesi"
      content: "Ek işlemler: GroupDocs.Signature'ı kullanarak imzalı belgeler üzerinde güçlü işlemler gerçekleştirebilirsiniz. Bu, iş belgelerinde mevcut imzaların aranmasını ve bunların belirli ölçütler kullanılarak doğrulanmasını içerir. Ek olarak, bu .NET API aracılığıyla belge bilgilerini alabilir ve sayfaları önizleyebilirsiniz."

    # feature loop
    - title: "Sonuçları özelleştirme"
      content: "GroupDocs.Signature for .NET kapsamlı özelleştirme seçenekleri sunar. İmzaları belge sayfasında herhangi bir yere tam olarak konumlandırabilir ve çeşitli ayarları kullanarak görünümlerini ayarlayabilirsiniz. Ayrıca bu API, işlenmiş belgelerin çok çeşitli desteklenen formatlarda kaydedilmesini destekler."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform bağımsızlığı"
  description: "GroupDocs.Signature for .NET aşağıdaki işletim sistemlerini, çerçeveleri ve paket yöneticilerini destekler"
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
    GroupDocs.Signature for .NET, aşağıdaki [dosya formatlarıyla](https://docs.groupdocs.com/signature/net/supported-document-formats/) yapılan işlemleri destekler.
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
  description: "PDF'leri, Office Belgelerini ve Görüntüleri hızlı ve doğru bir şekilde imzalama"

  items:
    # feature loop
    - icon: "sign"
      title: "Belge imzalama"
      content: "İş belgelerinde belirtilen herhangi bir konuma bir veya daha fazla desteklenen imza türünü doğru bir şekilde ekleyin."

    # feature loop
    - icon: "custom"
      title: "İmzaları özelleştirin"
      content: "İmzaların görünümünü yapılandırmak için renk, yazı tipi, kenarlık, döndürme vb. özelliklerden yararlanın."

    # feature loop
    - icon: "password"
      title: "Belge şifre koruması"
      content: "İmzaladıktan sonra bir parola belirleyerek belirli belge türlerini güvence altına alın."

    # feature loop
    - icon: "protect"
      title: "Değişikliklere karşı koruma"
      content: "Dijital sertifikayla imza ekledikten sonra önemli iş belgelerinde değişiklik yapılmasını önleyin."

    # feature loop
    - icon: "convert"
      title: "İmzalı dosyaları diğer formatlara dönüştürün"
      content: "İmzalı dosyaları, örneğin bir Word belgesini PDF olarak kaydetmek gibi istediğiniz biçimlere dönüştürün."

    # feature loop
    - icon: "preview"
      title: "Sayfa önizlemelerini çıkar"
      content: "İmzalı belgelerdeki sayfaları ileride işlenmek üzere ayrı ayrı görüntüler olarak çıkarın."

    # feature loop
    - icon: "search"
      title: "Belgelerde imza arama"
      content: "Belirli belgelere önceden eklenen imzalar hakkında bilgi alın."

    # feature loop
    - icon: "validate"
      title: "İmzalı belgeleri doğrulayın"
      content: "Doğrulama özelliklerini kullanarak belgelerin doğru şekilde imzalandığını doğrulayın."

    # feature loop
    - icon: "update"
      title: "İmzaları güncelleme veya silme"
      content: "Belirli imzaları bir sayfada kolayca yeniden konumlandırın, metinlerini değiştirin veya herhangi bir sorun yaşamadan silin."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Kod örnekleri"
  description: ".NET işlemleri için tipik GroupDocs.Signature'ın bazı kullanım durumları"
  items:
    # code sample loop
    - title: "PDF'ye QR kodu ekleyin"
      content: |
        PDF belgelerinin belirli sayfalarına [QR kodlarının](https://docs.groupdocs.com/signature/net/esign-document-with-qr-code-signature/) eklenmesi iş süreçlerini iyileştirebilir. Aşağıda GroupDocs.Signature kullanılarak QR kodunun nasıl ekleneceğine ilişkin bir örnek verilmiştir.
        {{< landing/code title="QR kodunu PDF'ye nasıl yerleştiririm?">}}
        ```csharp {style=abap}
        // İmzalanacak belgeyi yükleyin
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Önceden tanımlanmış metinle QR kodu seçenekleri oluşturun
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // QR kodu kodlama türünü ve sayfadaki konumunu yapılandırın
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // Belgeyi imzalayın ve sonuç dosyası olarak kaydedin
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "DOCX belgesini dijital sertifika kullanarak koruma"
      content: |
        Dijital sertifikalar olarak saklanan kişisel veya kurumsal imzaları kullanarak [Bir Belgeyi Koruyabilirsiniz](https://docs.groupdocs.com/signature/net/esign-document-with-digital-signature/). Bu tür korumalı belgeler, imzayı geçersiz kılmadan değiştirilemez.
        {{< landing/code title="Belge bütünlüğünün nasıl sağlanacağı aşağıda açıklanmıştır.">}}
        ```csharp {style=abap}   
        // Dijital olarak imzalanacak belgeyi yükleyin
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // Dijital imzalama seçeneklerini belirtin ve sertifika dosyasının yolunu belirtin
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // Sertifika şifresini ayarlayın
                Password = "1234567890"
            };
            // Belgeyi imzalayın ve istediğiniz yola kaydedin
            signature.Sign("digitally_signed.pdf", options);
        }
        ```
        {{< /landing/code >}}

---
