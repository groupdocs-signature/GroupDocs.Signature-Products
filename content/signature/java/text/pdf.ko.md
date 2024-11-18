



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:54
draft: false
lang: ko
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java을(를) 사용하여 PDF 텍스트 서명 만들기"
head_description: "Java API를 활용하여 PDF 파일에 텍스트 서명을 삽입하세요. PDF, Word, Excel, 프레젠테이션, 이미지 및 ZIP을 포함한 인기 있는 문서 형식을 원활하게 처리합니다."

############################# Header ############################
title: "PDF용 텍스트 서명 만들기" 
description: "GroupDocs.Signature for Java를 사용하여 비즈니스 문서에 사용자 지정 텍스트 서명을 추가하세요. 서명 사용자 지정 옵션을 통해 조직의 작업 흐름을 간소화하세요."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 시작하기"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java 솔루션 소개"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 문서 관리 작업을 간소화하기 위해 유연하고 사용자 지정 가능한 텍스트 서명을 제공합니다. 텍스트 서명의 내용과 디자인을 구성하고, 모든 페이지에 적용하여 조직의 문서 작업 흐름을 향상시킵니다.

############################# Steps ############################
steps:
    enable: true
    title: "Java을(를) 사용하여 PDF에 텍스트 서명 추가하는 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 Java 애플리케이션에 통합되어 PDF 문서에 텍스트 서명을 추가할 수 있습니다. 개발자는 우리의 솔루션을 사용하여 제품의 기능을 신속하게 향상시킬 수 있습니다.
      
      1. Signature 클래스 생성자에 PDF 문서를 매개변수로 사용하세요.
      2. 필요한 텍스트로 TextSignOptions를 인스턴스화하세요.
      3. 서명의 시각적 옵션을 구성하십시오.
      4. 텍스트 서명을 문서의 모든 페이지에 추가하세요.
   
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
        // Signature 생성자에 문서 경로 전달
        Signature signature = new Signature("input.pdf");

        // 서명 텍스트로 TextSignOptions 인스턴스화
        TextSignOptions options = new TextSignOptions("Approved");
        
        // 텍스트 색상 및 글꼴 속성 설정
        options.setForeColor(Color.RED);
        SignatureFont signatureFont = new SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName("Comic Sans MS");
        options.setFont(signatureFont);

        // 문서에 텍스트 서명 추가
        SignResult result = signature.sign("output.pdf", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 텍스트 서명 관리"
  description: "GroupDocs.Signature for Java를 사용하면 인기 있는 파일 형식에 텍스트 서명을 추가하여 회사의 문서 작업 흐름을 간소화할 수 있습니다. 서명의 외관과 내용을 쉽게 구성할 수 있습니다."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "문서 서명"
      content: "지원되는 문서의 모든 페이지에 텍스트, 이미지, 바코드, QR 코드 또는 스탬프 서명을 적용합니다. 메타데이터를 활용하여 숨겨진 내용을 삽입하고 디지털 인증서로 문서를 보호하세요."

    # feature loop
    - title: "서명 검색 및 검증"
      content: "서명 검증 도구를 통해 서명된 문서의 무결성을 보장하세요. 문서 내에 삽입된 모든 서명을 검색하고 검색할 수 있습니다."

    # feature loop
    - title: "서명 수정 또는 제거"
      content: "기존에 추가된 서명의 내용, 위치 및 외관을 수정하거나 문서에서 완전히 제거할 수 있습니다."

    # feature loop
    - title: "네이티브 텍스트 서명"
      content: "PDF의 스티커나 Word 문서의 워터마크와 같은 문서 특정 텍스트 서명을 추가하여 사용자 지정을 강화하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "문서에 텍스트 서명 추가"
      content: |
        비즈니스 문서에 텍스트 정보를 추가하여 비즈니스 프로세스를 향상시키는 방법을 배우세요.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 서명할 문서 선택
          Signature signature = new Signature("input.pdf");

          // 원하는 텍스트로 텍스트 옵션 생성
          TextSignOptions options = new TextSignOptions("Rescheduled to 03/04/2025");

          // 서명의 크기 및 페이지 위치 지정
          options.setLeft(100);
          options.setTop(180);
          options.setWidth(230);
          options.setHeight(30);

          // 서명은 페이지 모서리에서 여백을 지원합니다.
          Padding padding = new Padding();
          padding.setBottom(20);
          padding.setRight(20);
          options.setMargin(padding);

          // 텍스트 색상 및 글꼴 스타일은 사용자 지정할 수 있습니다.
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);

          // 텍스트 서명에 테두리를 포함할 수 있습니다.
          Border border = new Border();
          border.setColor(Color.RED);
          border.setDashStyle(DashStyle.Dash);
          border.setTransparency(0.5);
          border.setVisible(true);
          border.setWeight(2);
          options.setBorder(border);

          // 배경 사용자 지정도 가능합니다.
          Background background = new Background();
          background.setColor(Color.YELLOW);
          background.setTransparency(0.8);
          options.setBackground(background);

          // 텍스트는 호환성을 위해 이미지로 저장할 수 있습니다.
          options.setSignatureImplementation(TextSignatureImplementation.Image);

          // 추가된 텍스트로 문서 저장
          SignResult result = signature.sign("output.pdf", options);
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
            link: "/examples/signature/formats/signature_text.pdf"
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
    title: "주요 기능 및 서명 옵션"
    exclude: "text"
    description: "우리의 솔루션은 일곱 가지 서로 다른 유형의 서명에 대해 완전한 CRUD 작업 및 그 이상을 지원합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
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
    title: "다양한 파일 형식에 텍스트 서명 추가"
    exclude: "PDF"
    description: "Java API를 활용하여 Office 문서에 텍스트 서명을 삽입하여 문서 생애 주기의 모든 단계에서 내용에 대한 완전한 제어를 보장하세요."
    items: 
          
        # format loop 1
        - name: "PDF 텍스트 서명"
          format: "PDF"
          link: "/signature/java/text/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX 텍스트 서명"
          format: "DOCX"
          link: "/signature/java/text/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG 텍스트 서명"
          format: "JPEG"
          link: "/signature/java/text/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX 텍스트 서명"
          format: "PPTX"
          link: "/signature/java/text/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX 텍스트 서명"
          format: "XLSX"
          link: "/signature/java/text/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---