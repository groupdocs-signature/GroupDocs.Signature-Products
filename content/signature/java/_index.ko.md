---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 디지털 서명 API, PDF Word Excel 이미지에 전자 서명 추가"
head_description: "자바 디지털 서명 API. PDF, Microsoft Word, Excel 스프레드시트, PowerPoint 프레젠테이션 및 이미지 문서 형식에 디지털 서명을 하는 전자 서명 라이브러리입니다."

############################# Header ############################
title: "디지털 서명을 관리하는 Java API"
description: "이미지 및 디지털 문서 파일 형식 서명을 위해 Java 애플리케이션에서 이미지, QR 코드, 바코드, 메타데이터, 텍스트 및 스탬프 유형의 전자 서명을 관리합니다."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "개요"

            # button loop
            - link: "#features"
              text: "특징"

            # button loop
            - link: "#support"
              text: "지원하다"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "라이브 데모"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      Java API용 GroupDocs.Signature를 사용하면 외부 소프트웨어를 설치하지 않고도 지원되는 형식의 디지털 문서에 서명할 수 있는 전자 서명 기능이 있는 Java 응용 프로그램을 개발할 수 있습니다. 이미지, 바코드, QR 코드, 스탬프, 텍스트, 광학 및 메타데이터와 같은 다양한 유형의 전자 서명 조작 및 관리를 지원합니다. Microsoft Office Word, PowerPoint 프레젠테이션, Excel 스프레드시트, 이미지 및 PDF 파일과 같은 모든 전자 비즈니스 문서는 서명 속성을 사용자 지정하여 디지털 서명할 수 있습니다. 귀하의 요구 사항에 따라 그림자, 치수, 정렬 등. 디지털 서명 라이브러리는 단순하고 가벼우며 신규 또는 기존 Java 애플리케이션 내에서 쉽게 통합할 수 있는 단일 DLL 파일로 구성됩니다.  

      GroupDocs.Signature for Java API를 통해 시스템에서 등록된 모든 인증서를 로드하거나 단순 및 고급 검색을 사용하여 기존 서명을 찾을 수 있습니다. 일반 서명 속성(텍스트 크기, 불투명도, 회전, 확인, 글꼴 속성, 색상 옵션, 페이지 번호, 너비, 상단, 왼쪽 등)을 지정하고 다양한 전자 서명 유형 구현 지원을 지정하여 암호로 보호된 문서 작업 옵션을 통해 신뢰할 수 있습니다. 디지털 문서를 위한 전자 서명 관리 솔루션입니다.  

      Java용 GroupDocs.Signature는 모든 Java 버전과 호환되며 Java 런타임을 실행할 수 있는 널리 사용되는 운영 체제(Windows, Linux, MacOS)를 지원합니다.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          다음은 Java용 GroupDocs.Signature 기능의 개요입니다.
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "서명 유형"
          content: |
            * 텍스트 서명
            * 이미지 서명
            * 디지털 서명
            * QR 코드 서명
            * 바코드 서명
            * 스탬프 서명
            * 양식 필드 서명
      
      ## TAB TWO ##
      tab_two:
        description: |
          Java 전자 서명 API는 아래와 같이 [문서 파일 형식](https://docs.groupdocs.com/signature/java/supported-document-formats/)을 지원합니다.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **이미지**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **메타파일**: EMF, WMF, CMX
                * **가지고 다닐 수 있는**: PDF
                * **확장 가능한 벡터 그래픽**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **기타**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          Java용 GroupDocs.Signature는 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "개발 환경"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "빌드 자동화 도구"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Java용 GroupDocs.Signature 기능"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "지원되는 문서 형식에서 전자 서명 생성, 읽기, 수정, 숨기기 및 삭제"

      # feature loop
      - icon: "fas fa-eye"
        content: "스트림, 상대 경로 또는 절대 경로에서 서명된 문서에 액세스"

      # feature loop
      - icon: "fas fa-bolt"
        content: "문서, 스프레드시트, 프리젠테이션, 이미지 및 PDF 파일에 텍스트 서명 적용"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "PDF 파일에 주석, 스티커, 이미지로 텍스트 서명 추가 및 스타일 및 색상 구성"

      # feature loop
      - icon: "fas fa-code"
        content: "PDF 문서, 이미지 파일에 서명하고 다른 파일 형식으로 출력하기"

      # feature loop
      - icon: "fas fa-cloud"
        content: "텍스트 서명을 워터마크로 사용하여 이미지에 디지털 서명 및 투명도 추가, 전자 서명에 회전"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "인증서 검색 및 디지털 인증서로 Microsoft Word, Excel 및 PDF 문서 서명"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "기본 텍스트 워터마크로 워드 프로세싱 문서 형식 서명"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "QR 코드, 바코드를 사용하여 단어, 슬라이드, 셀, PDF 및 이미지 파일 서명"

      # feature loop
      - icon: "fas fa-border-all"
        content: "지원되는 파일 형식을 보호하기 위해 스탬프 서명 구성 및 적용"

      # feature loop
      - icon: "fas fa-wrench"
        content: "문서, 스프레드시트, 프리젠테이션, 이미지 및 PDF 파일에 이미지 서명 설정 및 할당"

      # feature loop
      - icon: "fas fa-columns"
        content: "서명 속성(예: 모양 및 느낌, 여백, 정렬 등)을 구성합니다."

      # feature loop
      - icon: "fas fa-file-word"
        content: "암호로 보호된 문서에 디지털 서명 적용"

      # feature loop
      - icon: "fas fa-envelope"
        content: "서명 처리기를 사용하여 PDF 문서의 텍스트 확인 수행"

      # feature loop
      - icon: "fas fa-print"
        content: ".CER 및 .PFX 인증서 컨테이너를 사용하여 Word, Cell, PDF 문서의 디지털 검증"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "PDF 텍스트 서명에 대해 다른 측정 단위 유형(예: 밀리미터, 픽셀 등) 지정"

      # feature loop
      - icon: "fas fa-lock"
        content: "파일 또는 URL을 통해 문서 정보 얻기 - PDF 문서에 양식 필드 서명 추가"

      # feature loop
      - icon: "fas fa-file-code"
        content: "맞춤형 데이터 객체, 임베디드 VCard, 이메일, EPC, MeCard 또는 이벤트 객체를 QR 코드에 추가"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "서명에 다양한 브러시 스타일 적용(예: 그라데이션, 방사형, 단색 및 텍스처 브러시)"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "FTP 또는 Azure Cloud Storage에 있는 문서 서명"

      # feature loop
      - icon: "fas fa-heading"
        content: "문서, 슬라이드, 이미지 및 PDF 파일의 도형 내부에 텍스트 정렬 설정"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "PowerPoint 프레젠테이션 문서 검색, 확인 및 디지털 서명"

      # feature loop
      - icon: "fas fa-cube"
        content: "셀 문서의 픽셀을 사용하여 서명 배치 및 스탬프 서명을 위한 텍스트 위치 지정"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "모서리가 둥근 사각형 스탬프 서명 구현"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "이미지 데이터 콘텐츠로 바코드 및 QR 코드 서명 확장"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "서명 및 검색 옵션으로 작업하는 동안 암호화된 메타데이터 서명 추가"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "Word, Excel 및 프레젠테이션 내의 메타데이터 서명에 사용자 지정 개체 포함"

    more_feature:
      # more_feature_loop
      - title: "손쉬운 전자 서명 구성 및 적용"
        content: |
          Java API용 GroupDocs.Signature를 사용하면 전자 서명을 구성하고 지원되는 문서 형식에 추가할 수 있습니다. 다음은 PDF 파일에 텍스트 서명을 적용하는 것이 얼마나 간단한지 보여주는 코드 예제입니다.

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // 서명 위치 설정
          options.setLeft(100);
          options.setTop(100);
          
          // 서명 사각형 설정
          options.setWidth(100);
          options.setHeight(30);

          // 텍스트 색상 및 글꼴 설정
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // 문서를 파일로 서명
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "전자 서명에 대해 지원되는 바코드 인코딩 유형"
        content: |
          Java API용 GroupDocs.Signature를 사용하여 지원되는 파일 형식에 바코드 및 QR 코드 서명을 적용할 수 있습니다. Java용 GroupDocs.Signature는 대부분의 요구 사항을 충족할 수 있는 광범위한 바코드 인코딩 유형을 지원합니다. 지원되는 바코드 인코딩 유형에는 Code 11, Code 128, Code 16K/32, Databar 코드, GS1 Codeblock, ISBN, ISMN, ISSN, ITF16, Pdf147, EAN8, EAN13, EAN14, UPCA, UPCE, ITF14, Code39 Standard 및 Code39 확장.

          마찬가지로 GroupDocs.Signature for Java API를 사용하면 QR, Aztec 및 Data Matrix와 같은 QR 코드 유형을 사용할 수 있습니다. 지원되는 QR 코드 인코딩 유형에는 Aztec, DataMatrix, GS1 DataMatrix 및 GS1 QR이 포함됩니다.

      # more_feature_loop
      - title: "서명 및 인증서 검색"
        content: |
          GroupDocs.Signature for Java API를 통해 모든 문서, 프리젠테이션, 스프레드시트, 이미지 및 PDF 파일에서 QR 코드 및 바코드 서명을 검색하고 검색 결과를 가져올 수 있습니다. 또한 QR 코드 서명으로 서명된 문서에서 사용자 지정 데이터 개체를 검색하고 QR 코드로 서명된 문서에서 표준 VCard 및 이메일 개체를 검색할 수 있습니다. QR 코드 서명의 암호화된 텍스트 확인 및 PDF 문서의 메타데이터 서명 검색도 지원됩니다. Words & Cells 문서의 디지털 서명에 대한 추가 검색 기준을 적용합니다.  

          검색 옵션은 Word 문서, 슬라이드 및 스프레드시트의 메타데이터 서명에도 사용할 수 있으며 양식 필드 검색은 PDF 문서에 사용할 수 있습니다.

      # more_feature_loop
      - title: "전자 서명 속성 구성"
        content: |
          최종 사용자의 UX를 향상시키기 위해 GroupDocs.Signature for Java API는 매우 쉽게 구성할 수 있는 많은 속성을 제공합니다. 글꼴 및 색상 옵션(배경색, 전경색, 굵게, 기울임꼴, 밑줄, 글꼴군, 글꼴 크기 등), 배경 및 테두리 옵션(배경색, 배경 투명도, 테두리 색상, 테두리 대시 스타일, 테두리 두께, 테두리 투명도 등), 서명 여백(왼쪽, 위쪽, 너비, 높이, 여백 등), 이미지 서명 영역 및 서명 정렬 설정(가로 정렬, 세로 정렬 등).

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Signature는 널리 사용되는 다른 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---