



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:10
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C#를 통해 XLSX 전자 서명하기"
head_description: "XLSX를 활용하여 PDF, Word, Excel, 프레젠테이션 및 이미지와 같은 다양한 형식에서 보안 및 준수를 보장하는 전자 서명 유형을 추가하세요."

############################# Header ############################
title: "XLSX 파일의 전자 서명" 
description: "GroupDocs.Signature for .NET를 사용하여 문서에 다양한 전자 서명을 삽입하고, PDF, Word, Excel, 프레젠테이션 및 이미지와 같은 형식의 준수성과 무결성을 보장하세요."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for .NET API 소개"
    link: "/signature/net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/)는 포괄적인 전자 서명 기능을 제공합니다. 이를 통해 서로 다른 문서 유형에 대해 디지털 서명을 쉽게 추가, 검색, 검증, 업데이트 및 제거할 수 있으며, 별도의 도구 없이 가능합니다. PDF 파일, Word 문서, Excel 시트, PowerPoint 프레젠테이션 및 다양한 이미지 형식의 서명을 손쉽게 지원합니다.

############################# Steps ############################
steps:
    enable: true
    title: "C#를 사용하여 XLSX 서명 단계"
    content: |
      [GroupDocs.Signature](/signature/net/)는 XLSX 파일에 맞춤형 서명을 통합할 수 있도록 지원합니다. .NET 개발자는 소프트웨어를 사용하여 서명 기능을 그들의 애플리케이션에 매끄럽게 통합할 수 있습니다.
      
      1. Signature 인스턴스에 서명을 위해 XLSX 파일을 제공합니다.
      2. SignOptions를 사용하여 서명 매개변수를 설정합니다.
      3. 크기, 색상 및 콘텐츠와 같은 속성을 구성합니다.
      4. 서명된 파일을 원하는 위치에 저장합니다.
   
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
        // 문서를 Signature 인스턴스로 로드합니다
        using (Signature signature = new Signature("input.xlsx"))
        {
            // 새 QrCodeSignOptions 객체를 생성합니다
            QrCodeSignOptions options = new QrCodeSignOptions("QR code text")
            {
                // 모든 필요한 옵션을 구성합니다
                Left = 50,
                Top = 200,
                ForeColor = Color.Red
            };

            // 서명된 문서를 로컬 저장소에 저장합니다
            SignResult result = signature.Sign("output.xlsx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 문서 전자 서명"
  description: "당사의 정교한 e-서명 API는 비즈니스 워크플로를 향상시켜 전자 서명의 서명, 검증, 수정 및 관리 작업을 효율적으로 자동화합니다."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "전자 서명 기능"
  features:
    # feature loop
    - title: "오피스 문서의 전자 서명"
      content: "문서의 원하는 위치에 전자 서명을 원활하게 삽입합니다. 디지털 인증서, 메타데이터, 바코드 또는 시각적 요소로 콘텐츠를 사용자 정의하고 풍부하게 하며 진위성과 보안을 보장합니다."

    # feature loop
    - title: "종합 서명 관리"
      content: "서명된 문서는 후속 처리가 용이합니다. 기존 서명의 전체 개요에 접근하여 필요한 경우 정확하게 서명을 업데이트하거나 삭제할 수 있습니다."

    # feature loop
    - title: "강화된 콘텐츠 보안"
      content: "디지털 인증서를 사용하여 문서의 무결성을 보호합니다. 향상된 문서 추적 및 감사 기능을 위해 메타데이터를 삽입하거나 추출하여 준수 및 콘텐츠의 진위성을 보장합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 이미지 서명 추가하는 방법"
      content: |
        이 예제는 문서의 특정 페이지에 이미지 서명을 적용하는 절차를 설명합니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 소스 문서를 인수로 제공합니다.
          using (Signature signature = new Signature("input.xlsx"))
          {
              // 서명 구성에서 이미지 경로를 지정합니다.
              ImageSignOptions options = new ImageSignOptions("image.jpg")
              {
                  // 서명을 위한 크기 및 대상 페이지를 정의합니다.
                  VerticalAlignment = VerticalAlignment.Bottom,
                  HorizontalAlignment = HorizontalAlignment.Right,
                  Height = 150,
                  Width = 200,
                  Margin = new Padding(50),
                  AllPages = true
              };

              // 서명을 문서에 적용합니다.
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
            link: "/examples/signature/formats/signature_esign.xlsx"
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
    title: "모든 기능을 탐색하세요"
    exclude: "esign"
    description: "다양한 서명 옵션과 관련된 작업을 제공하게 되어 자랑스럽습니다."
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
    title: "다양한 파일 형식에 디지털 서명"
    exclude: "XLSX"
    description: ".NET API는 60개 이상의 산업 표준 파일 형식에 전자 서명을 가능하게 하여 비즈니스 문서를 보호하는 데 뛰어난 유연성을 제공합니다."
    items: 
          
        # format loop 1
        - name: "e-서명 PDF"
          format: "PDF"
          link: "/signature/net/esign/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "e-서명 DOCX"
          format: "DOCX"
          link: "/signature/net/esign/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "e-서명 JPEG"
          format: "JPEG"
          link: "/signature/net/esign/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "e-서명 PPTX"
          format: "PPTX"
          link: "/signature/net/esign/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "e-서명 XLSX"
          format: "XLSX"
          link: "/signature/net/esign/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---