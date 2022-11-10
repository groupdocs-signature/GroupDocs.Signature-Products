---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Barcode
fileformat: Docx
productName: Java
lang: pt
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Barcode signature on Docx for Java

############################# Head ############################
head_title: "Atualize assinaturas Barcode colocadas em arquivos Docx com Java"
head_description: "Use o código Java simples e fácil para atualização de assinaturas Barcode em documentos Docx assinados."

############################# Header ############################
title: "Edite e atualize assinaturas Barcode colocadas em arquivos Docx"
description: "A API para Java fornece funcionalidade para atualização de assinaturas Barcode em documentos Docx. Atualize assinaturas eletrônicas dentro de seus documentos Docx com algumas linhas de código Java de forma rápida e fácil."
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
    title: "Saiba mais sobre os recursos da API GroupDocs.Signature for Java"
    content: |
        A funcionalidade da API [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) contém uma vasta seleção de meios para processar em formatos de documentos sob demanda usando assinaturas eletrônicas. Amplo espectro de assinaturas eletrônicas, como textos, imagens, certificados digitais, códigos de barras, códigos QR, selos ou metadados são suportados. Os clientes podem adicionar, remover, editar, validar ou pesquisar assinaturas digitais em PDFs, documentos do MS Word, pastas de trabalho do MS Excel, apresentações do MS PowerPoint, arquivos do Adobe Photoshop e vários formatos de imagem. Vários recursos e configurações úteis estão disponíveis.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Como alterar assinaturas Barcode em seu documento Docx"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) inclui recursos úteis como atualização de Barcode assinaturas colocadas em documentos Docx. Possibilita alterar recursos de assinaturas sem código extra.
        
        * Para começar, crie o objeto Signature passando como um caminho de parâmetro construtor para um documento que deve ser atualizado.
        * Em seguida, instancie um objeto de assinatura específico apropriado e configure seu identificador e propriedades que precisam ser alteradas.
        * Por último, chame o método Update do Signature passando um objeto de assinatura específico.
        * Processe a atualização dos resultados ao seu aviso.

    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Signature for Java são compatíveis com todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.

        * Sistemas operacionais: Microsoft Windows, Linux, MacOS
        * Ambientes de desenvolvimento: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * Faça o download da versão mais recente do GroupDocs.Signature for Java de [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)
         
    code: |
        ```java    
                
        // Set up input Docx file
        String filePath = "input.docx";
        // Set up output file
        String outputFilePath = "output.docx";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "07f83369-318b-41ad-a843-732417b912c2";

        // provide signature features to update
        // set up particular signature id
        BarcodeSignature signatureToUpdate = new BarcodeSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(300);
        // specify signature height
        signatureToUpdate.setHeight(50);
        // set left position
        signatureToUpdate.setLeft(80);
        // set top position
        signatureToUpdate.setTop(100);

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Atualizando as assinaturas Barcode nas páginas do documento - Demonstração ao vivo"
    content: |
       Edite várias assinaturas eletrônicas do documento Docx agora mesmo visitando o site do [GroupDocs.Signature App](https://products.groupdocs.app/signature/family).          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Atualize várias assinaturas Barcode via Java"
    content: |
        "Edição de assinaturas digitais que são colocadas em vários formatos de documentos. Atualize os dados de assinaturas sem código extra."
    format: 
       
       
back_to_top:
    enable: true
---