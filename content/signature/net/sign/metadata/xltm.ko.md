---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Metadata
fileformat: Xltm
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put Metadata signature on Xltm for C#

############################# Head ############################
head_title: "C#을(를) 통해 Xltm 문서에 메타데이터 전자 서명 추가"
head_description: "몇 줄의 C# 코드를 사용하여 Xltm 문서 내에서 메타데이터를 숨겨진 전자 서명으로 사용합니다. GroupDocs 문서 서명 API를 사용하여 메타데이터 정보가 포함된 비즈니스 문서 및 파일에 전자 서명합니다."

############################# Header ############################
title: ".NET를 통한 Xltm 문서의 메타데이터 전자 서명은 간단하고 사용하기 쉽습니다!"
description: "숨겨진 메타데이터 항목으로 Xltm 문서 및 계약에 전자 서명합니다. 문제 및 추가 코딩 없이 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션 및 다양한 이미지 형식에 대한 메타데이터를 생성합니다."
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
    title: "GroupDocs.Signature for .NET 메타데이터 서명 API 정보"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 디지털 문서 전자 서명에 널리 사용되는 API입니다. 텍스트, 이미지, 디지털 인증서, 바코드, QR 코드, 스탬프 또는 메타데이터와 같은 서명을 사용할 수 있습니다. 서명은 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에 배치될 수 있습니다. 고객은 문서에 서명하고 해당 문서에 있는 전자 서명을 업데이트, 검색, 확인, 삭제 또는 미리 볼 수 있습니다. 또한 서명 사용자 정의를 위한 많은 기능이 제공됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Metadata으로 Xltm에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Metadata 서명으로 Xltm 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Xltm 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Xltm 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: " 시스템 요구 사항"
    content_right: |
        GroupDocs.Signature for .NET은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
        
        // Set up input Xltm file
        string filePath = "input.xltm";
        // Set up output file
        string outputFilePath = "output.xltm";

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
                
                // sign Xltm document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata 라이브 데모로 Xltm 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Xltm 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Metadata 서명"
    content: |
        "다른 서명 유형으로 Xltm에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
       
       
back_to_top:
    enable: true
---