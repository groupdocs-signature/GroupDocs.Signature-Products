



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:26
draft: false
lang: ko
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JPEG용 바코드 생성 및 추가하기 JavaScript 응용 프로그램 사용"
head_description: "JavaScript를 사용하여 몇 줄의 코드로 JPEG 문서에 바코드 서명을 신속하게 생성하고 삽입하세요. GroupDocs.Signature는 여러 파일 형식을 지원합니다."

############################# Header ############################
title: "JPEG에 바코드를 손쉽게 생성하고 추가하기" 
description: "GroupDocs.Signature for Node.js via Java를 사용하여 비즈니스 문서에 바코드를 통합하고 필요한 정확한 위치에 배치하세요. 우리의 솔루션은 바코드 서명을 당신의 요구에 맞게 조정할 수 있는 광범위한 커스터마이징 옵션을 제공합니다."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "지금 다운로드 - 무료입니다!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java 소개"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)는 텍스트, 이미지, 바코드, 디지털 인증서 및 스탬프를 포함한 다양한 서명 유형을 지원하는 강력한 문서 서명 도구입니다. PDF, MS Office 파일, 이미지 및 ZIP 아카이브 등 60개 이상의 파일 형식과의 호환성을 제공하여 포괄적인 문서 관리가 가능합니다. 문서 내 서명은 필요에 따라 검색, 검증, 수정 또는 제거할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "JPEG 파일에 바코드를 생성하고 삽입하는 방법"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 JPEG 페이지에서 다양한 인기 형식의 바코드를 생성하고 배치할 수 있도록 지원합니다. 60개 이상의 바코드 유형을 지원하는 Node.js via Java 응용 프로그램은 우리의 라이브러리를 통합하여 바코드 서명 기능을 쉽게 향상할 수 있습니다.
      
      1. JPEG 파일 또는 스트림을 제공하여 처리합니다.
      2. 바코드 텍스트를 BarcodeSignOptions 인스턴스에 전달합니다.
      3. 위치, 크기 등의 바코드 설정을 조정합니다.
      4. 새로 추가된 바코드와 함께 문서를 저장합니다.
   
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

        // 문서 경로로 Signature 객체를 인스턴스화 합니다.
        const signature = new signatureLib.Signature('input.jpeg');

        // BarcodeSignOptions를 사용하여 문서에 바코드를 통합합니다.
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // 바코드 유형 및 추가 매개변수를 설정합니다.
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // 서명된 문서를 저장합니다.
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 서명 옵션으로 문서를 보강하고 보호하세요"
  description: "GroupDocs.Signature for Node.js via Java 라이브러리는 인기 있는 문서 형식의 서명 및 관리를 간소화하도록 설계되었습니다. 다양한 서명을 빠르고 손쉽게 추가, 수정, 검증 또는 제거할 수 있습니다."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "동적 문서 서명"
      content: "텍스트, 이미지, 바코드, QR 코드 및 스탬프를 포함한 다양한 서명 유형을 사용하여 문서의 모든 페이지에 서명하세요. 또한, 이미지에 EXIF 데이터와 같은 숨겨진 메타데이터를 포함하거나 디지털 인증서를 사용해 문서를 무단 수정으로부터 보호할 수 있습니다."

    # feature loop
    - title: "강력한 서명 검증 및 검색"
      content: "우리의 솔루션은 서명된 문서를 관리하는 광범위한 도구를 제공합니다. 문서의 무결성을 보장하기 위해 서명의 진위를 검증하고, 문서 내에 삽입된 모든 서명을 나열하기 위해 검색 기능을 사용하세요."

    # feature loop
    - title: "서명 수정"
      content: "대부분의 이전에 추가된 서명은 쉽게 수정할 수 있습니다. 텍스트를 업데이트하거나, 위치를 재조정하거나, 필요에 맞게 서명의 외관을 변경하세요."

    # feature loop
    - title: "간편한 서명 제거"
      content: "CRUD 작업에 대한 포괄적인 지원으로, 우리의 도구는 문서에서 서명을 효율적으로 제거할 수 있으며, 가장 관련성 있는 서명만 남기게 해줍니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명 적용 방법"
      content: |
        이 예시는 JPEG 문서 페이지에 사용자 정의 바코드를 삽입하는 방법을 설명합니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // 서명할 문서를 제공합니다.
          const signature = new signatureLib.Signature('input.jpeg');

          // BarcodeSignOptions를 사용하여 문서에 바코드를 통합합니다.
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // 바코드 유형 및 추가 매개변수를 설정합니다.
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // 페이지 경계로부터 바코드 여백을 정의합니다.
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // 바 색상을 선택합니다.
          signOptions.setForeColor(signatureLib.Color.RED);

          // 메시지에 대한 글꼴 스타일을 지정합니다.
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // 메시지의 위치를 표시합니다.
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // 서명하고 문서를 저장합니다.
          signature.sign('output.jpeg', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.jpeg"
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
    title: "주요 기능을 살펴보세요"
    exclude: "barcode"
    description: "우리가 제공하는 다양한 서명 유형 및 도구를 경험해보세요"
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 문서 형식으로 서명하기"
    exclude: "JPEG"
    description: "Node.js via Java API는 60개 이상의 다양한 형식에 서명할 수 있는 기능을 제공합니다. 특정 페이지에 서명을 추가하거나 정확한 위치에 배치하는 것이 쉽습니다."
    items: 
          
        # format loop 1
        - name: "PDF에 바코드 추가"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 바코드 추가"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG에 바코드 추가"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX에 바코드 추가"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX에 바코드 추가"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---