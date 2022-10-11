---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: Sign
signaturetype: Barcode
codetype: UPCA
fileformat: Png
productName: Java
lang: ko
productCode: java
otherformats: pdf doc docx docm dot dotm dotx odt ott rtf xls xlsx xlsm xlsb csv ods ots xltx xltm ppt pptx pps ppsx odp otp potx potm pptm ppsm png jpg bmp gif tiff svg webp wmf
breadcrumb: Put  Barcode signature on Png for Java

############################# Head ############################
head_title: "Java의 UPCA 바코드로 Png 문서에 전자 서명"
head_description: "UPCA Barcode Signature를 생성하고 몇 줄의 코드를 사용하여 Java를 사용하여 Png 문서에 넣습니다. 다양한 파일 형식에 서명하려면 GroupDocs 문서 서명 API를 사용하십시오."

############################# Header ############################
title: "Java에서 Png 문서에 대한 UPCA 바코드 서명 생성"
description: "UPCA 바코드로 Png 비즈니스 문서에 전자 서명하세요. 서명 옵션을 설정하는 몇 줄의 코드로 빠르고 쉽게 바코드 서명을 생성합니다."
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
    title: "GroupDocs.Signature for Java Barcode signatures API 정보."
    content: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)은 UPCA, UPCE, EAN13, EAN14, Code39, Code39Extended, Code128, Codabar, Postnet, ISBN과 같은 바코드 유형을 사용하여 디지털 문서 전자 서명을 관리하는 빠르고 쉬운 API입니다. , ITF14 및 기타 다수. 고객은 필요한 텍스트를 제공하는 바코드를 쉽게 생성하여 PDF, Microsoft Office Words 문서, Microsoft Office Excel 통합 문서, MS PowerPoint 프레젠테이션, Adobe Photoshop 파일 및 다양한 이미지 형식에 넣을 수 있습니다. 문서에 배치된 바코드는 업데이트, 검색, 확인, 삭제 또는 미리 볼 수 있습니다. 또한 바코드 사용자 정의가 지원됩니다.
    

############################# Steps ############################
steps:
    enable: true
    title_left: "Java에서 Barcode으로 Png에 서명하는 단계"
    content_left: |
        [GroupDocs.Signature for Java](https://products.groupdocs.com/signature/java/)은 Barcode 서명으로 Png 문서에 빠르고 쉽게 서명할 수 있는 기능을 제공합니다.
        
        * 경로 또는 메모리 스트림으로 서명해야 하는 Png 파일을 제공하는 Signature 클래스의 인스턴스 생성
        * SignOptions 클래스를 인스턴스화하고 필요한 모든 데이터를 설정합니다.
        * 출력 Png 파일 또는 메모리 스트림을 전달하는 Signature.Sign() 메서드를 호출합니다.

    title_right: " 시스템 요구 사항"
    content_right: |
        GroupDocs.Signature for Java은(는) 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 전제 조건이 설치되어 있는지 확인하십시오.

        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java runtime: J2SE 6.0 and above
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-signature)에서 최신 GroupDocs.Signature for Java 가져오기
         
    code: |
        ```java    
                
        // Set up input Png file
        String filePath = "input.png";
        // Set up output file
        String outputFilePath = "output.png";

        // Instantiate Signature for input file
        Signature signature = new Signature(filePath);

        // create barcode option with predefined barcode text
        BarcodeSignOptions options = new BarcodeSignOptions("John Smith");

        // setup Barcode encoding type
        options.setEncodeType(BarcodeTypes.UPCA);

        // set signature position
        options.setLeft(50);
        options.setTop(50);
        options.setWidth(200);
        options.setHeight(50);

        // sign Png document
        SignResult result = signature.sign(outputFilePath, options);

        ```

############################# Demos ############################
demos:
    enable: true
    title: "Barcode 라이브 데모로 Png 문서 서명"
    content: |
       지금 바로 [GroupDocs.Signature 앱](https://products.groupdocs.app/signature/family) 웹사이트에서 다양한 서명으로 Png 파일에 서명하세요. 무료 온라인 데모가 여러분을 기다리고 있습니다.

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About UPCA Barcode"
          content: |
            범용 제품 코드는 매장에서 거래 품목을 추적하기 위해 전 세계적으로 널리 사용되는 바코드 기호입니다.
          characterset: |
             숫자(0-9).
          textcapacity: |
             정확히 11자리 + 1 체크 디지트입니다.
          image: |
             iVBORw0KGgoAAAANSUhEUgAAAGwAAABjCAYAAAB+MOUYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAARpSURBVHhe7ZFBimBRCMT6/pfuUYaAi6pe58MLSJCAG39+H5/iPexjvId9jPewj/Ee9jHewz7Ge9jH+PNhPz//M4bdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXoZ2YHdzS2bA2q4TvQztwO7mlsyAtV0nehnagd3NLZkBa7tO9DK0A7ubWzID1nad6GVoB3Y3t2QGrO060cvQDuxubskMWNt1opehHdjd3JIZsLbrRC9DO7C7uSUzYG3XiV6GdmB3c0tmwNquE70M7cDu5pbMgLVdJ3oZ2oHdzS2ZAWu7TvQytAO7m1syA9Z2nehlaAd2N7dkBqztOtHL0A7sbm7JDFjbdaKXoR3Y3dySGbC260QvQzuwu7klM2Bt14lehnZgd3NLZsDarhO9DO3A7uaWzIC1XSd6GdqB3c0tmQFru070MrQDu5tbMgPWdp3oZWgHdje3ZAas7TrRy9AO7G5uyQxY23Wil6Ed2N3ckhmwtutEL0M7sLu5JTNgbdeJXh5K3sM+xnvYx3gP+xjvYR/jPexT/P7+A4FOQDtpBhIBAAAAAElFTkSuQmCC

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Java에 대해 지원되는 기타 Barcode 서명"
    content: |
        "다른 서명 유형으로 Png에 서명할 수도 있습니다. 아래 목록을 참조하십시오."
    format: 
        
       
back_to_top:
    enable: true
---