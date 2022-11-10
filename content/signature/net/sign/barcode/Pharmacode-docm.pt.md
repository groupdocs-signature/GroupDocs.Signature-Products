---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Docm
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Docm for C#

############################# Head ############################
head_title: "eSign Docm documento com Pharmacode Código de barras em C#"
head_description: "Crie uma assinatura de código de barras Pharmacode e coloque-a no documento Docm com .NET usando algumas linhas de código. Use a API de assinatura de documento do GroupDocs para assinar vários formatos de arquivo."

############################# Header ############################
title: "Gere assinatura de código de barras Pharmacode para Docm documento em C#"
description: "Assine seus documentos comerciais Docm com o código de barras Pharmacode. Gere assinatura de código de barras de forma rápida e fácil com algumas linhas de código para configurar as opções de assinatura."
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
    title: "Sobre a API de assinaturas de código de barras do GroupDocs.Signature for .NET."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) é uma API rápida e fácil para gerenciar a assinatura eletrônica de documentos digitais usando tipos de código de barras como UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN , ITF14 e muitos outros. Os clientes podem criar facilmente códigos de barras fornecendo o texto necessário e colocá-los em PDF, documentos do Microsoft Office Words, pastas de trabalho do Microsoft Office Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Os códigos de barras colocados em documentos podem ser atualizados, pesquisados, verificados, excluídos ou visualizados. Além disso, a personalização de códigos de barras é suportada.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Docm com Barcode em C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permite assinar documentos Docm com assinaturas Barcode de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Docm para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Docm ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenha o GroupDocs.Signature for .NET mais recente de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
        
        // Set up input Docm file
        string filePath = "input.docm";
        // Set up output file
        string outputFilePath = "output.docm";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Docm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Docm documentos com Barcode Demonstração ao vivo"
    content: |
       Assine o arquivo Docm com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            Pharmacode, também conhecido como Código Binário Farmacêutico, é um padrão de código de barras, usado na indústria farmacêutica como sistema de controle de embalagens.
          characterset: |
             Dígitos numéricos (0-9).
          textcapacity: |
             Representa apenas um único inteiro de 3 a 131070.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Barcode suportadas para C#"
    content: |
        "Você também pode assinar Docm com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
        
       
back_to_top:
    enable: true
---