



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: ko
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript를 사용하여 DOCX에 텍스트 서명 추가하기"
head_description: "JavaScript API를 활용하여 DOCX 문서에 텍스트 서명을 원활하게 통합하십시오. 우리의 API는 PDF, Word, Excel, 프레젠테이션, 이미지 및 ZIP 파일을 포함한 다양한 형식을 지원합니다."

############################# Header ############################
title: "DOCX에 텍스트 서명 추가하기" 
description: "GroupDocs.Signature for Node.js via Java를 사용하여 비즈니스 파일에 개인화된 텍스트 서명을 통합하십시오. 안전하고 사용자 정의 가능한 서명 옵션으로 문서 워크플로를 제어하십시오."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험 시작"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java 소개"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 문서에 텍스트 서명을 추가하는 것을 용이하게 하도록 설계된 혁신적인 솔루션입니다. 서명을 사용자 정의하고 페이지 어디에나 배치하여 문서 처리의 효율성을 향상시킬 수 있습니다. 개인화된 텍스트 마크를 통합하여 조직의 워크플로를 간소화하고 기능성과 전문성을 강화하십시오.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript를 사용한 DOCX용 텍스트 서명 생성 가이드"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 Node.js via Java 애플리케이션 내의 DOCX 문서에 텍스트 서명을 추가할 수 있게 합니다. 우리의 강력한 솔루션으로 제품의 기능을 신속하게 확장하십시오.
      
      1. Signature 클래스에 DOCX 문서를 인수로 제공합니다.
      2. 필요한 텍스트로 TextSignOptions를 인스턴스화합니다.
      3. 텍스트 서명의 시각적 속성을 설정합니다.
      4. 문서의 원하는 페이지에 텍스트 서명을 추가합니다.
   
    code:
      platform: "nodejs-java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Signature 클래스를 문서 경로와 함께 초기화합니다.
        const signature = new signatureLib.Signature('input.docx');

        // 필요한 서명 텍스트로 TextSignOptions를 생성합니다.
        const options = new signatureLib.TextSignOptions('Approved');

        // 텍스트 색상 및 글꼴 속성을 구성합니다.
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // 문서에 텍스트 서명을 추가합니다.
        const result = signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "강화된 텍스트 서명 제어"
  description: "GroupDocs.Signature for Node.js via Java를 사용하여 주요 문서 형식에서 텍스트 기반 서명의 관리를 크게 향상시킬 수 있습니다. 이 도구는 서명의 스타일, 위치 및 내용을 구성할 수 있도록 하여 기업이 문서 프로세스를 맞춤화할 수 있게 합니다."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 핵심 기능"
  features:
    # feature loop
    - title: "동적 문서 서명"
      content: "텍스트, 이미지, 바코드, QR 코드 또는 도장과 같은 다양한 유형의 서명을 지원 문서의 모든 페이지에 삽입할 수 있습니다. 숨겨진 정보를 표현하기 위한 메타데이터를 포함하거나 고급 보안 조치를 위한 디지털 인증서를 적용할 수 있습니다."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "문서에 내장된 서명의 진품성을 확인하십시오. 모든 서명 인스턴스를 찾기 위한 효율적인 검색을 수행함으로써 철저한 문서 추적 및 관리가 가능합니다."

    # feature loop
    - title: "서명 수정 또는 제거"
      content: "필요에 따라 이전에 추가한 서명을 수정하거나 삭제할 수 있습니다. 진화하는 요구 사항에 맞게 서명의 외관, 위치 또는 내용을 조정하여 문서 처리의 유연성을 보장합니다."

    # feature loop
    - title: "네이티브 서명 사용자 정의"
      content: "특정 파일 형식에 대해 문서 기능을 사용하여 서명 배치를 조정할 수 있습니다. 예를 들어 Word 파일에 워터마크를 추가하거나 PDF에 사용자 정의된 스탬프를 추가하여 문서의 독창성을 향상시킬 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 텍스트 서명 구현하기"
      content: |
        비즈니스 문서에 텍스트 서명을 삽입하는 방법을 배워 프로세스를 최적화하십시오.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 서명할 문서를 선택합니다.
          const signature = new signatureLib.Signature('input.docx');

          // 지정된 내용을 포함한 텍스트 옵션을 정의합니다.
          const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

          // 서명의 크기와 페이지에서의 위치를 설정합니다.
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // 서명이 페이지 가장자리에서 패딩을 적용하도록 설정합니다.
          const padding = new signatureLib.Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // 텍스트 색상과 글꼴 스타일을 사용자 정의합니다.
          options.setForeColor(signatureLib.Color.RED);
          const signatureFont = new signatureLib.SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName('Comic Sans MS');
          options.setFont(signatureFont);

          // 원하는 경우 텍스트 서명에 테두리를 추가합니다.
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // 서명의 배경을 구성합니다.
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // 옵션으로 호환성을 위해 텍스트를 이미지로 저장합니다.
          options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
          
          // 추가된 텍스트 서명과 함께 문서를 저장합니다.
          const result = signature.sign('output.docx', options);
          ```
        platform: "nodejs-java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_text.docx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "NPM 다운로드"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "포괄적인 서명 관리 기능"
    exclude: "text"
    description: "우리의 플랫폼은 7가지 고유 서명 유형의 전체 CRUD 작업 및 고급 기능을 제공하여 문서 서명을 정밀하고 용이하게 관리할 수 있습니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/docx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/docx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/docx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/docx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/nodejs-java/search/docx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/nodejs-java/verify/docx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/nodejs-java/modify/docx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/nodejs-java/delete/docx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 형식에 텍스트 서명 적용하기"
    exclude: "DOCX"
    description: "Node.js via Java API의 기능을 활용하여 다양한 Office 형식에 텍스트 기반 서명을 통합하십시오. 문서 생애 주기의 모든 단계에서 정보 흐름을 제어하며 강력하게 사용자 정의할 수 있는 텍스트 마크를 추가하십시오."
    items: 
          
        # format loop 1
        - name: "PDF 텍스트 서명"
          format: "PDF"
          link: "/signature/nodejs-java/text/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 텍스트 서명"
          format: "DOCX"
          link: "/signature/nodejs-java/text/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG 텍스트 서명"
          format: "JPEG"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX 텍스트 서명"
          format: "PPTX"
          link: "/signature/nodejs-java/text/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX 텍스트 서명"
          format: "XLSX"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---