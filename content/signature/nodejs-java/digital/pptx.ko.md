



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:59
draft: false
lang: ko
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "JavaScript를 사용하여 PPTX 파일에 전자 서명 추가하기"
head_description: "JavaScript를 사용하여 PPTX 파일에 디지털 서명을 몇 줄의 코드로 추가하세요. 여러 파일 형식에 서명하기 위해 GroupDocs.Signature for Node.js via Java을(를) 사용하세요."

############################# Header ############################
title: "PPTX를 디지털 인증서로 보호하십시오" 
description: "GroupDocs.Signature for Node.js via Java의 고급 기능을 사용하여 비즈니스 문서의 보안을 확보하십시오. 문서를 보호하고 인증하는 유연한 옵션을 제공합니다."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Node.js via Java에 대해"
    link: "/signature/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/)은 다양한 문서 처리 요구 사항을 처리하기 위해 설계된 포괄적인 서명 솔루션입니다. PDF, MS Office, 이미지, ZIP 파일 등 60개 이상의 파일 형식에 텍스트, 이미지, 디지털 인증서 및 봉투를 통합할 수 있습니다. 또한 서명된 문서는 필요에 따라 쉽게 검색, 검증, 수정 또는 삭제할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "JavaScript에서 디지털 인증서를 사용하여 PPTX 보안 가이드라인"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/)는 Node.js via Java 개발자가 디지털 서명을 사용하여 PPTX 문서의 수정으로부터 보호할 수 있도록 합니다. 포괄적인 데이터 보안 기능으로 비즈니스 애플리케이션을 향상시키십시오.
      
      1. Signature 클래스 생성자에 PPTX 문서를 전달합니다.
      2. 문서를 보호하기 위해 디지털 인증서 및 해당 비밀번호를 적용합니다.
      3. 선택적으로 문서 페이지에 디지털 서명의 시각적 표현을 추가합니다.
      4. 문서를 서명하여 향후 변경을 방지합니다.
   
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

        // Signature를 사용하여 문서에 디지털 서명을 적용합니다.
        const signature = new signatureLib.Signature('input.pptx');

        // 필요한 디지털 인증서 및 비밀번호를 제공하십시오.
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 필요한 경우 시각적 서명 설정을 구성하십시오.
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // 디지털 인증서를 사용하여 문서를 암호화하십시오.
        const result = signature.sign('output.pptx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "서명을 통해 문서 콘텐츠 최적화 또는 보호"
  description: "GroupDocs.Signature for Node.js via Java는 모든 주요 파일 형식에 서명하도록 설계되어 다양한 유형의 서명을 추가, 조정, 검증 또는 제거할 수 있는 기능을 제공합니다."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "문서에 서명 추가하기"
      content: "지원되는 문서의 모든 페이지에 텍스트, 이미지, 바코드, QR 코드 또는 스탬프 서명을 쉽게 추가할 수 있습니다. 또한 이미지의 EXIF와 같은 숨겨진 메타데이터를 삽입하거나 수정할 수 있습니다. 디지털 인증서를 통해 문서 내용을 무단 변경으로부터 보호하십시오."

    # feature loop
    - title: "서명 찾기 및 검증하기"
      content: "서명 후 문서는 여러 차례 검증을 받을 수 있습니다. 서명된 콘텐츠의 무결성을 확인하거나 모든 기존 서명을 나열하기 위한 세부 검색을 수행하십시오."

    # feature loop
    - title: "기존 서명 수정하기"
      content: "대부분의 서명 유형은 생성 후 수정이 가능합니다. 텍스트 수정, 요소 재배치, 색상 조정, 크기 조정 및 기타 필요한 변경을 쉽게 수행할 수 있습니다."

    # feature loop
    - title: "불필요한 서명 제거하기"
      content: "우리의 솔루션은 서명에 대한 전체 CRUD 작업을 지원합니다. 필요한 경우, 문서에서 다양한 서명 유형, 디지털 인증서를 포함하여 제거할 수 있습니다."
      
  code_samples:
    # code sample loop
    - title: "디지털 서명으로 문서 보호하기"
      content: |
        디지털 서명을 사용하여 문서를 변경할 수 없도록 하는 방법을 배우십시오.
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // 서명이 필요한 문서를 제공합니다.
        const signature = new signatureLib.Signature('input.pptx');

        // 적절한 디지털 인증서와 비밀번호를 사용하십시오.
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // 필요한 추가 텍스트 정보를 포함하십시오.
        options.setReason('Security issue');
        options.setContact('John Smith');
        options.setLocation('Office D.W.');

        // 서명 표현을 위한 이미지와 같은 시각적 요소를 추가하십시오.
        options.setImageFilePath('image.png');
        options.setAllPages(true);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setWidth(80);
        options.setHeight(60);

        const padding = new signatureLib.Padding();
        padding.setBottom(10);
        padding.setRight(10);
        options.setMargin(padding);
        
        // 디지털로 안전하게 된 문서를 지정된 위치에 저장하십시오.
        const result = signature.sign('output.pptx', options);
        ```
        {{< /landing/code >}}


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
    title: "주요 기능 알아보기"
    exclude: "digital"
    description: "우리는 포괄적인 서명 옵션 및 기능 세트를 자랑스럽게 지원합니다."
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
    title: "다양한 형식의 문서 서명하기"
    exclude: "PPTX"
    description: "Node.js via Java API는 60개 이상의 형식을 지원하여 문서의 어떤 페이지에서든 서명을 적용하고, 디지털 인증서로 콘텐츠 보안을 유지하며, 문서 내 서명을 효과적으로 관리할 수 있도록 합니다."
    items: 
          
        # format loop 1
        - name: "PDF 보호"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 보호"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "PPTX 보호"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 4
        - name: "XLSX 보호"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---