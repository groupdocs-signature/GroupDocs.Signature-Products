---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Interleaved2of5
fileformat: Pptm
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Pptm for Java

############################# Head ############################
head_title: "Java의 Interleaved2of5 바코드로 Pptm 문서에 전자 서명"
head_description: "Interleaved2of5 Barcode Signature를 생성하고 몇 줄의 코드를 사용하여 Java를 사용하여 Pptm 문서에 넣습니다. 다양한 파일 형식에 서명하려면 GroupDocs 문서 서명 API를 사용하십시오."

############################# Header ############################
title: "Java에서 Pptm 문서에 대한 Interleaved2of5 바코드 서명 생성"
description: "Interleaved2of5 바코드로 Pptm 비즈니스 문서에 전자 서명하세요. 서명 옵션을 설정하는 몇 줄의 코드로 빠르고 쉽게 바코드 서명을 생성합니다."
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
    title: "{barcode-about.title}"
    content: |
        {barcode-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{barcode-steps.title}"
    content_left: |
        {barcode-steps.content.description}
        
        * {barcode-steps.content.step_1}
        * {barcode-steps.content.step_2}
        * {barcode-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Java runtime: J2SE 6.0 and above
        * {system-requirements.content.step_3}
         
    code: |
        ```java    
                
        // Set up input Pptm file
        String filePath = "input.pptm";
        // Set up output file
        String outputFilePath = "output.pptm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.Interleaved2of5);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Pptm document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode 라이브 데모로 Pptm 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Pptm 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Interleaved2of5 Barcode"
          content: |
            Interleaved 2 of 5(ITF)는 숫자를 인코딩하는 연속 2폭 바코드 기호입니다. 135 필름, ITF-14 바코드 및 일부 제품의 상자에 상업적으로 사용되며 내부 제품에는 UPC 또는 EAN 라벨이 붙어 있습니다.
          characterset: |
             숫자(0-9).
          textcapacity: |
             가변 길이.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAB8AAACGCAYAAAAlx1GyAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAFdSURBVHhe7Y0xCkJRAMPe/S/9BSFLqHaSN9hAhyzNeS6y+BUWv8LX+DnnPfjkHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3ikXaGe2A3i0faGe6B3SweaWe4B3azeKSd4R7YzeKRdoZ7YDeLR9oZ7oHdLB5pZ7gHdrN4pJ3hHtjN4pF2hntgN4tH2hnugd0sHmlnuAd2s3ikneEe2M3X+K9Z/Ar/Gn+eF5E2tt5Q4JATAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java에 대해 지원되는 기타 Barcode 서명"
    content: |
        "다른 서명 유형으로 Pptm에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
        
       
back_to_top:
    enable: true
---