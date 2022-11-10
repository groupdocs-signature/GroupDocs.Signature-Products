---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Qrcode
fileformat: Potm
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Qrcode signatures at Potm with Java

############################# Head ############################
head_title: "Procure por assinaturas Qrcode no arquivo Potm em Java"
head_description: "Use Java para pesquisar assinaturas Qrcode em arquivos Potm usando algumas linhas de código."

############################# Header ############################
title: "Procure por assinaturas Qrcode no arquivo Potm"
description: "A API nativa do Java permite pesquisar assinaturas Qrcode em arquivos Potm já assinados. Realize uma pesquisa avançada de assinatura eletrônica em seus documentos Potm usando algumas linhas de código."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "Sobre a API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) fornece a API Java para processar documentos usando vários tipos de assinatura, como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados. Os usuários podem adicionar, excluir, atualizar, verificar ou pesquisar assinaturas eletrônicas em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem, com suporte adicional para personalizar as propriedades das assinaturas conforme necessário.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como pesquisar assinaturas de Qrcode em Potm"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) torna mais fácil para os desenvolvedores do Java pesquisar assinaturas Qrcode em arquivos Potm de seus aplicativos implementando algumas etapas fáceis.
        
        * Crie uma nova instância da classe Signature e passe o caminho do documento de origem como um parâmetro de construtor.
        * Instancie o objeto SearchOptions de acordo com seus requisitos e especifique as opções de pesquisa.
        * Chame o método Search da instância da classe Signature e passe SearchOptions para ele.
        * Processe os resultados da pesquisa de acordo com suas demandas.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faça o download da versão mais recente do GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Potm file
        String filePath = "input.potm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Create search options
        QrCodeSearchOptions options = new QrCodeSearchOptions();

        // specify special pages to search on 
        options.setAllPages(false);
        // single page number
        options.setPageNumber(1);
        // specify text match type
        options.setMatchType(TextMatchType.Contains);
        // specify text pattern to search
        options.setText("Text signature");
        // return  Qrcode images for processing
        options.setReturnContent(true);
        // set up type of returned  Qrcode images
        options.setReturnContentType(FileType.PNG);
                            
        // search for Qrcode signatures in Potm document
        List<QrCodeSignature> signatures = signature.search(QrCodeSignature.class, options);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Pesquise por Qrcode assinaturas eletrônicas Demonstração ao vivo"
    content: |
       Pesquise no documento várias assinaturas eletrônicas para arquivos Potm agora mesmo visitando o site do [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Pesquise outras assinaturas Qrcode usando Java"
    content: |
        "Pesquisa de assinaturas eletrônicas em vários documentos. Encontre assinaturas de um dos formatos de arquivo populares, conforme mostrado abaixo."
    format: 
           
       
back_to_top:
    enable: true
---