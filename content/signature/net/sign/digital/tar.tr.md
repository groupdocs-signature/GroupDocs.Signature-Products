---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Tar
productName: .NET
lang: tr
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Tar for C#

############################# Head ############################
head_title: "C# ile Tar dosyasına Dijital elektronik imza ekleme"
head_description: "Birkaç satır kod kullanarak Dijital İmzayı .NET için Tar dosyasına koyun. Düzinelerce dosya biçimini imzalamak için GroupDocs Belge İmza API'sini kullanın."

############################# Header ############################
title: "C# içinde Digital imzalı Tar dosyalarını imzalayın"
description: "Birkaç satır .NET koduyla Digital imzası nasıl eklenir"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET Dijital imza API'sı hakkında"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), belgeleri dijital sertifikalarla dijital elektronik imzalarla tasarlamak için popüler bir API'dir. Dijital imzalar için API, belgeyi parola korumalı özel ve genel anahtarlarla esign etmek için PFX sertifika dosyalarını kullanır. Dijital imzalar, belirli bir eSign PDF sayfasıyla iş belgelerini onaylamak, Words, Excel, Powerpoint dosyaları ve Open Office belgeleri gibi tüm Microsoft Office belgelerini onaylamak için kullanılabilir. Müşteriler, düzenleme, kaldırma veya ayarlama gibi imzaları kolayca değiştirebilir. API, imzaları aramak ve doğrulamak için bir yol sağlar. Ayrıca, imza özelleştirme için birçok yetenek sağlanmıştır.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# içinde Digital ile Tar imzalama adımları"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), Tar belgelerini Digital imzasıyla hızlı ve kolay bir şekilde imzalama olanağı sağlar.
        
        * Yol veya bellek akışı olarak imzalaması gereken Tar dosyasını sağlayan bir Signature sınıfı örneği oluşturun
        * SignOptions sınıfını örnekleyin ve istenen tüm verileri ayarlayın.
        * Çıkış Tar dosyasını veya bellek akışını geçen Signature.Sign() yöntemini çağırın

    title_right: " sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for .NET, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * En son GroupDocs.Signature for .NET ürününü [Nuget}](https://www.nuget.org/packages/groupdocs.signature) adresinden edinin
         
    code: |
        ```csharp    
                
        // Set up input Tar file
        string filePath = "input.tar";
        // Set up output file
        string outputFilePath = "output.tar";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Tar document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Tar dokümanı Digital Canlı Demo ile imzalama"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek çeşitli imzalarla Tar dosyasını imzalayın. Ücretsiz çevrimiçi demo sizi bekliyor.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# için desteklenen diğer Digital imzaları"
    content: |
        "Tar'ı diğer imza türleriyle de imzalayabilirsiniz. Lütfen aşağıdaki listeye bakın."
    format: 
       
       
back_to_top:
    enable: true
---