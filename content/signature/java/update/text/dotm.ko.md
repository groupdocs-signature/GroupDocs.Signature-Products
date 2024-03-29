---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Update
signaturetype: Text
fileformat: Dotm
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm
breadcrumb: Put Text signature on Dotm for Java

############################# Head ############################
head_title: "Java을(를) 사용하여 Dotm 파일에 있는 Text 서명 업데이트"
head_description: "서명된 Dotm 문서에서 Text 서명 업데이트를 위해 간단하고 이해하기 쉬운 Java 코드를 사용하세요."

############################# Header ############################
title: "Dotm 파일에 있는 Text 서명 편집 및 업데이트"
description: "Java용 API는 Dotm 문서에서 업데이트되는 Text 서명에 대한 기능을 제공합니다. 몇 줄의 Java 코드로 Dotm 문서 내의 전자 서명을 빠르고 쉽게 업데이트하십시오."
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
    title: "GroupDocs.Signature for Java API 기능에 대해 알아보기"
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/) API 기능에는 전자 서명을 사용하여 주문형 문서 형식을 처리하기 위한 다양한 수단이 포함되어 있습니다. 텍스트, 이미지, 디지털 인증서, 바코드, QR 코드, 스탬프 또는 메타데이터와 같은 광범위한 전자 서명이 지원됩니다. 고객은 PDF, MS Word 문서, MS Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에서 디지털 서명을 추가, 제거, 편집, 유효성 검사 또는 검색할 수 있습니다. 많은 유용한 기능과 설정을 사용할 수 있습니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Dotm 문서에서 Text 서명을 변경하는 방법"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)에는 Dotm 문서에 있는 Text 서명 업데이트와 같은 유용한 기능이 포함되어 있습니다. 추가 코드 없이 서명 기능을 변경할 수 있습니다.
        
        * 시작하려면 업데이트해야 하는 문서에 대한 생성자 매개변수 경로로 전달하는 Signature 객체를 생성합니다.
        * 그런 다음 적절한 특정 서명 개체를 인스턴스화하고 변경해야 하는 해당 식별자와 속성을 설정합니다.
        * 마지막으로 특정 서명 개체를 전달하는 Signature의 Update 메서드를 호출합니다.
        * 통지에 대한 결과 업데이트를 처리합니다.

    title_right: "시스템 요구 사항"
    content_right: |
        GroupDocs.Signature for Java은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)에서 최신 버전의 GroupDocs.Signature for Java 다운로드
         
    code: |
        ```java    
                
        // Set up input Dotm file
        String filePath = "input.dotm";
        // Set up output file
        String outputFilePath = "output.dotm";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // Id of signature which is supposed to be updated
        // such Id might be got as a result of search operation
        String id = "eff64a14-dad9-47b0-88e5-2ee4e3604e71";

        // provide signature features to update
        // set up particular signature id
        TextSignature signatureToUpdate = new TextSignature(id);

        // specify signature width
        signatureToUpdate.setWidth(130);
        // specify signature height
        signatureToUpdate.setHeight(20);
        // set left position
        signatureToUpdate.setLeft(40);
        // set top position
        signatureToUpdate.setTop(50);
        // set up new text
        signatureToUpdate.setText("Mr. John Smith");

        // update signature
        Boolean updateResult = signature.update(outputFilePath, signatureToUpdate);

        // process updation result
        if (updateResult)
        {
                System.out.println("Signature was updated successfully!");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "문서 페이지에서 Text 서명 업데이트 - 라이브 데모"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 Dotm 문서의 다양한 전자 서명을 수정하세요.          

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java을(를) 통해 다양한 Text 서명 업데이트"
    content: |
        "다양한 문서 형식에 있는 디지털 서명을 편집합니다. 추가 코드 없이 서명 데이터를 업데이트합니다."
    format: 
       
       
back_to_top:
    enable: true
---