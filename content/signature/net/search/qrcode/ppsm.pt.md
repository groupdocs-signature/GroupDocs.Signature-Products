---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Ppsm
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Ppsm with C#

############################# Head ############################
head_title: "Procure por assinaturas Qrcode no arquivo Ppsm em C#"
head_description: "Use .NET para pesquisar assinaturas Qrcode em arquivos Ppsm usando algumas linhas de código."

############################# Header ############################
title: "Procure por assinaturas Qrcode no arquivo Ppsm"
description: "A API nativa do .NET permite pesquisar assinaturas Qrcode em arquivos Ppsm já assinados. Realize uma pesquisa avançada de assinatura eletrônica em seus documentos Ppsm usando algumas linhas de código."
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
    title: "Sobre a API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fornece a API .NET para processar documentos usando vários tipos de assinatura, como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados. Os usuários podem adicionar, excluir, atualizar, verificar ou pesquisar assinaturas eletrônicas em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem, com suporte adicional para personalizar as propriedades das assinaturas conforme necessário.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como pesquisar assinaturas de Qrcode em Ppsm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) torna mais fácil para os desenvolvedores do .NET pesquisar assinaturas Qrcode em arquivos Ppsm de seus aplicativos implementando algumas etapas fáceis.
        
        * Crie uma nova instância da classe Signature e passe o caminho do documento de origem como um parâmetro de construtor.
        * Instancie o objeto SearchOptions de acordo com seus requisitos e especifique as opções de pesquisa.
        * Chame o método Search da instância da classe Signature e passe SearchOptions para ele.
        * Processe os resultados da pesquisa de acordo com suas demandas.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faça o download da versão mais recente do GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Ppsm file
        string filePath = "input.ppsm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Create search options
                QrCodeSearchOptions options = new QrCodeSearchOptions()
                {
                    // specify special pages to search on 
                    AllPages = false,
                    // single page number
                    PageNumber = 1,
                    // set up text match type
                    MatchType = TextMatchType.Contains,
                    // specify text pattern to search
                    Text = "Text signature",
                    // return  Qrcode images for processing
                    ReturnContent = true,
                    // set up type of returned  Qrcode images
                    ReturnContentType = FileType.PNG
                };

                // search for Qrcode signatures in Ppsm document
                List<QrCodeSignature> signatures = signature.Search<QrCodeSignature>(options);

                // process signatures which were found                
                foreach (QrCodeSignature item in signatures)
                {
                    //...
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Pesquise por Qrcode assinaturas eletrônicas Demonstração ao vivo"
    content: |
       Pesquise no documento várias assinaturas eletrônicas para arquivos Ppsm agora mesmo visitando o site do [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Pesquise outras assinaturas Qrcode usando C#"
    content: |
        "Pesquisa de assinaturas eletrônicas em vários documentos. Encontre assinaturas de um dos formatos de arquivo populares, conforme mostrado abaixo."
    format: 
           
       
back_to_top:
    enable: true
---