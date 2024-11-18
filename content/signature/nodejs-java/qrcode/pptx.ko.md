



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:02
draft: false
lang: ko
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PPTX 문서에서 JavaScript로 QR 코드 생성하기"
head_description: "GroupDocs.Signature API를 활용하여 PPTX 파일 내에 2D 바코드를 생성하고 통합하세요. 모든 문서 페이지에 QR 코드를 간편하게 배치할 수 있습니다."

############################# Header ############################
title: "PPTX용 QR 코드 만들기" 
description: "GroupDocs.Signature for Node.js via Java을 사용하여 PDF, Word, Excel, 이미지 등 다양한 문서 형식에 텍스트 및 숫자 데이터를 포함한 사용자 지정 콘텐츠로 2D 바코드를 생성하고 삽입하세요."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험하기"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java의 기능 탐색"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 인기 파일 형식에 QR 코드를 포함한 다양한 서명 유형을 생성하고 삽입할 수 있는 고급 문서 개선 도구를 제공합니다. 텍스트, 이미지, 바코드, QR 코드, 메타데이터, 디지털 및 스탬프 서명을 통해 PDF, Word 문서, Excel 스프레드시트, PowerPoint 프레젠테이션 및 이미지를 서명하고 보호하세요.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 내의 어느 위치에나 QR 코드를 생성하고 삽입하는 방법"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 다양한 널리 사용되는 형식에서 QR 코드를 생성하고 이를 PPTX 페이지에 통합할 수 있도록 지원합니다. 10가지 이상의 QR 코드 유형을 지원하는 당사의 솔루션은 Node.js via Java 응용 프로그램에 문제없이 통합되어 QR 코드 서명 기능을 색칠합니다.
      
      1. QR 코드 서명을 위한 PPTX 파일 또는 스트림을 제공합니다.
      2. 원하는 텍스트를 QrCodeSignOptions 인스턴스에 입력합니다.
      3. 색상, 위치, 크기 등의 시각적 설정을 조정합니다.
      4. QR 코드가 포함된 문서를 저장합니다.
   
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

        // Signature 인스턴스를 생성하고 문서 경로를 전달합니다.
        const signature = new signatureLib.Signature('input.pptx');

        // QrCodeSignOptions를 활용하여 QR 코드를 문서에 삽입합니다.
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // 서명 유형과 페이지에서의 위치를 정의합니다.
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // 새로 추가된 QR 코드가 포함된 문서를 저장합니다.
        signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "종합적인 서명 및 QR 코드 통합"
  description: "GroupDocs.Signature for Node.js via Java API를 통해 모든 종류의 서명을 관리할 수 있습니다. 다양한 문서 형식에 걸쳐 서명을 효율적으로 생성, 사용자 지정, 검증, 검색 및 제거할 수 있어 귀하의 작업 흐름에 특별한 유연성을 제공합니다."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "서명 및 QR 코드 기능"
  features:
    # feature loop
    - title: "다양한 형식 문서 서명"
      content: "지원되는 모든 문서 형식에 텍스트, 이미지, 바코드, QR 코드 및 스탬프 서명을 포함한 여러 유형의 서명을 추가하세요. 문서의 모든 페이지에 서명을 배치하고 문서 메타데이터를 관리합니다. 디지털 인증서를 통해 문서 보안을 보장하여 무단 변경을 방지합니다."

    # feature loop
    - title: "효율적인 서명 검증"
      content: "서명이 표준을 준수하는지 확인하기 위해 문서 내 모든 서명을 검증합니다. 내장된 검색 기능을 통해 서명을 쉽게 검색하고 검토할 수 있습니다."

    # feature loop
    - title: "유연한 서명 편집"
      content: "기존 서명을 업데이트하거나 수정하여 내용, 위치, 크기 및 색상 등을 문서의 요구에 맞게 조정할 수 있습니다."

    # feature loop
    - title: "서명 제거 간편화"
      content: "불필요하거나 오래된 서명(디지털 인증서 포함)을 간편하게 제거하세요. 서명을 관리하는 모든 권한을 통해 깔끔하고 정돈된 문서를 보장합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "생성된 QR 코드 사용자 지정"
      content: |
        이 예제는 PPTX 페이지에 사용자 지정 QR 코드를 추가하는 과정을 자세히 설명합니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 서명할 문서를 가져와 Signature에 전달합니다.
          const signature = new signatureLib.Signature('input.pptx');

          // 필요한 텍스트로 QR 코드 옵션을 설정합니다.
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // 페이지에서 QR 코드의 위치를 결정합니다.
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // 서명 여백을 지정합니다.
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // QR 코드 색상을 선택합니다.
          signOptions.setForeColor(signatureLib.Color.RED);

          // 동반 메시지에 대한 글꼴 옵션을 정의합니다.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // QR 코드의 배경 색상 및 브러쉬를 사용자 지정합니다.
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // 문서에 QR 코드를 삽입합니다.
          signature.sign('output.pptx', signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.pptx"
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
    title: "우리의 주요 기능 이해하기"
    exclude: "qrcode"
    description: "귀하의 요구에 맞게 조정된 폭넓은 서명 형식과 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/pptx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/pptx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/nodejs-java/search/pptx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pptx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pptx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 파일 형식과 QR 코드 통합"
    exclude: "PPTX"
    description: "Node.js via Java API를 활용하여 QR 코드를 생성하고 다양한 널리 사용되는 파일 형식에 삽입하세요. 이 바코드에 중요한 데이터를 캡슐화하여 원활한 통합 및 미래의 탐색을 가능하게 합니다."
    items: 
          
        # format loop 1
        - name: "PDF용 QR 코드"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX용 QR 코드"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG용 QR 코드"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX용 QR 코드"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX용 QR 코드"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---