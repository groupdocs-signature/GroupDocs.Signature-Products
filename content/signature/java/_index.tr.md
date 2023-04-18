---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Dijital İmza API'si, PDF Word Excel Görüntüsüne e-İmza Ekleyin"
head_description: "Java dijital imza API'si. PDF, Microsoft Word, Excel elektronik tabloları, PowerPoint sunumları ve resim belge formatlarını dijital olarak imzalamak için elektronik imza kitaplığı."

############################# Header ############################
title: "Dijital İmzaları Yönetmek için Java API"
description: "Görüntüleri ve Dijital Belge Dosya Biçimlerini İmzalamak için Java Uygulamalarında Görüntü, QR Kodu, Barkod, Meta Veri, Metin ve Damga Türlerinin e-İmzasını yönetin."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "genel bakış"

            # button loop
            - link: "#features"
              text: "Özellikler"

            # button loop
            - link: "#support"
              text: "Destek"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "Canlı Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "Fiyatlandırma"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Signature for Java API, herhangi bir harici yazılım yüklemeden desteklenen biçimlerdeki dijital belgeleri imzalamak için elektronik imza işlevine sahip Java uygulamaları geliştirmenize yardımcı olur. Görüntü, Barkod, QR Kodu, Damga, Metin, Optik ve Meta Veri gibi çeşitli e-İmza türlerinin işlenmesini ve yönetimini destekler. Microsoft Office Word, PowerPoint sunumları, Excel elektronik tabloları, resimler ve PDF dosyaları gibi tüm elektronik iş belgeleriniz, örneğin imza özelliklerini özelleştirerek dijital olarak imzalanabilir. gereksinimlerinize göre gölge, boyutlar, hizalama ve daha fazlası. Yeni veya mevcut bir Java uygulamasına kolayca entegre edilebilen tek bir DLL dosyasından oluşan dijital imza kitaplığı basit ve hafiftir.  

      GroupDocs.Signature for Java API aracılığıyla, tüm kayıtlı sertifikaları sistemden yükleyebilir veya basit ve gelişmiş aramayı kullanarak mevcut imzaları bulabilirsiniz. Parola korumalı belgelerle çalışma seçenekleri, ortak imza özelliklerini belirleme (metin boyutu, opaklık, döndürme, doğrulama, yazı tipi özellikleri, renk seçenekleri, sayfa numarası, genişlik, üst, sol vb.) ve farklı e-İmza türlerini uygulama desteği onu güvenilir kılar. Dijital belgeler için e-İmza yönetimi çözümü.  

      GroupDocs.Signature for Java, tüm Java sürümleriyle uyumludur ve Java çalışma zamanını çalıştırabilen popüler işletim sistemlerini (Windows, Linux, MacOS) destekler.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Bu, Java için GroupDocs.Signature özelliklerine genel bir bakıştır:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "İmza Türleri"
          content: |
            * Metin İmzası
            * Resim İmzası
            * Dijital imzalar
            * QR-Kod İmzası
            * Barkod İmzası
            * Kaşe İmza
            * Form alanı İmzası
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java elektronik olarak imzalama API'si, aşağıda listelendiği gibi [belge dosyası biçimlerini](https://docs.groupdocs.com/signature/java/supported-document-formats/) destekler.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **Görüntüler**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **Meta dosyalar**: EMF, WMF, CMX
                * **Taşınabilir**: PDF
                * **ölçeklendirilebilir Vektör Grafiği**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **Diğerleri**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Signature for Java, aşağıdaki İşletim Sistemlerini, Çerçeveleri ve Paket Yöneticilerini destekler:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "İşletim sistemleri"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Desteklenen Çerçeveler"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Geliştirme Ortamları"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Otomasyon Aracı Oluştur"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Java Özellikleri için GroupDocs.Signature"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Desteklenen Belge Formatlarından e-İmza Oluşturma, Okuma, Değiştirme, Gizleme ve Silme"

      # feature loop
      - icon: "fas fa-eye"
        content: "Akış, Göreli Yol veya Mutlak Yoldan İmzalanacak Belgeye Erişim"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Belgelere, Elektronik Tablolara, Sunumlara, Görüntülere ve PDF Dosyalarına Metin İmzası Uygulayın"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "PDF Dosyalarına Ek Açıklama, Etiket, Görüntü Olarak Metin İmzası Ekleyin, Stili ve Rengi Yapılandırın"

      # feature loop
      - icon: "fas fa-code"
        content: "PDF Belgesini, Görüntü Dosyasını İmzalayın ve Farklı Dosya Formatlarında Çıktı Alın"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Görüntüleri Filigran Olarak Metin İmzasıyla Dijital Olarak İmzalayın ve Saydamlık, Döndürerek eİmzaya Ekleyin"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Sertifikaları Arayın ve Microsoft Word, Excel ve PDF Belgelerini Dijital Sertifikalarla İmzalayın"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Yerel Metin Filigranları ile Kelime İşleme Belge Biçimlerini İmzalayın"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Kelime, Slayt, Hücre, PDF ve Görüntü Dosyalarını İmzalamak için QR Kodu, Barkod Kullanın"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Desteklenen Dosya Biçimlerini Güvenli Hale Getirmek İçin Damga İmzalarını Yapılandırın ve Uygulayın"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Belgelere, Elektronik Tablolara, Sunumlara, Görüntülere ve PDF Dosyalarına Görüntü İmzalarını Kurma ve Atama"

      # feature loop
      - icon: "fas fa-columns"
        content: "İmza Özelliklerini yapılandırın, örn., Bak ve Hisset, Kenar Boşlukları, Hizalama vb."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Parola Korumalı Belgeye Dijital İmza Uygula"

      # feature loop
      - icon: "fas fa-envelope"
        content: "İmza İşleyiciyi Kullanarak PDF Belgelerinin Metin Doğrulamasını Gerçekleştirin"

      # feature loop
      - icon: "fas fa-print"
        content: ".CER ve .PFX Sertifika Kapsayıcıları ile Word, Hücre, PDF Belgelerinin Dijital Olarak Doğrulanması"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "PDF Metin İmzaları için Farklı Ölçü Birimi Türleri (ör. Milimetre, Piksel vb.) Belirtin"

      # feature loop
      - icon: "fas fa-lock"
        content: "Belge Bilgilerini Dosya veya URL Yoluyla Alın - PDF Belgelerine Form Alanı İmzaları Ekleyin"

      # feature loop
      - icon: "fas fa-file-code"
        content: "QR Koduna Özel Veri Nesnesi, Gömülü VCard, E-posta, EPC, MeCard veya Olay Nesnesi Ekleyin"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "İmzalara Farklı Fırça Stilleri Uygulayın, örneğin Degrade, Radyal, Katı ve Doku Fırçası"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "FTP veya Azure Cloud Storage'da Bulunan Belgeyi İmzalayın"

      # feature loop
      - icon: "fas fa-heading"
        content: "Belgeler, Slaytlar, Görüntüler ve PDF Dosyaları için Şekillerde Metin Hizalamasını Ayarlama"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "PowerPoint Sunum Belgelerini Arayın, Doğrulayın ve Dijital Olarak İmzalayın"

      # feature loop
      - icon: "fas fa-cube"
        content: "Hücre Belgelerinde Pikselleri Kullanarak İmza Yerleştirme ve Damga İmzaları için Metin Konumlandırma"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Köşeleri Yuvarlatılmış Dikdörtgen Damga İmzası Uygulayın"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Görsel Veri İçeriği ile Barkod ve QR-Kod İmzalarını Genişletin"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "İmzalama ve Arama Seçenekleriyle Çalışırken Şifreli Meta Veri İmzaları Ekleyin"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Özel Nesneleri Word, Excel ve Sunumlardaki Meta Veri İmzalarına Gömme"

    more_feature:
      # more_feature_loop
      - title: "E-İmzaları Kolayca Yapılandırın ve Uygulayın"
        content: |
          GroupDocs.Signature for Java API, e-İmzaların yapılandırılmasını ve desteklenen belge biçimlerine eklenmesini sağlar. Aşağıda, bir PDF dosyasına metin imzası uygulamanın ne kadar basit olduğunu gösteren bir kod örneği verilmiştir:

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // imza konumunu ayarla
          options.setLeft(100);
          options.setTop(100);
          
          // imza dikdörtgeni ayarla
          options.setWidth(100);
          options.setHeight(30);

          // metin rengini ve Yazı tipini ayarla
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // belgeyi dosyaya imzala
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "e-İmza için Desteklenen Barkod Kodlama Türleri"
        content: |
          GroupDocs.Signature for Java API'yi kullanarak, desteklenen dosya biçimlerine barkod ve QR kodu İmzaları uygulayabilirsiniz. GroupDocs.Signature for Java, çoğu gereksinimi karşılamak için çok çeşitli barkod kodlama türlerini destekler. Desteklenen barkod kodlama türleri arasında Code 11, Code 128, Code 16K/32, Databar kodları, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard ve Code39 Uzatıldı.

          Benzer şekilde GroupDocs.Signature for Java API, QR, Aztec ve Data Matrix gibi QR kodu türlerini kullanmanıza olanak tanır. Desteklenen QR Kodu kodlama türleri arasında Aztec, DataMatrix, GS1 DataMatrix ve GS1 QR yer alır.

      # more_feature_loop
      - title: "İmzaları ve Sertifikaları Ara"
        content: |
          GroupDocs.Signature for Java API aracılığıyla, herhangi bir belgede, sunumda, elektronik tabloda, görselde ve ayrıca PDF dosyasında QR-Code ve Barkod imzalarını arayabilir ve arama sonucunu alabilirsiniz. Ayrıca, QR-Code Signature ile imzalanmış belgelerden özel veri nesnesini ve QR-Code ile İmzalanmış Belgelerden Standart VCard ve E-posta Nesnesini arayabilirsiniz. PDF belgelerinde meta veri imzası aramanın yanı sıra QR-Code imzalarının şifrelenmiş metninin doğrulanması da desteklenir. Words & Cells Belgelerinin dijital imzaları için ek arama kriterleri uygulayın.  

          Word belgeleri, slaytlar ve elektronik tablolar için meta veri imzası için arama seçeneği, PDF belgeleri için form alanı araması da mevcuttur.

      # more_feature_loop
      - title: "e-İmza Özelliklerini Yapılandırma"
        content: |
          Son kullanıcıların UX'ini geliştirmek için GroupDocs.Signature for Java API, kolayca yapılandırılabilen birçok özellik sağlar. Yazı tipi ve renk seçeneklerini (Arka Plan Rengi, Ön Plan Rengi, Kalın, İtalik, Altı Çizili, Yazı Ailesi, Yazı Tipi Boyutu vb.), Arka Plan ve Kenarlık Seçeneklerini (Arka Plan Rengi, Arka Plan Saydamlığı, Kenarlık Rengi, Kenar Çizgi Stili, Kenarlık Kalınlığı, Kenar Saydamlığı vb.), İmza Kenar Boşlukları (Sol, Üst, Genişlik, Yükseklik, Dolgu vb.) ve Kurulum Görüntüsü İmza Alanı ve İmza Hizalaması (Yatay Hizalama, Dikey Hizalama vb.).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature, diğer popüler geliştirme ortamları için belge görüntüleme API'leri sunar"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---