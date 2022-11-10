---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Digital
fileformat: Xltx
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Search Digital signatures at Xltx with C#

############################# Head ############################
head_title: "Procure por assinaturas Digital no arquivo Xltx em C#"
head_description: "Use .NET para pesquisar assinaturas Digital em arquivos Xltx usando algumas linhas de código."

############################# Header ############################
title: "Procure por assinaturas Digital no arquivo Xltx"
description: "A API nativa do .NET permite pesquisar assinaturas Digital em arquivos Xltx já assinados. Realize uma pesquisa avançada de assinatura eletrônica em seus documentos Xltx usando algumas linhas de código."
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
    title_left: "Como pesquisar assinaturas de Digital em Xltx"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) torna mais fácil para os desenvolvedores do .NET pesquisar assinaturas Digital em arquivos Xltx de seus aplicativos implementando algumas etapas fáceis.
        
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
                
        // Set up input Xltx file
        string filePath = "input.xltx";

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

                // search for Digital signatures in Xltx document
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
    title: "Pesquise por Digital assinaturas eletrônicas Demonstração ao vivo"
    content: |
       Pesquise no documento várias assinaturas eletrônicas para arquivos Xltx agora mesmo visitando o site do [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Pesquise outras assinaturas Digital usando C#"
    content: |
        "Pesquisa de assinaturas eletrônicas em vários documentos. Encontre assinaturas de um dos formatos de arquivo populares, conforme mostrado abaixo."
    format: 
           
       
back_to_top:
    enable: true
---