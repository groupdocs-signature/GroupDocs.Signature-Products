---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Digital
fileformat: Ots
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Ots for C#

############################# Head ############################
head_title: "C#을(를) 사용하여 Ots 파일에 디지털 전자 서명 추가"
head_description: "몇 줄의 코드를 사용하여 .NET에 대한 Ots 파일에 디지털 서명을 넣습니다. GroupDocs 문서 서명 API를 사용하여 수십 가지 파일 형식에 서명합니다."

############################# Header ############################
title: "C#에서 Digital 서명이 있는 Ots 파일에 eSign"
description: "몇 줄의 .NET 코드로 Digital 서명을 추가하는 방법"
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
    title: "GroupDocs.Signature for .NET 디지털 서명 API 정보"
    content: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 디지털 인증서와 함께 디지털 전자 서명으로 문서를 서명하는 데 널리 사용되는 API입니다. 디지털 서명의 경우 API는 PFX 인증서 파일을 사용하여 암호로 보호된 개인 및 공개 키로 문서에 서명합니다. 디지털 서명은 eSign PDF 특정 페이지로 비즈니스 문서를 인증하고 Words, Excel, Powerpoint 파일 및 Open Office 문서와 같은 전체 Microsoft Office 문서를 인증하는 데 사용될 수 있습니다. 고객은 서명 편집, 제거 또는 조정과 같이 서명을 쉽게 조작할 수 있습니다. API는 서명을 검색하고 확인하는 방법을 제공합니다. 또한 서명 사용자 정의를 위한 많은 기능이 제공됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Digital으로 Ots에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Digital 서명으로 Ots 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Ots 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Ots 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: " 시스템 요구 사항"
    content_right: |
        GroupDocs.Signature for .NET은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
                
        // Set up input Ots file
        string filePath = "input.ots";
        // Set up output file
        string outputFilePath = "output.ots";
        // Provide digital certificate
        string certificateFilePath = "certificate.pfx";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                //Provide sign options
                DigitalSignOptions options = new DigitalSignOptions(certificateFilePath)
                {
                    // set certificate password
                    Password = "1234567890",
                    // set signature position
                    Left = 50,
                    Top = 200,
                };

                // sign Ots document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital 라이브 데모로 Ots 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Ots 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Digital 서명"
    content: |
        "다른 서명 유형으로 Ots에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
       
       
back_to_top:
    enable: true
---