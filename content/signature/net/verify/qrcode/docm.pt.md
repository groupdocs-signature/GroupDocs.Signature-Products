---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Docm
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Docm for C#

############################# Head ############################
head_title: "Verificação de assinaturas Qrcode para arquivos Docm via C#"
head_description: "Use apenas algumas linhas de código .NET para verificar documentos Docm e suas assinaturas Qrcode."

############################# Header ############################
title: "Qrcode verificação de assinaturas para Docm arquivos"
description: "A API para .NET oferece a oportunidade de verificar assinaturas Qrcode em documentos Docm. A verificação de assinaturas eletrônicas dentro de seus documentos Docm pode ser realizada de forma rápida e fácil."
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
    title: "Descubra os novos recursos da API GroupDocs.Signature for .NET"
    content: |
        A API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferece uma ampla variedade de maneiras de processar vários formatos de documentos usando assinaturas eletrônicas. Muitos tipos de assinaturas digitais como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados são suportados. Os clientes podem adicionar, remover, editar, validar ou pesquisar assinaturas digitais em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Um número surpreendente de recursos e configurações adicionais estão disponíveis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como validar assinaturas Qrcode em seu documento Docm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclui recursos úteis, como verificação de Qrcode assinaturas colocadas em documentos Docm. Use esta oportunidade sem implementar código extra.
        
        * Em primeiro lugar, instanciar a classe Signature fornecendo como um caminho de parâmetro construtor para um documento que deve ser verificado.
        * Em segundo lugar, crie um novo objeto VerifyOptions e configure todas as propriedades necessárias.
        * Por fim, invoque o método Verify do objeto Signature passando a instância VerifyOptions.
        * Em seguida, processe os resultados da verificação.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faça o download da versão mais recente do GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Docm file
        string filePath = "input.docm";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide verification options
                QrCodeVerifyOptions options = new QrCodeVerifyOptions()
                {
                    // process only first page
                    PagesSetup = new PagesSetup() { FirstPage = true },
                    AllPages = false,
                    // set up text match type
                    MatchType = TextMatchType.StartsWith,
                    // specify text pattern to search
                    Text = "QrCode text",
                };

                // Verify document signatures
                VerificationResult result = signature.Verify(options);

                //process result
                if (result.IsValid)
                {
                    //..
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinar com assinaturas Qrcode Demonstração ao vivo"
    content: |
       Adicione várias assinaturas eletrônicas ao arquivo Docm agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifique outras assinaturas Qrcode usando C#"
    content: |
        "Verificação de assinaturas eletrônicas colocadas em vários documentos. Verifique a qualidade das assinaturas nos formatos de arquivo populares, conforme revelado abaixo."
    format: 
       
       
back_to_top:
    enable: true
---