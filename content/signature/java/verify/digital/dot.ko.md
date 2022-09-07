---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Verify
signaturetype: Digital
fileformat: Dot
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotx odt ott xls xlsx xlsm xlsb ods ots xltx xltm pptx pptm
breadcrumb: Put Digital signature on Dot for Java

############################# Head ############################
head_title: "Java을 통해 Dot 파일에 대한 Digital 서명 확인"
head_description: "몇 줄의 Java 코드만 사용하여 Dot 문서와 Digital 서명을 확인하십시오."

############################# Header ############################
title: "Dot 파일에 대한 Digital 서명 확인"
description: "Java용 API는 Dot 문서에서 Digital 서명을 확인할 수 있는 기회를 제공합니다. Dot 문서 내의 전자 서명 확인은 빠르고 쉽게 수행될 수 있습니다."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"



############################# About ############################
about:
    enable: true
    title: "새로운 GroupDocs.Signature for Java API 기능 알아보기"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API는 전자 서명을 사용하여 다양한 문서 형식을 처리하는 다양한 방법을 제공합니다. 텍스트, 이미지, 디지털 인증서, 바코드, QR 코드, 스탬프 또는 메타데이터와 같은 다양한 유형의 디지털 서명이 지원됩니다. 고객은 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에서 디지털 서명을 추가, 제거, 편집, 유효성 검사 또는 검색할 수 있습니다. 놀라운 수의 추가 기능과 설정을 사용할 수 있습니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Dot 문서에서 Digital 서명을 확인하는 방법"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)에는 Dot 문서에 있는 Digital 서명 확인과 같은 유용한 기능이 포함되어 있습니다. 추가 코드를 구현하지 않고 이 기회를 사용하십시오.
        
        * 먼저 확인해야 하는 문서에 대한 생성자 매개변수 경로를 제공하는 Signature 클래스를 인스턴스화합니다.
        * 둘째, 새 VerifyOptions 개체를 만들고 모든 필수 속성을 설정합니다.
        * 마지막으로, VerifyOptions 인스턴스를 전달하는 서명의 개체 Verify 메서드를 호출합니다.
        * 그런 다음 검증 결과를 처리합니다.

    title_right: "System Requirements"
    content_right: |
        GroupDocs.Signature for Java은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)에서 최신 버전의 GroupDocs.Signature for Java 다운로드
         
    code: |
        ```java    
                
        // Set up input Dot file
        String filePath = "input.dot";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        //Provide verification options
        DigitalVerifyOptions options = new DigitalVerifyOptions();

        // Digital signature comment
        options.setComments("Approved");

        // specify period of signatures
        options.setSignDateTimeFrom(new Date(2020, 12, 12));
        options.setSignDateTimeTo(new Date(2022, 12, 12));
                            
        // Verify document signatures
        VerificationResult result = signature.verify(options);

        //process result
        if (result.isValid())
        {
            //..
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Digital 서명으로 서명 라이브 데모"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트를 방문하여 Dot 파일에 다양한 전자 서명을 추가하세요.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java을(를) 사용하여 다른 Digital 서명 확인"
    content: |
        "다양한 문서에 배치된 전자 서명 확인. 아래와 같이 널리 사용되는 파일 형식의 서명 품질을 확인하십시오."
    format: 
       
       
back_to_top:
    enable: true
---