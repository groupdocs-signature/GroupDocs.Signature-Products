



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python를 사용하여 XLSX 파일용 QR 코드 생성"
head_description: "GroupDocs.Signature API를 사용하여 XLSX 파일에 QR 코드를 생성하고 삽입하세요. QR 코드를 모든 페이지에 배치하여 추가 기능을 더할 수 있습니다."

############################# Header ############################
title: "XLSX용 QR 코드 생성" 
description: "텍스트 또는 숫자 데이터를 사용하여 2D 바코드를 간편하게 생성하고, PDFs, Word, Excel 등 다양한 페이지 및 형식에 적용할 수 있는 GroupDocs.Signature for Python via .NET입니다."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET의 기능 탐색"
    link: "/signature/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)는 다양한 서명 유형을 생성하고 삽입할 수 있는 광범위한 기능을 제공합니다. PDF, Word, Excel, PowerPoint 또는 이미지와 같은 주요 문서 형식에서 텍스트, 이미지, 바코드, QR 코드, 메타데이터, 디지털 또는 스탬프 서명으로 문서를 향상시킬 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX에 QR 코드를 생성하고 삽입하는 단계"
    content: |
      [GroupDocs.Signature](/signature/python-net/)는 인기 있는 형식의 QR 코드를 생성하고 XLSX 페이지에 배치할 수 있게 해줍니다. 10종 이상의 QR 코드 유형을 지원하여 이 기능을 Python via .NET 애플리케이션에 원활하게 통합할 수 있습니다. 우리의 제품을 사용하여 QR 코드 서명으로 문서를 향상하세요.
      
      1. XLSX 파일 또는 QR 코드가 추가될 스트림을 획득하세요.
      2. QrCodeSignOptions에 필요한 텍스트를 제공하세요.
      3. 색상, 위치 및 크기와 같은 시각적 설정을 사용자 정의하세요.
      4. QR 코드가 삽입된 문서를 저장하세요.
   
    code:
      platform: "python-net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # 문서와 함께 새 Signature 인스턴스 초기화
            with sg.Signature('input.xlsx') as signature:

                # QrCodeSignOptions를 사용하여 문서에 QR 코드 삽입
                options = sg.QrCodeSignOptions("Text Content")

                # 서명 유형을 지정하고 페이지에서의 위치 설정
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # QR 코드가 삽입된 문서 저장
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서에 대한 완전한 서명 통합"
  description: "GroupDocs.Signature for Python via .NET API를 사용하면 다양한 서명 유형을 생성, 수정, 검색, 검증 및 제거할 수 있어 문서 워크플로를 정밀하게 간소화합니다."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "다양한 서명 유형 적용"
      content: "GroupDocs.Signature는 텍스트, 이미지, 바코드, QR 코드, 스탬프 서명을 모든 문서에 적용할 수 있습니다. 원하는 페이지에 서명을 정확하게 배치하고 메타데이터를 쉽게 관리할 수 있습니다. 디지털 인증서로 문서를 무단 변경으로부터 보호하세요."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "고급 검증 도구를 사용하여 문서 서명의 진위와 정확성을 확인하세요. 문서에 삽입된 모든 서명의 상세 목록을 쉽게 얻어 더 나은 감독이 가능합니다."

    # feature loop
    - title: "기존 서명 수정"
      content: "특정 요구 사항에 맞게 콘텐츠, 위치, 색상, 크기 및 기타 속성을 조정하여 이전에 적용된 서명을 업데이트할 수 있습니다."

    # feature loop
    - title: "서명 쉽게 제거"
      content: "원하는 서명을 신속하게 제거하여 문서 관리를 간소화하세요. 디지털 인증서 또는 다른 서명 유형이든지 간편하게 제거할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "생성된 QR 코드 사용자 정의"
      content: |
        이 예제는 XLSX 페이지에 사용자 정의된 QR 코드를 배치하는 방법을 보여줍니다.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 서명할 문서를 가져오고 Signature에 전달
              with sg.Signature('input.xlsx') as signature:

                    # 필요한 텍스트로 QR 코드 옵션 구성
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # 페이지에서 QR 코드의 위치 설정
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # 서명의 패딩 설정
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # QR 코드의 색상 선택
                    options.ForeColor = sg.Color.Red

                    # 메시지의 글꼴 옵션 정의
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # QR 코드의 배경색과 브러시 설정
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # 문서에 QR 코드 삽입
                    result = signature.Sign("output.xlsx", options)
          ```
        platform: "python-net"
        copy_title: "복사"
        install:
          command: "pip install groupdocs-signature-net"
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "PyPi 다운로드"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "우리의 서명 솔루션 탐색"
    exclude: "qrcode"
    description: "문서 요구 사항을 충족하기 위해 다양한 서명 유형과 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 문서 형식에 QR 코드 삽입"
    exclude: "XLSX"
    description: "Python via .NET API를 사용하여 산업 표준 문서 형식에 QR 코드를 삽입하세요. 중요한 정보를 2D 바코드로 저장 및 인코딩하여 간편하게 스캔하고 데이터 검색을 할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF용 QR 코드"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX용 QR 코드"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG용 QR 코드"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX용 QR 코드"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX용 QR 코드"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---