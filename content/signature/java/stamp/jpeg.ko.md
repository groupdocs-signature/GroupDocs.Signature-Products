



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:46
draft: false
lang: ko
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java를 사용하여 JPEG에 스탬프 추가"
head_description: "GroupDocs.Signature와 Java를 활용하여 맞춤형 스탬프를 생성하고 JPEG 문서의 어느 페이지에나 배치하세요."

############################# Header ############################
title: "JPEG에 맞춤형 스탬프 추가" 
description: "GroupDocs.Signature for Java를 사용하여 고리 또는 사각형 스탬프를 문서의 모든 섹션에 디자인하고 적용하세요. 우리의 솔루션은 모든 비즈니스 요구를 충족할 수 있는 광범위한 사용자 정의 옵션을 제공합니다."
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
    title: "GroupDocs.Signature for Java에 대해"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 문서에 다양한 스탬프 서명을 추가할 수 있는 강력한 도구입니다. PDF, Word, Excel, 이미지, ZIP 파일 등 60개 이상의 다양한 파일 형식을 지원합니다. 텍스트, 이미지, 바코드, 메타데이터, 디지털 인증서 및 스탬프 서명을 적용할 수 있습니다. 서명을 추가하는 것 외에도 이를 검색, 검증, 수정 및 제거할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java를 통해 JPEG에 스탬프를 추가하는 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 Java 애플리케이션에 유용한 스탬프 생성기를 제공합니다. 이를 활용하여 문서 페이지에 잘 사용자 지정된 스탬프를 생성하세요.
      
      1. JPEG 문서를 제공하세요.
      2. StampSignOptions를 사용하여 모든 필요한 매개변수를 구성하세요.
      3. 필요한 만큼의 라인을 추가하세요.
      4. 스탬프를 적용하고 문서를 저장하세요.
   
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
        // Signature 객체와 함께 문서 경로 사용
        Signature signature = new Signature("input.jpeg");

        // 원하는 서명 텍스트로 StampSignOptions 인스턴스화
        StampSignOptions options = new StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // 하나 이상의 스탬프 라인 추가
        StampLine outerLine = new StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(Color.WHITE);
        outerLine.setBackgroundColor(Color.BLUE);
        options.getOuterLines().add(outerLine);

        // 스탬프가 추가된 문서 저장
        SignResult result = signature.sign("output.jpeg", options);
        ```        

############################# More features ############################
more_features:
  enable: true
  title: "서명으로 문서 내용 보호"
  description: "GroupDocs.Signature for Java 라이브러리는 인기 있는 파일 형식에서 서명을 관리하고 서명하는 데 적합하게 설계되었습니다. 스탬프 및 기타 유형의 서명을 쉽게 추가, 수정, 검증 또는 제거할 수 있습니다."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "GroupDocs.Signature를 사용한 스탬프 서명"
  features:
    # feature loop
    - title: "문서에 서명하기"
      content: "문서의 어느 부분에든 사용자 정의 가능한 서명을 적용하세요. 텍스트, 이미지, 바코드, QR 코드 및 스탬프를 포함한 다양한 서명 유형 중에서 선택할 수 있습니다. 추가로, 문서 보안을 향상시키기 위해 숨겨진 메타데이터를 추가하거나 수정할 수 있습니다."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "문서에 서명된 후, 우리의 검증 도구를 사용하여 서명 내용이 유효한지 확인하세요. 추가 처리를 위해 모든 서명의 목록을 검색하고 검색할 수 있습니다."

    # feature loop
    - title: "필요에 따라 서명 업데이트"
      content: "문서에 적용된 다양한 서명을 쉽게 수정하세요. 크기, 색상, 위치, 내용 등과 같은 속성을 업데이트할 수 있습니다."

    # feature loop
    - title: "서명 제거"
      content: "문서에서 서명을 제거해야 하나요? 우리의 API는 서명 삭제를 완전히 지원하므로 문서를 효과적으로 관리할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "특별 서명을 사용하여 문서에 맞춤형 스탬프 추가"
      content: |
        중요한 텍스트 정보를 포함한 맞춤형 스탬프를 생성하여 문서에 추가하는 방법을 알아보세요.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 스탬프할 문서를 제공하세요
          Signature signature = new Signature("input.jpeg");

          // 스탬프 옵션 객체를 인스턴스화하세요
          StampSignOptions options = new StampSignOptions();

          // 페이지에서 크기 및 위치를 설정하세요
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(VerticalAlignment.Bottom);
          options.setHorizontalAlignment(HorizontalAlignment.Right);
          options.setAllPages(true);

          // 텍스트와 함께 외부 원형 라인을 하나 이상 추가하세요
          StampLine outerLine1 = new StampLine();
          outerLine1.setText("* The best  choice *");
          outerLine1.setTextRepeatType(StampTextRepeatType.FullTextRepeat);
          SignatureFont signatureFont1 = new SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName("Arial");
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(Color.WHITE);
          outerLine1.setBackgroundColor(Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // 하나 이상의 내부 사각형 라인을 추가하세요
          StampLine innerLine1 = new StampLine();
          innerLine1.setText("Company #1");
          innerLine1.setTextColor(Color.RED);
          SignatureFont signFont1 = new SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);

          // 스탬프가 추가된 문서를 저장하세요
          SignResult result = signature.sign("output.jpeg", options);
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
            link: "/examples/signature/formats/signature_stamp.jpeg"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "문서"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

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
    title: "핵심 기능 탐색"
    exclude: "stamp"
    description: "서명을 추가, 관리 및 삭제하기 위한 다양한 옵션을 활용하세요."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/jpeg/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/jpeg/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/jpeg/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/jpeg/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/jpeg/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/jpeg/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "여러 파일 형식에 스탬프 추가"
    exclude: "JPEG"
    description: "GroupDocs.Signature API는 60개 이상의 형식으로 문서에 스탬프를 추가하는 것을 지원합니다. 문서 관리 및 사용자 지정을 개선하기 위해 모든 페이지나 영역에 스탬프를 배치하세요."
    items: 
          
        # format loop 1
        - name: "PDF에 도장"
          format: "PDF"
          link: "/signature/java/stamp/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX에 도장"
          format: "DOCX"
          link: "/signature/java/stamp/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG에 도장"
          format: "JPEG"
          link: "/signature/java/stamp/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX에 도장"
          format: "PPTX"
          link: "/signature/java/stamp/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX에 도장"
          format: "XLSX"
          link: "/signature/java/stamp/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---