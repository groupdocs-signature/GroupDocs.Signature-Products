---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: Pharmacode
fileformat: Tiff
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Tiff for C#

############################# Head ############################
head_title: "C#의 Pharmacode 바코드로 Tiff 문서에 전자 서명"
head_description: "Pharmacode Barcode Signature를 생성하고 몇 줄의 코드를 사용하여 .NET를 사용하여 Tiff 문서에 넣습니다. 다양한 파일 형식에 서명하려면 GroupDocs 문서 서명 API를 사용하십시오."

############################# Header ############################
title: "C#에서 Tiff 문서에 대한 Pharmacode 바코드 서명 생성"
description: "Pharmacode 바코드로 Tiff 비즈니스 문서에 전자 서명하세요. 서명 옵션을 설정하는 몇 줄의 코드로 빠르고 쉽게 바코드 서명을 생성합니다."
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
    title: "GroupDocs.Signature for .NET API 정보"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN, ITF14와 같은 다양한 바코드 유형을 사용하는 디지털 문서 전자 서명에 널리 사용되는 API입니다. 그리고 많은 다른 사람들. 고객은 원하는 텍스트만 제공하는 바코드를 쉽게 생성하여 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에 넣을 수 있습니다. 문서에 배치된 바코드는 업데이트, 검색, 확인, 삭제 또는 미리 볼 수 있습니다. 또한 바코드 사용자 정의가 지원됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Barcode으로 Tiff에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Barcode 서명으로 Tiff 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Tiff 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Tiff 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET을(를) 사용한 문서 서명은 몇 가지 간단한 단계로 수행할 수 있습니다. 당사의 API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
        
        // Set up input Tiff file
        string filePath = "input.tiff";
        // Set up output file
        string outputFilePath = "output.tiff";

        // Instantiate Signature for input file
        using (var signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined barcode text
                var options = new BarcodeSignOptions("BC12345678")
                {
                    // setup Barcode encoding type
                    EncodeType = BarcodeTypes.Pharmacode,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50                                        
                };
                
                // sign Tiff document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode 라이브 데모로 Tiff 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Tiff 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Pharmacode Barcode"
          content: |
            제약 바이너리 코드라고도 하는 Pharmacode는 제약 산업에서 포장 제어 시스템으로 사용되는 바코드 표준입니다.
          characterset: |
             숫자(0-9).
          textcapacity: |
             3에서 131070 사이의 단일 정수만 나타냅니다.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAIEAAAAkCAYAAACucVkNAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAIQSURBVHhe7dIxigQxEATB/f+n91RuUH2GEMhYBaRTasaaz/f5ee8neN5P8Lyf4FneT/C8n+B5P8Gz/PsTfD6fmtpNUrtJOr2bdnfT7d0m88vSPpTUbpLaTdLp3bS7m27vNplflvahpHaT1G6STu+m3d10e7fJ/LK0DyW1m6R2k3R6N+3uptu7TeaXpX0oqd0ktZuk07tpdzfd3m0yvyztQ0ntJqndJJ3eTbu76fZuk/llaR9KajdJ7Sbp9G7a3U23d5vML0v7UFK7SWo3Sad30+5uur3bZH5Z2oeS2k1Su0k6vZt2d9Pt3Sbzy9I+lNRuktpN0undtLubbu82mV+W9qGkdpPUbpJO76bd3XR7t8n8srQPJbWbpHaTdHo37e6m27tN5pelfSip3SS1m6TTu2l3N93ebTK/LO1DSe0mqd0knd5Nu7vp9m6T+WVpH0pqN0ntJun0btrdTbd3m8wvS/tQUrtJajdJp3fT7m66vdtkflnah5LaTVK7STq9m3Z30+3dJvPL0j6U1G6S2k3S6d20u5tu7zaZX5b2oaR2k9Rukk7vpt3ddHu3yfyytA8ltZukdpN0ejft7qbbu03ml6V9KKndJLWbpNO7aXc33d5tMr8s7UNJ7Sap3SSd3k27u+n2bpP5ZWkfSmo3Se0m6fRu2t1Nt3ebzC/Pz3g/wfN+guf9BM/yfoLn/QTP9/sHDRdB4BliyZUAAAAASUVORK5CYII=

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Barcode 서명"
    content: |
        "다른 서명 유형으로 Tiff에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
           
       
back_to_top:
    enable: true
---