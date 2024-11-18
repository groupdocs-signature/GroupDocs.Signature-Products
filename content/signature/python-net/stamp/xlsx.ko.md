



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Python를 사용하여 XLSX에서 원형 및 사각 스탬프 만들기"
head_description: "GroupDocs.Signature for Python via .NET API를 사용하여 XLSX 파일에 개인화된 스탬프를 생성하고 삽입하세요."

############################# Header ############################
title: "XLSX용 스탬프 만들기" 
description: "GroupDocs.Signature for Python via .NET을(를) 사용하여 문서의 어떤 부분에든 맞춤 설계된 스탬프를 추가하여 비즈니스 요구 사항을 충족하는 유연한 배치 및 구성을 제공합니다."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Python via .NET 개요"
    link: "/signature/python-net/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/)은(는) 문서에 다양한 서명 유형을 삽입할 수 있는 포괄적인 도구로, 맞춤형 스탬프도 포함됩니다. PDF 및 Word 문서에서 이미지와 ZIP 파일에 이르기까지 60개 이상의 파일 형식을 지원하여 텍스트, 이미지, 바코드, 메타데이터, 디지털 인증서 및 스탬프를 사용해 문서를 강화할 수 있습니다. 또한 적용된 서명을 검색, 확인, 편집 또는 삭제할 수 있는 전체 제어 권한을 제공합니다.

############################# Steps ############################
steps:
    enable: true
    title: "Python를 사용하여 XLSX에 스탬프 추가하기"
    content: |
      [GroupDocs.Signature](/signature/python-net/)는({는}) Python via .NET 애플리케이션을 개선하기 위해 강력한 스탬프 생성 도구를 제공합니다. 이를 사용하여 문서 페이지에 맞춤형 스탬프를 설계하고 구현하세요.
      
      1. XLSX 문서를 제공하세요.
      2. StampSignOptions를 사용하여 모든 필요한 설정을 구성합니다.
      3. 필요한 경우 여러 스탬프 줄을 추가합니다.
      4. 스탬프를 적용하고 업데이트된 문서를 저장하세요.
   
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

            # Signature 인스턴스에 문서 경로 첨부
            with sg.Signature('input.xlsx') as signature:

                # 필요한 스탬프 세부정보로 StampSignOptions 설정
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # 스탬프에 한 줄 또는 여러 줄 추가
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # 적용된 스탬프와 함께 문서 저장
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "서명을 사용하여 문서 보안 및 무결성 향상"
  description: "GroupDocs.Signature for Python via .NET 라이브러리를 사용하면 문서에 서명 기능을 원활하게 추가할 수 있습니다. 맞춤형 스탬프 및 기타 서명 유형을 쉽게 생성, 수정, 확인 또는 삭제함으로써 문서 워크플로우에 대한 유연성과 보안을 제공합니다."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signature에서 제공하는 스탬프 서명"
  features:
    # feature loop
    - title: "완전한 문서 서명"
      content: "텍스트, 이미지, 바코드, QR 코드 및 스탬프와 같은 서명을 문서의 어떤 페이지든 원하는 위치에 추가하여 문서를 강화하세요. 임베디드 메타데이터를 관리하고 디지털 인증서를 적용하여 무단 변경으로부터 보호합니다."

    # feature loop
    - title: "효율적인 서명 검색 및 확인"
      content: "서명이 완료된 후 고급 검색 도구를 사용하여 모든 임베디드 서명을 찾아보세요. 문서의 무결성을 보장하기 위해 서명 데이터를 쉽게 확인하거나 관리할 수 있습니다."

    # feature loop
    - title: "서명 편집 및 맞춤화"
      content: "이전에 추가된 서명을 자유롭게 변경하세요. 내용, 위치, 크기 또는 색상을 변경하고자 할 경우, GroupDocs.Signature for Python via .NET를 사용하면 서명을 필요에 따라 조정할 수 있는 전체 제어 권한을 제공합니다."

    # feature loop
    - title: "서명 쉽게 제거"
      content: "서명을 제거해야 하는 경우, GroupDocs.Signature for Python via .NET은 스탬프 및 디지털 인증서를 포함하여 모든 유형을 삭제할 수 있는 도구를 제공합니다. 이를 통해 문서를 최신 상태로 유지하고 규정을 준수할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 맞춤형 스탬프 추가하는 방법"
      content: |
        이 예에서는 특정 텍스트 세부정보가 포함된 맞춤형 스탬프를 생성하고 문서에 삽입하는 방법을 보여줍니다.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # 스탬프할 문서를 제공하세요
              with sg.Signature('input.xlsx') as signature:

                    # 원하는 설정으로 스탬프 옵션을 설정합니다
                    options = sg.StampSignOptions()

                    # 페이지에 스탬프의 크기와 배치를 정의합니다
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # 텍스트가 포함된 외부 원형 선 추가
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # 선택적으로 내부 사각형 선 추가
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # 스탬프가 적용된 문서를 최종화하고 저장합니다
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
            link: "/examples/signature/formats/signature_stamp.xlsx"
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
    title: "주요 기능 탐색"
    exclude: "stamp"
    description: "서명의 생성, 관리 및 제거를 위한 다양한 옵션을 찾아보고, 문서 워크플로우에 대한 전체 제어 권한을 부여받으세요."
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
    title: "다양한 문서 형식에 스탬프 적용"
    exclude: "XLSX"
    description: "GroupDocs.Signature API를 사용하면 60개 이상의 표준 파일 형식에 사용자 정의 스탬프를 삽입할 수 있습니다. 문서의 어디에나 스탬프를 쉽게 적용하여 개인화 및 추적을 개선할 수 있습니다."
    items: 
          
        # format loop 1
        - name: "PDF에 도장"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 도장"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG에 도장"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX에 도장"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX에 도장"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---