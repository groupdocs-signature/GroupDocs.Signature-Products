---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Pdf
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Pdf for C#

############################# Head ############################
head_title: "Atualize assinaturas Text colocadas em arquivos Pdf com C#"
head_description: "Use o código .NET simples e fácil para atualização de assinaturas Text em documentos Pdf assinados."

############################# Header ############################
title: "Edite e atualize assinaturas Text colocadas em arquivos Pdf"
description: "A API para .NET fornece funcionalidade para atualização de assinaturas Text em documentos Pdf. Atualize assinaturas eletrônicas dentro de seus documentos Pdf com algumas linhas de código C# de forma rápida e fácil."
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
    title: "Saiba mais sobre os recursos da API GroupDocs.Signature for .NET"
    content: |
        A funcionalidade da API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) contém uma vasta seleção de meios para processar em formatos de documentos sob demanda usando assinaturas eletrônicas. Amplo espectro de assinaturas eletrônicas, como textos, imagens, certificados digitais, códigos de barras, códigos QR, selos ou metadados são suportados. Os clientes podem adicionar, remover, editar, validar ou pesquisar assinaturas digitais em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Vários recursos e configurações úteis estão disponíveis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como alterar assinaturas Text em seu documento Pdf"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) inclui recursos úteis como atualização de Text assinaturas colocadas em documentos Pdf. Possibilita alterar recursos de assinaturas sem código extra.
        
        * Para começar, crie o objeto Signature passando como um caminho de parâmetro construtor para um documento que deve ser atualizado.
        * Em seguida, instancie um objeto de assinatura específico apropriado e configure seu identificador e propriedades que precisam ser alteradas.
        * Por último, chame o método Update do Signature passando um objeto de assinatura específico.
        * Processe a atualização dos resultados ao seu aviso.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for .NET são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * Faça o download da versão mais recente do GroupDocs.Signature for .NET de [Nuget](https://www.nuget.org/packages/groupdocs.signature)
         
    code: |
        ```csharp    
                
        // Set up input Pdf file
        string filePath = "input.pdf";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // Id of signature which is supposed to be updated
                // such Id might be got as a result of search operation
                string id = "ff988ab1-7403-4c8d-8db7-f2a56b9f8530";

                // provide signature features to update
                // set up particular signature id
                TextSignature signatureToUpdate = new TextSignature(id)
                {
                    // specify signature width
                    Width = 130,
                    // specify signature height
                    Height = 20,
                    // set left position
                    Left = 40,
                    // set top position
                    Top = 50,
                    // set up new text
                    Text = "Mr. John Smith"
                };

                // update signature
                bool updateResult = signature.Update(signatureToUpdate);

                // process updation result
                if (updateResult)
                {
                    Console.WriteLine("Signature was updated successfully!");
                }
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Atualizando as assinaturas Text nas páginas do documento - Demonstração ao vivo"
    content: |
       Edite várias assinaturas eletrônicas do documento Pdf agora mesmo visitando o site do [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Atualize várias assinaturas Text via C#"
    content: |
        "Edição de assinaturas digitais que são colocadas em vários formatos de documentos. Atualize os dados de assinaturas sem código extra."
    format: 
       
       
back_to_top:
    enable: true
---