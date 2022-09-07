---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Search
signaturetype: Metadata
fileformat: Doc
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Search Metadata signatures at Doc with Java

############################# Head ############################
head_title: "Java의 Doc 파일에서 Metadata 서명 검색"
head_description: "몇 줄의 코드를 사용하여 Doc 파일에서 Metadata 서명을 검색하려면 Java를 사용하세요."

############################# Header ############################
title: "Doc 파일에서 Metadata 서명 검색"
description: "Java 기본 API를 사용하면 이미 서명된 Doc 파일에서 Metadata 서명을 검색할 수 있습니다. 몇 줄의 코드를 사용하여 Doc 문서 내에서 고급 전자 서명 검색을 수행합니다."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocsature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "GroupDocs.Signature for Java API 정보"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)은 텍스트, 이미지, 디지털 인증서, 바코드, QR 코드, 스탬프 또는 메타데이터와 같은 다양한 서명 유형을 사용하여 문서를 처리하기 위한 Java API를 제공합니다. 사용자는 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식 내에서 전자 서명을 추가, 삭제, 업데이트, 확인 또는 검색할 수 있으며 필요에 따라 서명 속성을 사용자 지정하기 위한 추가 지원이 가능합니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Doc에서 Metadata 서명을 검색하는 방법"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)을 사용하면 몇 가지 간단한 단계를 구현하여 Java 개발자가 애플리케이션의 Doc 파일에서 Metadata 서명을 더 쉽게 검색할 수 있습니다.
        
        * Signature 클래스의 새 인스턴스를 만들고 소스 문서 경로를 생성자 매개변수로 전달합니다.
        * 요구 사항에 따라 SearchOptions 개체를 인스턴스화하고 검색 옵션을 지정합니다.
        * Signature 클래스 인스턴스의 Search 메소드를 호출하고 여기에 SearchOptions를 전달하십시오.
        * 귀하의 요구에 따라 검색 결과를 처리합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)에서 최신 버전의 GroupDocs.Signature for Java 다운로드
         
    code: |
        ```java    
        
        // Set up input Doc file
        String filePath = "input.doc";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // search for Metadata signatures in Doc document
        List<WordProcessingMetadataSignature> signatures = signature.search(WordProcessingMetadataSignature.class, SignatureType.Metadata);

        // process signatures which were found 
        signatures.forEach(item -> System.out.println(item.toString()));


        ```

############################# Demos ############################
demos:
    enable: true
    title: "Metadata 서명으로 서명 라이브 데모"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트를 방문하여 Doc 파일에 다양한 전자 서명을 추가하세요.

        
############################# More Formats ############################
more_formats:
    enable: true
    title: "Java을(를) 사용하여 다른 Metadata 서명 검색"
    content: |
        "전자 서명은 다양한 문서에서 검색됩니다. 아래와 같이 널리 사용되는 파일 형식 중 하나에서 서명을 찾으십시오."
    format: 
           
       
back_to_top:
    enable: true
---