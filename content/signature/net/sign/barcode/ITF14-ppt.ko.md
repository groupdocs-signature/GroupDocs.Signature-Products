---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: I T F14
fileformat: Ppt
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Ppt for C#

############################# Head ############################
head_title: "C#의 I T F14 바코드로 Ppt 문서에 전자 서명"
head_description: "I T F14 Barcode Signature를 생성하고 몇 줄의 코드를 사용하여 .NET를 사용하여 Ppt 문서에 넣습니다. 다양한 파일 형식에 서명하려면 GroupDocs 문서 서명 API를 사용하십시오."

############################# Header ############################
title: "C#에서 Ppt 문서에 대한 I T F14 바코드 서명 생성"
description: "I T F14 바코드로 Ppt 비즈니스 문서에 전자 서명하세요. 서명 옵션을 설정하는 몇 줄의 코드로 빠르고 쉽게 바코드 서명을 생성합니다."
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
    title: "GroupDocs.Signature for .NET Barcode signatures API 정보."
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN과 같은 바코드 유형을 사용하여 디지털 문서 전자 서명을 관리하는 빠르고 쉬운 API입니다. , ITF14 및 기타 다수. 고객은 필요한 텍스트를 제공하는 바코드를 쉽게 생성하여 PDF, Microsoft Office Words 문서, Microsoft Office Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에 넣을 수 있습니다. 문서에 배치된 바코드는 업데이트, 검색, 확인, 삭제 또는 미리 볼 수 있습니다. 또한 바코드 사용자 정의가 지원됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Barcode으로 Ppt에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Barcode 서명으로 Ppt 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Ppt 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Ppt 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: " 시스템 요구 사항"
    content_right: |
        GroupDocs.Signature for .NET은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
        
        // Set up input Ppt file
        string filePath = "input.ppt";
        // Set up output file
        string outputFilePath = "output.ppt";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.I T F14,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Ppt document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode 라이브 데모로 Ppt 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Ppt 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About I T F14 Barcode"
          content: |
            ITF-14는 국제 무역 품목 번호를 인코딩하기 위해 Interleaved 2 of 5(ITF) 바코드의 GS1 구현입니다.
          characterset: |
             숫자(0-9).
          textcapacity: |
             13자리 + 1 체크 디지트.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Barcode 서명"
    content: |
        "다른 서명 유형으로 Ppt에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
        
       
back_to_top:
    enable: true
---