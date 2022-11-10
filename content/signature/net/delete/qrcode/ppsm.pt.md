---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Delete
signaturetype: Qrcode
fileformat: Ppsm
productName: .NET
lang: pt
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Qrcode signature on Ppsm for C#

############################# Head ############################
head_title: "Excluir assinaturas Qrcode de arquivos Ppsm via C#"
head_description: "A exclusão de assinaturas Qrcode específicas de documentos Ppsm assinados pode ser realizada facilmente com o código curto .NET."

############################# Header ############################
title: "Remova as assinaturas Qrcode que são colocadas em arquivos Ppsm"
description: "Exclua várias assinaturas Qrcode de documentos Ppsm. A remoção de assinaturas Qrcode requer um código C# simples."
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
    title: "Obtenha informações sobre os recursos da API GroupDocs.Signature for .NET"
    content: |
        A API [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) oferece várias maneiras de processar seus documentos usando assinaturas eletrônicas. Assinaturas digitais como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados estão disponíveis. Os clientes têm a possibilidade de adicionar, excluir, atualizar, verificar ou pesquisar assinaturas digitais em PDFs, documentos MS Word, pastas de trabalho MS Excel, apresentações MS PowerPoint, arquivos Adobe Photoshop e vários formatos de imagem. Um grande número de recursos e configurações úteis são fornecidos.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como remover assinaturas Qrcode do seu documento Ppsm"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/) fornece um recurso útil para limpar documentos Ppsm de assinaturas Qrcode com algumas linhas de código.
        
        * Em primeiro lugar, instancie o objeto Signature passando o caminho para o seu documento como um parâmetro do construtor.
        * Em seguida, crie um objeto de assinatura apropriado e configure seu identificador exclusivo.
        * Depois disso, invoque o método Delete passando o objeto de assinatura que deve ser excluído.
        * Finalmente, os resultados da operação do processo.

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
                // Id of signature which is supposed to be deleted
                // such Id may be obtained as result of search operation
                string id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

                // provide signature features to delete
                // set up particular signature id
                QrCodeSignature signatureToDelete = new QrCodeSignature(id);

                // delete signature
                bool deleteResult = signature.Delete(signatureToDelete);

                // process deletion result
                if (deleteResult)
                {
                    Console.WriteLine("Signature was deleted successfully!");
                }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinar com assinaturas Qrcode Demonstração ao vivo"
    content: |
       Adicione várias assinaturas eletrônicas ao arquivo Ppsm agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Exclua suas assinaturas Qrcode com C#"
    content: |
        "Exclusão de assinaturas eletrônicas que foram adicionadas a vários formatos de documentos. Remova assinaturas rapidamente sem código extra."
    format: 
       
       
back_to_top:
    enable: true
---