



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: ko
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java로 XLSX용 QR 코드 생성"
head_description: "GroupDocs.Signature API는 XLSX 파일용 QR 코드 생성을 지원합니다. 콘텐츠에서 QR 코드를 생성하고 모든 페이지에 삽입하십시오."

############################# Header ############################
title: "XLSX용 QR 코드 생성" 
description: "GroupDocs.Signature for Java를 사용하여 텍스트와 숫자 데이터를 포함한 2D 바코드를 생성하고 다양한 문서의 모든 페이지에 배치하십시오."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 평가판"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java에 대해 더 알아보기"
    link: "/signature/java/"
    link_title: "자세히 알아보기"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/)는 모든 주요 문서 형식에서 다양한 유형의 서명을 생성하고 포함할 수 있는 폭넓은 기능을 제공합니다. PDF, Word 문서, Excel 스프레드시트, PowerPoint 프레젠테이션 및 이미지 파일을 지원합니다. 문서에 텍스트, 이미지, 바코드, QR 코드, 메타데이터, 디지털 및 스탬프 서명을 추가하십시오.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX의 원하는 위치에 QR 코드를 생성하고 배치하는 단계"
    content: |
      [GroupDocs.Signature](/signature/java/)는 다양한 인기 형식에서 QR 코드를 생성하고 XLSX 페이지에 배치할 수 있습니다. 10가지 이상의 QR 코드 유형이 지원되며, Java 애플리케이션에 빠르게 통합될 수 있습니다. 생선된 QR 코드로 문서에 서명하는 데 제품을 사용하세요.
      
      1. QR 코드로 서명할 XLSX 파일 또는 스트림을 가져옵니다.
      2. QrCodeSignOptions에 대한 텍스트를 제공합니다.
      3. 색상, 위치, 크기 등과 같은 시각적 옵션을 사용자 정의합니다.
      4. QR 코드가 추가된 파일을 저장합니다.
   
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
        // 서명할 문서를 새 Signature 인스턴스에 전달합니다.
        Signature signature = new Signature("input.xlsx");

        // QrCodeSignOptions를 사용하여 문서에 QR 코드를 추가합니다.
        QrCodeSignOptions options = new QrCodeSignOptions("Text Content");

        // 서명 유형과 페이지상의 위치를 지정합니다.
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(50);
        options.setTop(150);

        // QR 코드가 추가된 파일을 저장합니다.
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서에 서명 추가"
  description: "GroupDocs.Signature for Java API는 모든 인기 파일 형식의 서명 지원합니다. 다양한 유형의 서명을 생성, 수정, 검색, 검증 및 삭제하십시오."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "GroupDocs.Signature의 주요 기능"
  features:
    # feature loop
    - title: "문서 서명"
      content: "GroupDocs.Signature는 텍스트, 이미지, 바코드, QR 코드 및 스탬프 서명으로 서명하는 것을 지원합니다. 모든 지원되는 문서 형식의 모든 페이지에 배치할 수 있습니다. 메타데이터 서명을 사용하여 문서 메타데이터를 관리하고, 디지털 인증서를 사용하여 무단 변경으로부터 콘텐츠를 보호하십시오."

    # feature loop
    - title: "검색 및 검증"
      content: "문서 내 모든 서명이 유효한지 검증 절차를 통해 확인하십시오. 내장 검색 기능을 사용하여 문서 내 서명의 전체 목록을 검색하십시오."

    # feature loop
    - title: "서명 수정"
      content: "서명 후 서명 속성을 쉽게 수정하십시오. 필요에 따라 콘텐츠, 위치, 색상, 크기 및 기타 속성을 조정하십시오."

    # feature loop
    - title: "서명 삭제"
      content: "원치 않는 서명을 간단하게 삭제하십시오. 디지털 인증서를 포함한 다양한 서명 유형을 프로그램적으로 문서에서 제거할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "생성된 QR 코드 사용자 정의 방법"
      content: |
        이 예제를 사용하여 XLSX 페이지에 새로운 QR 코드를 배치하는 방법을 배우십시오.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 서명할 문서를 가져와 Signature에 전달합니다.
          Signature signature = new Signature("input.xlsx");

          // QR 코드 옵션을 사용하여 필요한 정보를 담은 텍스트를 제공합니다.
          QrCodeSignOptions signOptions = new QrCodeSignOptions("Archived on July 11, 2019");

          // 페이지에서 QR 코드의 상대적 위치를 설정합니다.
          signOptions.setVerticalAlignment(VerticalAlignment.Top);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Right);

          // 서명의 패딩을 설정합니다.
          Padding padding = new Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // QR 코드의 색상을 지정합니다.
          signOptions.setForeColor(Color.RED);

          // 메시지의 글꼴 옵션을 정의합니다.
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // QR 코드 배경 색상 및 브러시를 사용자 정의합니다.
          Background background = new Background();
          background.setColor(Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new LinearGradientBrush(Color.GREEN, Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // QR 코드를 문서에 추가합니다.
          SignResult signResult = signature.sign("output.xlsx", signOptions);
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
            link: "/examples/signature/formats/signature_qrcode.xlsx"
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
    title: "주요 제공 사항 확인"
    exclude: "qrcode"
    description: "우리는 다양한 서명 기능과 고급 작업을 제공합니다."
    items: 
          
        # operation loop 1
        - name: "전자 서명"
          operation: "esign"
          link: "/signature/java/esign/xlsx/"
          description: "지원되는 파일 형식에 다양한 종류의 서명을 추가합니다."

        # operation loop 2
        - name: "문서에 텍스트 추가"
          operation: "text"
          link: "/signature/java/text/xlsx/"
          description: "사용자 정의 텍스트 서명으로 문서 내용을 향상시킵니다."

        # operation loop 3
        - name: "이미지 서명"
          operation: "image"
          link: "/signature/java/image/xlsx/"
          description: "문서 내 원하는 위치에 이미지를 배치합니다."

        # operation loop 4
        - name: "바코드 생성"
          operation: "barcode"
          link: "/signature/java/barcode/xlsx/"
          description: "지원되는 문서에 다양한 바코드를 생성하고 삽입합니다."

        # operation loop 5
        - name: "QR 코드 생성"
          operation: "qrcode"
          link: "/signature/java/qrcode/xlsx/"
          description: "문서 서명을 위한 QR 코드를 생성합니다."
          
        # operation loop 6
        - name: "디지털 인증서"
          operation: "digital"
          link: "/signature/java/digital/xlsx/"
          description: "비즈니스를 안전하게 보호하고 문서에 디지털 인증서로 서명합니다."

        # operation loop 7
        - name: "도장 서명"
          operation: "stamp"
          link: "/signature/java/stamp/xlsx/"
          description: "스탬프 생성기를 사용하여 사용자 정의 원형 또는 사각형 도장을 만듭니다."
          
        # operation loop 8
        - name: "서명 검색"
          operation: "search"
          link: "/signature/java/search/xlsx/"
          description: "문서 내 이전에 추가된 서명을 찾습니다."
          
        # operation loop 9
        - name: "서명 검증"
          operation: "verify"
          link: "/signature/java/verify/xlsx/"
          description: "서명이 적용된 후 서명의 진위를 검증합니다."
          
        # operation loop 10
        - name: "서명 수정"
          operation: "modify"
          link: "/signature/java/modify/xlsx/"
          description: "문서 내 다양한 서명을 쉽게 편집합니다."
          
        # operation loop 11
        - name: "서명 삭제"
          operation: "delete"
          link: "/signature/java/delete/xlsx/"
          description: "이전에 적용된 다양한 서명을 제거합니다."
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "추가 파일 형식에 대한 QR 코드 생성"
    exclude: "XLSX"
    description: "Java API를 사용하여 생성된 QR 코드로 모든 인기 파일 형식을 향상시키십시오. 쉽게 스캔 및 처리할 수 있도록 2D 바코드 데이터를 추가하십시오."
    items: 
          
        # format loop 1
        - name: "PDF용 QR 코드"
          format: "PDF"
          link: "/signature/java/qrcode/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 2
        - name: "DOCX용 QR 코드"
          format: "DOCX"
          link: "/signature/java/qrcode/docx/"
          description: "마이크로소프트 워드 개방 XML 문서"
          
        # format loop 3
        - name: "JPEG용 QR 코드"
          format: "JPEG"
          link: "/signature/java/qrcode/jpeg/"
          description: "JPEG 이미지"
          
        # format loop 4
        - name: "PPTX용 QR 코드"
          format: "PPTX"
          link: "/signature/java/qrcode/pptx/"
          description: "파워포인트 개방 XML 프레젠테이션"
          
        # format loop 5
        - name: "XLSX용 QR 코드"
          format: "XLSX"
          link: "/signature/java/qrcode/xlsx/"
          description: "마이크로소프트 엑셀 개방 XML 스프레드시트"


          

---