---
############################# Static ############################
layout: "landing"
date: 2023-09-14T19:07:22
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: pt
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: ".NET, Java, APIs de nuvem e aplicativos de assinatura de documentos on-line"
head_description: "Obtenha uma solução completa de assinatura eletrônica de documentos para aplicativos .NET, Java e baseados em nuvem. Assine formatos de documentos comuns online usando o recurso simples de arrastar e soltar"

############################# Header ############################
title: "Assinar documentos<br>através da API Java"
description: "Assine documentos e imagens digitais em qualquer plataforma usando nossas APIs flexíveis e soluções baseadas em aplicativos para programadores e usuários finais."
words:
  for: "para"

actions:
  main: "Download grátis do Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que é novo"
  downloads: "Transferências"

code:
  title: "Assine arquivos PDF em Java"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Selecione o documento PDF
    Signature signature = new Signature("sample.pdf");
    
    // Fornecer texto
    TextSignOptions options = new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Assine o documento e salve em arquivo
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão geral do GroupDocs.Signature"
  description: "API para executar assinatura de documentos e operações relacionadas em aplicativos Java"
  features:
    # feature loop
    - title: "Documentos comerciais aprimorados com assinaturas digitais em Java"
      content: "Assinatura rápida e personalizável: GroupDocs.Signature for Java oferece uma ampla gama de opções de assinatura digital para PDFs, imagens e documentos do Office. Você pode usar texto, códigos de barras, códigos QR, certificados digitais, imagens ou metadados ocultos. O processamento de documentos é rápido e eficiente."

    # feature loop
    - title: "Manipulando documentos assinados"
      content: "O processamento avançado de documentos envolve operações poderosas em documentos assinados usando GroupDocs.Signature for Java. Você pode pesquisar e validar assinaturas que foram adicionadas a documentos comerciais usando vários critérios úteis. Além disso, você pode acessar informações detalhadas sobre o documento ou obter imagens de visualização de suas páginas."

    # feature loop
    - title: "Variedade de opções de saída"
      content: "Opções robustas de assinatura permitem personalizar a saída de documentos assinados com GroupDocs.Signature for Java. Você pode posicionar com precisão qualquer assinatura em qualquer página do documento e configurar sua aparência de várias maneiras. A API Java suporta o salvamento de documentos comerciais assinados em vários formatos suportados e oferece opções para protegê-los com senhas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Signature for Java oferece suporte aos seguintes sistemas operacionais, estruturas e gerenciadores de pacotes"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Signature for Java oferece suporte a operações com os seguintes [formatos de arquivo](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos do Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Imagens e outros formatos
        * **Portátil:** PDF
        * **Imagens:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Outros formatos de escritório:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Outros formatos
        * **Rede:** HTML, MHTML
        * **Arquivos:** ZIP, TAR, 7Z
        * **Certificados:** PFX

############################# Features ############################
features:
  enable: true
  title: "Recursos do GroupDocs.Signature"
  description: "Assinatura de PDFs, documentos do Office e imagens com assinaturas digitais"

  items:
    # feature loop
    - icon: "sign"
      title: "Adicionando Assinaturas"
      content: "Assine um documento usando vários tipos de assinatura suportados, colocando uma assinatura digital precisamente em qualquer posição de qualquer página."

    # feature loop
    - icon: "custom"
      title: "Personalizando resultados"
      content: "Personalize a aparência da assinatura ajustando cor, fonte, borda, rotação e outros recursos para obter o resultado desejado."

    # feature loop
    - icon: "password"
      title: "Protegendo documentos com senha"
      content: "Para muitos tipos de documentos suportados, você pode proteger o documento assinado com uma senha."

    # feature loop
    - icon: "protect"
      title: "Evitando alterações não autorizadas"
      content: "Proteja documentos comerciais importantes assinados com um certificado digital contra modificações não autorizadas."

    # feature loop
    - icon: "convert"
      title: "Obtendo resultados nos formatos desejados"
      content: "Obtenha facilmente arquivos de resultados assinados em qualquer formato compatível. Você também pode converter documentos do MS Word em PDF sem esforço."

    # feature loop
    - icon: "preview"
      title: "Visualização do documento"
      content: "Salve qualquer página de um documento como imagem para processamento futuro."

    # feature loop
    - icon: "search"
      title: "Procurando assinaturas"
      content: "É possível obter informações sobre assinaturas previamente adicionadas em documentos específicos."

    # feature loop
    - icon: "validate"
      title: "Validando documentos"
      content: "Valide a exatidão das assinaturas em qualquer documento assinado."

    # feature loop
    - icon: "update"
      title: "Gerenciando assinaturas"
      content: "Depois que uma assinatura é colocada na página de um documento, ela pode ser excluída, movida ou atualizada conforme necessário."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Alguns casos de uso de operações típicas de GroupDocs.Signature para Java"
  items:
    # code sample loop
    - title: "Melhore o documento PDF com código QR"
      content: |
        Melhorar os processos de negócios adicionando [códigos QR](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) a páginas específicas de documentos PDF pode ser valioso. Há um exemplo de como adicionar um código QR usando GroupDocs.Signature for Java.
        {{< landing/code title="Melhore o documento PDF com código QR">}}
        ```java {style=abap}
        // Carregue o documento para assinar
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Crie opções de código QR com texto predefinido
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configure o tipo de codificação do código QR e a posição na página
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Assine o documento e salve-o como arquivo de resultado
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Use assinatura digital para proteger um DOCX"
      content: |
        Você pode [salvaguardar um documento](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) usando assinaturas pessoais ou corporativas armazenadas como certificados digitais. Os documentos protegidos por certificado não podem ser alterados sem invalidar a assinatura.
        {{< landing/code title="Use assinatura digital para proteger um DOCX">}}
        ```java {style=abap}   
        // Carregue o documento a ser assinado digitalmente
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Especifique as opções de assinatura digital e forneça o caminho para o arquivo do certificado
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Defina a senha do certificado
        options.setPassword("1234567890");

        // Assine o documento e salve-o no caminho desejado
        signature.sign("digitally_signed.pdf", options);
        ```
        {{< /landing/code >}}

---
