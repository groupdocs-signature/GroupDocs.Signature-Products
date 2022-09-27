---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltx
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltx for C#

############################# Head ############################
head_title: "C#을(를) 통해 Xltx 문서에 메타데이터 전자 서명 추가"
head_description: "몇 줄의 C# 코드를 사용하여 Xltx 문서 내에서 메타데이터를 숨겨진 전자 서명으로 사용합니다. GroupDocs 문서 서명 API를 사용하여 메타데이터 정보가 포함된 비즈니스 문서 및 파일에 전자 서명합니다."

############################# Header ############################
title: ".NET를 통한 Xltx 문서의 메타데이터 전자 서명은 간단하고 사용하기 쉽습니다!"
description: "숨겨진 메타데이터 항목으로 Xltx 문서 및 계약에 전자 서명합니다. 문제 및 추가 코딩 없이 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션 및 다양한 이미지 형식에 대한 메타데이터를 생성합니다."
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
    title: "{metadata-about.title}"
    content: |
        {metadata-about.content}
    

############################# Steps ############################
steps:
    enable: true
    title_left: "{metadata-steps.title}"
    content_left: |
        {metadata-steps.content.description}
        
        * {metadata-steps.content.step_1}
        * {metadata-steps.content.step_2}
        * {metadata-steps.content.step_3}

    title_right: " {system-requirements.title}"
    content_right: |
        {system-requirements.content.description}

        * {system-requirements.content.step_1}
        * {system-requirements.content.step_2}
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * {system-requirements.content.step_3}
         
    code: |
        ```csharp    
        
        // Set up input Xltx file
        string filePath = "input.xltx";
        // Set up output file
        string outputFilePath = "output.xltx";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // instantiate metadata signing options
                var options = new MetadataSignOptions();

                // setup Author property
                SpreadsheetMetadataSignature mdSign_Author = new SpreadsheetMetadataSignature("Author", "Mr.Scherlock Holmes");// String value
                options.Signatures.Add(mdSign_Author);
                // setup document data
                SpreadsheetMetadataSignature mdSign_DocData = new SpreadsheetMetadataSignature("CreatedOn", DateTime.Now);// Datetime value
                options.Signatures.Add(mdSign_DocData);
                // setup document id
                SpreadsheetMetadataSignature mdSign_DocId = new SpreadsheetMetadataSignature("DocumentId", 123456);// Integer value
                options.Signatures.Add(mdSign_DocId);
                
                // sign Xltx document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata 라이브 데모로 Xltx 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Xltx 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Metadata 서명"
    content: |
        "다른 서명 유형으로 Xltx에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
       
       
back_to_top:
    enable: true
---