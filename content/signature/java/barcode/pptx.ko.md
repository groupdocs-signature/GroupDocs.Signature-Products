



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:24
draft: false
lang: ko
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java로 PPTX 파일에 바코드 추가하기"
head_description: "Java에서 PPTX 문서에 바코드 서명을 생성하고 삽입합니다. GroupDocs.Signature은 여러 형식에 대해 다양한 서명 통합을 지원합니다."

############################# Header ############################
title: "PPTX용 바코드 생성" 
description: "GroupDocs.Signature for Java을 사용하여 비즈니스 문서의 모든 위치에 인기 있는 형식의 바코드를 추가하세요. 우리의 솔루션은 바코드 서명을 사용자화할 수 있는 광범위한 옵션을 제공합니다."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 소개"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 다양한 서명 유형을 지원하는 고급 서명 솔루션입니다. 텍스트, 이미지, 바코드, 디지털 인증서, 도장 및 기타 형식을 통해 60개 이상의 파일 형식(PDF, MS Office, 이미지, ZIP 파일 및 기타 인기 비즈니스 형식 포함)의 문서에 서명할 수 있습니다. 서명된 문서의 서명은 언제든지 검색, 검증, 수정 또는 삭제할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 파일에 바코드를 생성하고 추가하는 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 다양한 인기 형식의 바코드를 생성하고 PPTX 페이지에 배치할 수 있습니다. 60개 이상의 바코드 유형을 지원하여 Java 애플리케이션에 우리의 라이브러리를 통합하여 바코드 서명 기능을 쉽게 향상시킬 수 있습니다.
      
      1. PPTX 파일 또는 처리할 스트림을 제공합니다.
      2. BarcodeSignOptions 인스턴스에 바코드 텍스트를 전달합니다.
      3. 위치, 크기 등의 바코드 옵션을 사용자화합니다.
      4. 새로 추가된 바코드를 포함하여 파일을 저장합니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "샘플 서명"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "클릭하여 복사"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "문서"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}
        // 문서 경로로 새 Signature 인스턴스를 생성합니다.
        Signature signature = new Signature("input.pptx");

        // BarcodeSignOptions를 사용하여 문서에 바코드를 추가합니다.
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // 바코드 유형 및 기타 속성을 설정합니다.
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // 서명된 파일을 저장합니다.
        signature.sign("output.pptx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "서명으로 문서 내용 강화 또는 보호"
  description: "GroupDocs.Signature for Java 라이브러리는 인기 있는 파일 형식의 서명 및 추가 처리를 위해 설계되었습니다. 다양한 유형의 서명을 신속하게 추가, 수정, 검증 또는 삭제할 수 있습니다."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 기능"
  features:
    # feature loop
    - title: "문서 서명"
      content: "텍스트, 이미지, 바코드, QR 코드 또는 도장으로 지원되는 문서의 모든 페이지에 서명합니다. 이미지에 EXIF와 같은 숨겨진 메타데이터를 추가하거나 디지털 인증서를 사용하여 문서 내용을 무단 변경으로부터 보호할 수 있습니다."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "서명된 문서에서 할 수 있는 일이 많이 있습니다. 모든 것이 제대로 되어 있는지 확인하기 위해 서명 검증을 제공합니다. 또한 검색을 통해 문서의 모든 서명 목록을 가져올 수 있습니다."

    # feature loop
    - title: "서명 수정"
      content: "기존에 추가된 대부분의 서명은 수정이 가능합니다. 텍스트를 수정하거나 위치를 조정하거나 색상을 변경할 수 있습니다."

    # feature loop
    - title: "서명 삭제"
      content: "우리의 솔루션은 서명에 대한 전체 CRUD 작업을 지원합니다. 여러 종류의 서명을 필요에 따라 문서에서 삭제할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "바코드 서명을 생성하는 방법"
      content: |
        이 예시는 PPTX 문서 페이지에 맞춤형 바코드를 배치하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 서명할 문서를 제공합니다.
          Signature signature = new Signature("input.pptx");

          // 원하는 텍스트로 서명 옵션을 생성합니다.
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // 페이지에서 바코드의 상대적 위치를 설정합니다.
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // 페이지 가장자리에서 바코드 패딩을 설정합니다.
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // 막대의 색상을 설정합니다.
          signOptions.setForeColor(Color.RED);

          // 메시지 글꼴 스타일을 정의합니다.
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // 메시지 위치를 지정합니다.
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // 문서에 서명하고 저장합니다.
          SignResult signResult = signature.sign("output.pptx", signOptions);

          ```
        platform: "java"
        copy_title: "복사"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "클릭하여 복사"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/signature/formats/signature_barcode.pptx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Signature의 기능을 무료로 시도하거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "Maven 다운로드"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "라이센스 구매"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "핵심 기능을 알아보세요"
    exclude: "barcode"
    description: "저희는 지원되는 다양한 서명과 기능을 자랑스럽게 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/pptx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/pptx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/pptx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/pptx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/pptx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/pptx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/pptx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/pptx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/pptx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/pptx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/pptx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "기타 형식의 문서 서명"
    exclude: "PPTX"
    description: "저희 Java API를 사용하여 60개 이상의 형식에 서명할 수 있습니다. 문서의 모든 페이지 또는 위치에 다양한 서명을 적용하십시오."
    items: 
          
        # format loop 1
        - name: "PDF에 바코드 추가"
          format: "PDF"
          link: "/signature/java/barcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 바코드 추가"
          format: "DOCX"
          link: "/signature/java/barcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG에 바코드 추가"
          format: "JPEG"
          link: "/signature/java/barcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX에 바코드 추가"
          format: "PPTX"
          link: "/signature/java/barcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX에 바코드 추가"
          format: "XLSX"
          link: "/signature/java/barcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---