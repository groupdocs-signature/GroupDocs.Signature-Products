---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Text
fileformat: Ppt
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Text signature on Ppt for Java

############################# Head ############################
head_title: "Crie assinaturas eletrônicas de texto para o arquivo Ppt com Java"
head_description: "Coloque Text eSignature no arquivo Ppt para Java usando algumas linhas de código. Use a API de assinatura de documentos do GroupDocs para assinar dezenas de formatos de arquivo."

############################# Header ############################
title: "Assine Ppt arquivos com assinaturas Text em Java"
description: "Como adicionar assinatura Text com algumas linhas de código Java"
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
    title: "Sobre a API GroupDocs.Signature for Java"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) é uma API popular para assinatura eletrônica de documentos digitais. Assinaturas como textos, imagens, certificados digitais, códigos de barras, códigos QR, carimbos ou metadados estão disponíveis. Assinaturas podem ser colocadas em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Os clientes podem assinar seu documento e atualizar, pesquisar, verificar, excluir ou visualizar assinaturas eletrônicas que foram colocadas nesses documentos. Além disso, são fornecidas muitas habilidades para personalização de assinaturas.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Etapas para assinar Ppt com Text em Java"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) permite assinar documentos Ppt com assinaturas Text de forma rápida e fácil.
        
        * Crie uma instância da classe Signature fornecendo o arquivo Ppt para assinar como caminho ou fluxo de memória
        * Instancie a classe SignOptions e defina todos os dados exigidos.
        * Invoque o método Signature.Sign() passando o arquivo de saída Ppt ou fluxo de memória

    title_right: " Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Obtenha o GroupDocs.Signature for Java mais recente de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Ppt file
        String filePath = "input.ppt";
        // Set up output file
        String outputFilePath = "output.ppt";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide sign options
        TextSignOptions options = new TextSignOptions("John Smith");

        // set signature position
        options.setLeft(50);
        options.setTop(200);

        // sign Ppt document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Assinando Ppt documentos com Text Demonstração ao vivo"
    content: |
       Assine o arquivo Ppt com várias assinaturas agora mesmo visitando o site [GroupDocs.Signature App](https://products.groupdocs.app/signature/family). Demonstração online gratuita esperando por você.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Outras assinaturas Text suportadas para Java"
    content: |
        "Você também pode assinar Ppt com outros tipos de assinatura. Por favor, veja a lista abaixo."
    format: 
       
       
back_to_top:
    enable: true
---