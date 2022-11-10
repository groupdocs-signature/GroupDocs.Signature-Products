---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Doc
productName: .NET
lang: tr
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Doc for C#

############################# Head ############################
head_title: "C# ile Doc dosyasına Metin elektronik imzaları oluşturun"
head_description: "Birkaç satır kod kullanarak .NET için Doc dosyasına Text eSignature koyun. Düzinelerce dosya biçimini imzalamak için GroupDocs Belge İmza API'sini kullanın."

############################# Header ############################
title: "Doc dosyalarını Text imzasıyla C# içinde imzalayın"
description: "Birkaç satır .NET koduyla Text İmzası nasıl eklenir"
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
    title: "GroupDocs.Signature for .NET API'si hakkında"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), dijital belge e-imzalama için popüler bir API'dir. Metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi imzalar mevcuttur. İmzalar PDF'lere, MS Word belgelerine, MS Excel çalışma kitaplarına, MS PowerPoint sunumlarına, Adobe Photoshop dosyalarına ve çeşitli görüntü biçimlerine yerleştirilebilir. Müşteriler, belgelerini imzalayabilir ve bu belgelere konan e-imzaları güncelleyebilir, arayabilir, doğrulayabilir, silebilir veya önizleyebilir. Ayrıca, imza özelleştirme için birçok yetenek sağlanmıştır.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C# içinde Text ile Doc imzalama adımları"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), Doc belgelerini Text imzasıyla hızlı ve kolay bir şekilde imzalama olanağı sağlar.
        
        * Yol veya bellek akışı olarak imzalaması gereken Doc dosyasını sağlayan bir Signature sınıfı örneği oluşturun
        * SignOptions sınıfını örnekleyin ve istenen tüm verileri ayarlayın.
        * Çıkış Doc dosyasını veya bellek akışını geçen Signature.Sign() yöntemini çağırın

    title_right: " sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for .NET, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * En son GroupDocs.Signature for .NET ürününü [Nuget}](https://www.nuget.org/packages/groupdocs.signature) adresinden edinin
         
    code: |
        ```csharp    
                
        // Set up input Doc file
        string filePath = "input.doc";
        // Set up output file
        string outputFilePath = "output.doc";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                TextSignOptions options = new TextSignOptions("John Smith")
                {
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Doc document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Doc dokümanı Text Canlı Demo ile imzalama"
    content: |
       Hemen şimdi [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek çeşitli imzalarla Doc dosyasını imzalayın. Ücretsiz çevrimiçi demo sizi bekliyor.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C# için desteklenen diğer Text imzaları"
    content: |
        "Doc'ı diğer imza türleriyle de imzalayabilirsiniz. Lütfen aşağıdaki listeye bakın."
    format: 
       
       
back_to_top:
    enable: true
---