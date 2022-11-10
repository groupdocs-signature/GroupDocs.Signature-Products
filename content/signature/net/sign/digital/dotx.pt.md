---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Dotx
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dotx for C#

############################# Head ############################
head_title: "Adicionando assinaturas eletrônicas digitais ao arquivo Dotx com C#"
head_description: "Coloque a assinatura digital no arquivo Dotx para .NET usando algumas linhas de código. Use a API de assinatura de documentos do GroupDocs para assinar dezenas de formatos de arquivo."

############################# Header ############################
title: "eSign Dotx arquivos com assinaturas Digital em C#"
description: "Como adicionar a assinatura Digital com algumas linhas de código .NET"
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
    title: "Sobre a API de assinaturas digitais do GroupDocs.Signature for .NET"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) é uma API popular para assinar documentos com assinaturas eletrônicas digitais, com certificados digitais. Para a API de assinaturas digitais, usa arquivos de certificado PFX para assinar documentos com chaves privadas e públicas protegidas por senha. As assinaturas digitais podem ser usadas para certificar documentos comerciais com uma página específica do eSign PDF, certificar documentos inteiros do Microsoft Office, como Word, Excel, arquivos do Powerpoint e documentos do Open Office. Os clientes podem manipular facilmente as assinaturas, como editá-las, removê-las ou ajustá-las. A API fornece uma maneira de pesquisar e verificar assinaturas. Além disso, são fornecidas muitas habilidades para personalização de assinaturas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Dotx com Digital em C#"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) permite assinar documentos Dotx com assinaturas Digital de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Dotx para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Dotx ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Obtenha o GroupDocs.Signature for .NET mais recente de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Dotx file
        string filePath = "input.dotx";
        // Set up output file
        string outputFilePath = "output.dotx";
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

                // sign Dotx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Dotx documentos com Digital Demonstração ao vivo"
    content: |
       Assine o arquivo Dotx com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Digital suportadas para C#"
    content: |
        "Você também pode assinar Dotx com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
       
       
back_to_top:
    enable: true
---