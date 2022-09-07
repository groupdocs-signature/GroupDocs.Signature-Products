---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Qrcode
codetype: Aztec
fileformat: Xls
productName: .NET
lang: ko
productCode: net
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Qrcode signature on Xls for C#

############################# Head ############################
head_title: "C#의 Aztec QR 코드로 Xls 문서에 전자 서명"
head_description: "짧은 C# 코드와 함께 .NET을(를) 사용하여 Aztec QR 코드를 생성하고 Xls 파일에 넣습니다. GroupDocs 문서 서명 API를 사용하여 QR 코드로 비즈니스 문서 및 파일에 전자 서명하십시오."

############################# Header ############################
title: "C#에서 Xls 문서에 대한 Aztec QR 코드 서명 생성"
description: "Aztec QR 코드로 Xls 문서 및 계약에 전자 서명합니다. QR 코드 서명을 빠르고 쉽게 생성합니다."
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
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 QR 코드를 사용한 디지털 문서 전자 서명을 위한 성숙한 API입니다. 사용자는 요청된 텍스트를 제공하는 QR 코드 서명을 생성하여 다운로드하거나 이미지로 소셜 미디어에 공유할 수 있습니다. 서명된 문서는 API 또는 모바일 카메라를 통해 간단히 스캔할 수 있습니다! QR 코드 서명을 추가하여 비즈니스 계약 및 공식 문서에 전자 서명하고 조작하십시오. 모든 QR 코드 서명에는 서명자를 식별하거나 문서를 승인하는 고유한 사용자 지정 정보가 포함됩니다. 또한 QR 코드 콘텐츠는 프로그래밍 방식으로 개인 키로 암호화 및 해독할 수 있습니다. 이는 공개 문서 내에서 민감한 데이터를 공유할 수 있는 많은 기능을 제공합니다. 서명 후 사용자는 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식 내에서 QR 코드를 업데이트, 확인, 삭제, 미리보기 또는 검색할 수 있습니다. QR 코드는 추가로 사용자 정의할 수 있습니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "C#에서 Qrcode으로 Xls에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for .NET](https://products.groupdocs.com/signature/net/)은 Qrcode 서명으로 Xls 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Xls 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Xls 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for .NET을(를) 사용한 문서 서명은 몇 가지 간단한 단계로 수행할 수 있습니다. 당사의 API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Microsoft Visual Studio, Xamarin, MonoDevelop
        * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        * [Nuget](https://www.nuget.org/packages/groupdocs.signature)에서 최신 GroupDocs.Signature for .NET 가져오기
         
    code: |
        ```csharp    
                
        // Set up input Xls file
        string filePath = "input.xls";
        // Set up output file
        string outputFilePath = "output.xls";

        // Instantiate Signature for input file
        using (GroupDocs.Signature.Signature signature = new GroupDocs.Signature.Signature(filePath))
        {
                // create barcode option with predefined QrCode text
                QrCodeSignOptions options = new QrCodeSignOptions("JohnSmith")
                {
                    // setup QrCode encoding type
                    EncodeType = QrCodeTypes.Aztec,

                    // set signature position
                    Left = 50,
                    Top = 50,
                    Width = 200,
                    Height = 50
                };

                // sign Xls document
                SignResult result = signature.Sign(outputFilePath, options);
        }

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Qrcode 라이브 데모로 Xls 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Xls 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

              
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About Aztec QrCode"
          content: |
            아즈텍 코드는 다른 2차원 기호보다 더 높은 정확도를 갖도록 설계된 2차원(2차원) 범용 행렬 기호입니다. Aztec 코드 기호는 최대 3,832자리 숫자를 인코딩할 수 있습니다. 3,067개의 알파벳 문자; 또는 1,914바이트의 데이터.
          characterset: |
             모든 256 ASCII 문자.
          textcapacity: |
             최대 3,832개의 숫자 또는 3,067개의 알파벳 문자 또는 1,914바이트의 데이터.
          image: |
             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

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "C#에 대해 지원되는 기타 Qrcode 서명"
    content: |
        "다른 서명 유형으로 Xls에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
        
       
back_to_top:
    enable: true
---