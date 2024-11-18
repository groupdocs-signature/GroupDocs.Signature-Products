



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:02
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#를 사용하여 XLSX 파일에 QR 코드 생성"
head_description: "GroupDocs.Signature API를 활용하여 XLSX 파일에 QR 코드를 생성합니다. 향상된 기능을 위해 어느 페이지에나 QR 코드를 원활하게 임베드하세요."

############################# Header ############################
title: "XLSX용 QR 코드 생성" 
description: "텍스트 또는 숫자 데이터를 사용하여 2D 바코드를 생성하고 PDF, Word, Excel 등 다양한 페이지와 형식에 적용할 수 있습니다. GroupDocs.Signature for .NET를 통해 간편하게 실현하세요."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 사용해 보기"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET의 기능 탐색"
    link: "/signature/net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)는 다양한 서명 유형을 생성하고 임베드할 수 있는 기능을 제공합니다. PDF, Word 문서, Excel 시트, PowerPoint 프레젠테이션 또는 이미지 파일과 같은 주요 문서 형식에서 텍스트, 이미지, 바코드, QR 코드, 메타데이터, 디지털 및 스탬프 서명으로 문서의 품질을 향상시킬 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 내 모든 장소에 QR 코드를 생성하고 삽입하는 방법"
    content: |
      [GroupDocs.Signature](/signature/net/) 은 다양한 인기 있는 형식에서 QR 코드를 생성하고 XLSX 페이지에 배치할 수 있는 기능을 제공합니다. 10가지 이상의 QR 코드 유형을 지원하며, 우리의 라이브러리는 .NET 애플리케이션에 원활하게 통합할 수 있습니다. 우리 제품을 사용하여 QR 코드 서명으로 문서를 향상시켜 보세요.
      
      1. XLSX 파일 또는 QR 코드로 서명할 스트림을 준비합니다.
      2. QrCodeSignOptions에 필요한 텍스트를 제공합니다.
      3. 색상, 위치, 크기 등 시각적 매개변수를 사용자 정의합니다.
      4. 임베드된 QR 코드로 문서를 저장합니다.
   
    code:
      platform: "net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // 문서와 함께 새로운 Signature 인스턴스를 초기화합니다.
        using (Signature signature = new Signature("input.xlsx"))
        {
            // QrCodeSignOptions를 사용하여 문서에 QR 코드를 임베드합니다.
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // 서명 유형을 지정하고 페이지에서 위치를 설정합니다.
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // QR 코드가 통합된 문서를 저장합니다.
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서를 위한 포괄적인 서명 통합"
  description: "GroupDocs.Signature for .NET API를 통해 사용자는 쉽게 여러 서명 유형을 생성, 수정, 검색, 검증 및 제거할 수 있으며, 문서 워크플로우를 뛰어난 정확성으로 간소화할 수 있습니다."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "다양한 서명 유형을 통한 문서 서명"
      content: "GroupDocs.Signature는 텍스트, 이미지, 바코드, QR 코드 및 스탬프 서명을 모든 문서 형식에 적용할 수 있도록 지원합니다. 서명은 임의의 페이지에 정확하게 배치할 수 있으며, 메타데이터 서명을 통해 메타데이터를 원활하게 관리할 수 있습니다. 디지털 인증서를 통합하여 문서의 무결성을 보호하고 무단 변경을 방지하십시오."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "고급 검증 과정을 통해 문서 서명의 진위와 정확성을 확인하십시오. 문서에 임베드된 모든 서명의 상세 목록을 쉽게 검색하여 포괄적인 검토를 수행할 수 있습니다."

    # feature loop
    - title: "커스터마이징 가능한 서명 수정"
      content: "이전 서명을 수정하여 내용, 위치, 색상, 크기 및 기타 속성을 조정하여 특정 요구사항에 맞게 업데이트할 수 있습니다."

    # feature loop
    - title: "효율적인 서명 제거"
      content: "불필요한 서명을 프로그래밍적으로 제거하여 문서 관리 과정을 단순화합니다. 디지털 인증서 또는 기타 서명 유형을 처리할 때 신속하고 효과적으로 제거할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "다양한 옵션으로 QR 코드 생성 방법?"
      content: |
        이 예제는 XLSX 페이지에 맞춤형 QR 코드를 배치하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 서명할 문서를 가져오고 Signature에 전달합니다.
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 필요한 텍스트로 QR 코드 옵션을 설정합니다.
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // 페이지에서 QR 코드의 상대적 위치를 지정합니다.
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // 서명 여백을 설정합니다.
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // QR 코드 색상을 지정합니다.
                    ForeColor = Color.Red,

                    // 메시지의 글꼴 옵션을 정의합니다.
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // QR 코드 배경 색상 및 브러시를 사용자 정의합니다.
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // QR 코드를 문서에 임베드합니다.
              SignResult result = signature.Sign("output.xlsx", options);
          }
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.xlsx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "Nuget 다운로드"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "우리의 서명 솔루션에 대해 알아보기"
    exclude: "qrcode"
    description: "다양한 서명 유형과 운영 기능을 자랑스럽게 소개합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/net/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/net/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/net/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/net/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/net/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/net/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/net/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/net/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/net/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/net/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/net/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다른 문서 형식에 대한 QR 코드 생성"
    exclude: "XLSX"
    description: ".NET API를 통해 모든 업계 표준 파일 형식에 QR 코드를 임베드할 수 있는 기능을 추가하여 2D 바코드에 중요한 정보를 저장하고 인코딩합니다."
    items: 
          
        # format loop 1
        - name: "PDF용 QR 코드"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX용 QR 코드"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG용 QR 코드"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX용 QR 코드"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX용 QR 코드"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---