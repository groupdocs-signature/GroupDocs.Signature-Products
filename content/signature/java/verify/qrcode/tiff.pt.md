---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Qrcode
fileformat: Tiff
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Qrcode signature on Tiff for Java

############################# Head ############################
head_title: "Verificação de assinaturas Qrcode para arquivos Tiff via Java"
head_description: "Use apenas algumas linhas de código Java para verificar documentos Tiff e suas assinaturas Qrcode."

############################# Header ############################
title: "Qrcode verificação de assinaturas para Tiff arquivos"
description: "A API para Java oferece a oportunidade de verificar assinaturas Qrcode em documentos Tiff. A verificação de assinaturas eletrônicas dentro de seus documentos Tiff pode ser realizada de forma rápida e fácil."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Descubra os novos recursos da API GroupDocs.Signature for Java"
    content: |
        A API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) oferece uma ampla variedade de maneiras de processar vários formatos de documentos usando assinaturas eletrônicas. Muitos tipos de assinaturas digitais como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados são suportados. Os clientes podem adicionar, remover, editar, validar ou pesquisar assinaturas digitais em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Um número surpreendente de recursos e configurações adicionais estão disponíveis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como validar assinaturas Qrcode em seu documento Tiff"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclui recursos úteis, como verificação de Qrcode assinaturas colocadas em documentos Tiff. Use esta oportunidade sem implementar código extra.
        
        * Em primeiro lugar, instanciar a classe Signature fornecendo como um caminho de parâmetro construtor para um documento que deve ser verificado.
        * Em segundo lugar, crie um novo objeto VerifyOptions e configure todas as propriedades necessárias.
        * Por fim, invoque o método Verify do objeto Signature passando a instância VerifyOptions.
        * Em seguida, processe os resultados da verificação.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faça o download da versão mais recente do GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Tiff file
        String filePath = "input.tiff";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        QrCodeVerifyOptions options = new QrCodeVerifyOptions();

        // process only first page
        options.setPagesSetup(new PagesSetup());
        options.setPageNumber(1);
        options.setAllPages(false);
        // specify text match type
        options.setMatchType(TextMatchType.StartsWith);
        // specify text pattern to search
        options.setText("QrCode text");
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinar com assinaturas Qrcode Demonstração ao vivo"
    content: |
       Adicione várias assinaturas eletrônicas ao arquivo Tiff agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Verifique outras assinaturas Qrcode usando Java"
    content: |
        "Verificação de assinaturas eletrônicas colocadas em vários documentos. Verifique a qualidade das assinaturas nos formatos de arquivo populares, conforme revelado abaixo."
    format: 
       
       
back_to_top:
    enable: true
---