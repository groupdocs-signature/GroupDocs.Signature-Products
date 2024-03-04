---
############################# Static ############################
layout: "landing"
date: 2024-03-04T17:52:03
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: pt
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET, Java, APIs de nuvem e aplicativos de assinatura de documentos on-line"
head_description: "Obtenha uma solução completa de assinatura eletrônica de documentos para aplicativos .NET, Java e baseados em nuvem. Assine formatos de documentos comuns online usando o recurso simples de arrastar e soltar"

############################# Header ############################
title: "Assinar documentos<br>com API Node.js."
description: "Assine documentos e imagens digitais em qualquer plataforma usando nossas APIs flexíveis e soluções baseadas em aplicativos para programadores e usuários finais."
words:
  for: "para"

actions:
  main: "Baixe do NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Pronto para começar?"
  description: "Experimente os recursos do GroupDocs.Signature gratuitamente ou solicite uma licença"

release:
  title: "Versão {0} lançada"
  notes: "Veja o que é novo"
  downloads: "Transferências"

code:
  title: "Assinando PDFs por Node.js"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```javascript {style=abap}   
    // Selecione o documento PDF
    let signature = new Signature("sample.pdf");
    
    // Fornecer texto
    let options = new TextSignOptions("John Smith");
    
    // Definir cor
    options.ForeColor = Color.Red;
    
    // Assine o documento e salve em arquivo
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Visão geral do GroupDocs.Signature"
  description: "Biblioteca de assinatura de documentos pronta para ser usada em aplicativos Node.js."
  features:
    # feature loop
    - title: "Solução de assinatura digital para documentos comerciais com Node.js"
      content: "GroupDocs.Signature for Node.js via Java oferece um conjunto abrangente de opções de assinatura digital para PDF, documentos do Office e imagens. Texto, códigos de barras, imagens, certificados digitais e metadados estão disponíveis. O processamento simplificado de documentos garante eficiência."

    # feature loop
    - title: "Manipulação Avançada de Documentos Assinados"
      content: "GroupDocs.Signature permite que você processe documentos assinados. Pesquise e valide assinaturas usando vários critérios. Além disso, extraia informações detalhadas do documento ou gere imagens de visualização das páginas."

    # feature loop
    - title: "Diversos formatos de saída"
      content: "Nossa solução oferece amplo controle sobre o formato de saída de documentos assinados. Posicione assinaturas com precisão em qualquer página e personalize sua aparência. Salve documentos assinados em vários formatos suportados e, opcionalmente, proteja-os com senhas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de plataforma"
  description: "GroupDocs.Signature for Node.js via Java realiza processamento de documentos com vários sistemas operacionais"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    GroupDocs.Signature for Node.js via Java facilita operações para [formatos de arquivo populares](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Recursos de GroupDocs.Signature"
  description: "Assine PDFs, documentos do Office e imagens com assinaturas digitais"

  items:
    # feature loop
    - icon: "sign"
      title: "Assinaturas Empresariais"
      content: "Empregue vários tipos de assinatura para assinar documentos. Coloque assinaturas digitais com precisão em qualquer local da página."

    # feature loop
    - icon: "custom"
      title: "Personalizando a aparência da assinatura"
      content: "Personalize os aspectos visuais das assinaturas ajustando cor, fonte, bordas, rotação e muito mais para alcançar o resultado desejado."

    # feature loop
    - icon: "password"
      title: "Documentos protegidos por senha"
      content: "Para muitos formatos de documentos suportados, proteja os documentos assinados com uma senha para maior segurança."

    # feature loop
    - icon: "protect"
      title: "Prevenção de modificações não autorizadas"
      content: "Proteja documentos comerciais cruciais assinados com certificados digitais contra alterações não autorizadas."

    # feature loop
    - icon: "convert"
      title: "Formatos de saída desejados"
      content: "Obtenha documentos assinados sem esforço em qualquer formato compatível. Converta documentos do MS Word para o formato PDF com facilidade."

    # feature loop
    - icon: "preview"
      title: "Visualização de documentos"
      content: "Salve páginas individuais do documento como imagens para necessidades futuras."

    # feature loop
    - icon: "search"
      title: "Pesquisa de assinatura"
      content: "Recupere informações sobre assinaturas adicionadas anteriormente em seus documentos."

    # feature loop
    - icon: "validate"
      title: "Validação de Documentos"
      content: "Verifique a autenticidade das assinaturas apresentadas em qualquer documento."

    # feature loop
    - icon: "update"
      title: "Gerenciamento de assinatura"
      content: "Exclua, realoque ou modifique qualquer assinatura colocada em qualquer página do documento."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Amostras de código"
  description: "Exemplos ilustrativos que mostram operações típicas do GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Marcar PDF com códigos QR"
      content: |
        Incorporar [códigos de barras](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) em páginas específicas de documentos PDF pode agilizar os processos de negócios. Esta seção fornece um exemplo de adição de um código QR usando GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Como colocar código QR em PDF.">}}
        ```javascript {style=abap}
        // Carregue o documento para assinar
        let signature = new Signature("file_to_sign.pdf");
        
        // Crie opções de código QR com texto predefinido
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Configure o tipo de codificação do código QR e a posição na página
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Assine o documento e salve-o como arquivo de resultado
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Protegendo um DOCX com assinatura digital"
      content: |
        [Proteja seus documentos](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) por meio de assinaturas baseadas em certificados digitais. A assinatura digital protege seus documentos comerciais contra alterações de conteúdo.
        {{< landing/code title="Veja como garantir a integridade do documento.">}}
        ```javascript {style=abap}   
        // Carregue o documento a ser assinado digitalmente
        let signature = new Signature("file_to_sign.pdf");
        
        // Especifique as opções de assinatura digital e forneça o caminho para o arquivo do certificado
        let options = new DigitalSignOptions("certificate.pfx");

        // Defina a senha do certificado
        options.Password = "1234567890";

        // Assine o documento e salve-o no caminho desejado
        signature.Sign("digitally_signed.pdf", options);

        ```
        {{< /landing/code >}}

---
