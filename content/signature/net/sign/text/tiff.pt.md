---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Tiff
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Tiff for C#

############################# Head ############################
head_title: "Crie assinaturas eletrônicas de texto para o arquivo Tiff com C#"
head_description: "Coloque Text eSignature no arquivo Tiff para .NET usando algumas linhas de código. Use a API de assinatura de documentos do GroupDocs para assinar dezenas de formatos de arquivo."

############################# Header ############################
title: "Assine Tiff arquivos com assinaturas Text em C#"
description: "Como adicionar assinatura Text com algumas linhas de código .NET"
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
    title: "Sobre a API GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) é uma API popular para assinatura eletrônica de documentos digitais. Assinaturas como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados estão disponíveis. Assinaturas podem ser colocadas em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Os clientes podem assinar seu documento e atualizar, pesquisar, verificar, excluir ou visualizar assinaturas eletrônicas que foram colocadas nesses documentos. Além disso, são fornecidas muitas habilidades para personalização de assinaturas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Tiff com Text em C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permite assinar documentos Tiff com assinaturas Text de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Tiff para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Tiff ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenha o GroupDocs.Signature for .NET mais recente de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Tiff file
        string filePath = "input.tiff";
        // Set up output file
        string outputFilePath = "output.tiff";

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

                // sign Tiff document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Tiff documentos com Text Demonstração ao vivo"
    content: |
       Assine o arquivo Tiff com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Text suportadas para C#"
    content: |
        "Você também pode assinar Tiff com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
       
       
back_to_top:
    enable: true
---