---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Odt
productName: .NET
lang: tr
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Odt with C#

############################# Head ############################
head_title: "C# içinde Odt dosyasında Digital imzasını arayın"
head_description: "Birkaç satır kod kullanarak Odt dosyalarında Digital imzasını aramak için .NET kullanın."

############################# Header ############################
title: "Odt dosyasında Digital imzasını arayın"
description: ".NET yerel API'si, önceden imzalanmış Odt dosyalarında Digital imzalarının aranmasına olanak tanır. Birkaç satır kod kullanarak Odt belgelerinizde gelişmiş e-imza araması yapın."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API'si hakkında"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), metinler, resimler, dijital sertifikalar, barkodlar, QR kodları, damgalar veya meta veriler gibi çeşitli imza türlerini kullanan belgeleri işlemek için .NET API'si sağlar. Kullanıcılar, imza özelliklerini gerektiği gibi özelleştirmek için ek destekle birlikte PDF'ler, MS Word belgeleri, MS Excel çalışma kitapları, MS PowerPoint sunumları, Adobe Photoshop dosyaları ve çeşitli görüntü biçimleri içindeki elektronik imzaları ekleyebilir, silebilir, güncelleyebilir, doğrulayabilir veya arayabilir.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Odt içinde Digital imzası nasıl aranır?"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/), .NET geliştiricilerinin birkaç kolay adımı uygulayarak Odt dosyalarında Digital imzalarını aramasını kolaylaştırır.
        
        * Signature sınıfının yeni bir örneğini oluşturun ve kaynak belge yolunu yapıcı parametresi olarak iletin.
        * SearchOptions nesnesini gereksinimlerinize göre somutlaştırın ve arama seçeneklerini belirleyin.
        * Signature sınıfı örneğinin Arama yöntemini çağırın ve buna SearchOptions iletin.
        * Arama sonuçlarını taleplerinize göre işleyin.

    title_right: "sistem gereksinimleri"
    content_right: |
        GroupDocs.Signature for .NET, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen aşağıdaki ön koşulların sisteminizde kurulu olduğundan emin olun.

        * İşletim sistemleri: Microsoft Windows, Linux, MacOS
        * Geliştirme ortamları: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * GroupDocs.Signature for .NET ürününün en son sürümünü [Nuget}](https://www.nuget.org/packages/groupdocs.signature) adresinden indirin
         
    code: |
        ```csharp    
                
        // Set up input Odt file
        string filePath = "input.odt";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                DigitalSearchOptions options = new DigitalSearchOptions()
                {
                    // specify special search criteria
                    Comments = "Approved",
                    // specify date range period of signature
                    SignDateTimeFrom = new DateTime(year: 2020, month: 01, day: 01),
                    SignDateTimeTo = new DateTime(year: 2020, month: 12, day: 31)
                };

                // search for Digital signatures in Odt document
                List<DigitalSignature> signatures = signature.Search<DigitalSignature>(options);

                // process signatures which were found                
                foreach (DigitalSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital elektronik imza arayın Canlı Demo"
    content: |
       Şu anda [GroupDocs.Signature App](https://products.groupdocs.app/signature/family) web sitesini ziyaret ederek belgede Odt dosyalarına yönelik çeşitli elektronik imzaları arayın.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "C# kullanarak diğer Digital imzalarını arayın"
    content: |
        "Elektronik imzalar çeşitli belgelerde arama yapar. Aşağıda gösterildiği gibi popüler dosya biçimlerinden birindeki imzaları bulun."
    format: 
           
       
back_to_top:
    enable: true
---