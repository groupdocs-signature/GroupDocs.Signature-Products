



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:13
draft: false
lang: es
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Búsqueda de firmas electrónicas para PPTX usando Python"
head_description: "Aprovecha la API de GroupDocs.Signature for Python via .NET para buscar firmas electrónicas incrustadas en formatos como PDFs, Word, Excel, Presentaciones e Imágenes."

############################# Header ############################
title: "Búsqueda de firmas digitales en PPTX" 
description: "Extrae una lista completa de firmas electrónicas de múltiples formatos, incluyendo PDFs, Word, Excel, Presentaciones e Imágenes, con el poder de GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar ahora"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Desata el potencial de GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Aprende más"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) ofrece capacidades avanzadas para firmar y gestionar documentos digitales. Con soporte para más de 60 formatos de archivo, incluyendo PDFs, documentos de Office, Imágenes y archivos ZIP, puedes agregar, buscar, verificar, modificar o eliminar firmas como texto, imágenes, códigos de barras, códigos QR, certificados digitales y sellos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar firmas en PPTX usando Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) proporciona un potente motor para detectar firmas digitales en archivos PPTX. Los desarrolladores de Python via .NET pueden mejorar sus aplicaciones con esta funcionalidad.
      
      1. Proporciona la ruta del archivo PPTX para la búsqueda de firmas.
      2. Utiliza SearchOptions para refinar los criterios de búsqueda.
      3. Llama al método Search para recuperar los resultados.
      4. Revisa la lista de firmas identificadas.
   
    code:
      platform: "python-net"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Firmas de muestra"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Inicializa un objeto Signature con la ruta del archivo del documento
            with sg.Signature('input.pptx') as signature:

                # Crea una instancia de TextSearchOptions para buscar en todas las páginas
                options = sg.TextSearchOptions()
                options.AllPages = True

                # Ejecuta una búsqueda para localizar cualquier firma basada en texto en el documento
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # Compila una lista de firmas encontradas para una revisión detallada
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Una plataforma completa de firma de documentos"
  description: "Experimenta una solución de firma poderosa y rica en funciones que asegura tus documentos con múltiples tipos de firma, abarcando varios formatos de archivo."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Buscar y gestionar firmas"
  features:
    # feature loop
    - title: "Firmar y asegurar documentos comerciales"
      content: "Agrega firmas electrónicas en cualquier parte de un documento. GroupDocs.Signature admite múltiples tipos de firma, incluyendo texto, imágenes, códigos de barras, metadatos, sellos y certificados digitales, garantizando la autenticidad y seguridad del documento."

    # feature loop
    - title: "Gestión integral de firmas"
      content: "Una vez que un documento está firmado, utiliza la función de búsqueda para encontrar todas las firmas incrustadas. Puedes modificar o eliminar firmas según sea necesario, dándote control total sobre la integridad del documento."

    # feature loop
    - title: "Asegurar la integridad del documento"
      content: "Utiliza herramientas avanzadas para gestionar metadatos ocultos dentro de los documentos. Agrega o elimina metadatos y aplica certificados digitales para proteger tus documentos de cambios no autorizados, asegurando su autenticidad."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buscar firmas de imagen"
      content: |
        Este ejemplo demuestra cómo encontrar una firma de imagen dentro de un documento específico.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Pasa el documento fuente al constructor
              with sg.Signature('input.pptx') as signature:

                    # Busca cualquier firma basada en texto
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # Muestra las propiedades detalladas de las firmas identificadas
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "Copiar"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Signature de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Funciones principales"
    exclude: "search"
    description: "Nuestra API ofrece una flexibilidad extensa, permitiendo a los usuarios firmar documentos y realizar operaciones posteriores a la firma como búsqueda, verificación y edición de firmas."
    items: 
          
        # operation loop 1
        - name: "Firmas electrónicas"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "Agrega varios tipos de firmas a formatos de archivo soportados"

        # operation loop 2
        - name: "Agregar texto a documentos"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "Mejora el contenido del documento con firmas de texto personalizables"

        # operation loop 3
        - name: "Firmas de imagen"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "Coloca cualquier imagen en cualquier posición dentro de un documento"

        # operation loop 4
        - name: "Generar códigos de barras"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "Crear e insertar varios códigos de barras en documentos soportados"

        # operation loop 5
        - name: "Generar códigos QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Generar y utilizar códigos QR para la firma de documentos"
          
        # operation loop 6
        - name: "Certificados digitales"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "Asegura negocios y firma documentos con certificados digitales"

        # operation loop 7
        - name: "Firmas de sello"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "Utiliza el Constructor de Sellos para crear sellos personalizados redondos o cuadrados"
          
        # operation loop 8
        - name: "Buscar firmas"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "Ubica cualquier firma previamente añadida dentro de un documento"
          
        # operation loop 9
        - name: "Verificación de firmas"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "Verifica la autenticidad de las firmas después de que se han aplicado"
          
        # operation loop 10
        - name: "Modificar firmas"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "Edita fácilmente una variedad de firmas dentro de un documento"
          
        # operation loop 11
        - name: "Eliminar firmas"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "Remueve una amplia gama de firmas aplicadas previamente"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Extraer firmas de múltiples formatos de archivo"
    exclude: "PPTX"
    description: "La API de GroupDocs.Signature for Python via .NET te permite extraer y gestionar firmas de una amplia variedad de formatos de documento. Recupera fácilmente las firmas incrustadas de los principales tipos de archivos para un análisis o procesamiento posterior."
    items: 
          
        # format loop 1
        - name: "Buscar firmas en PDF"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 2
        - name: "Encontrar firmas en DOCX"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Documento XML Abierto de Microsoft Word"
          
        # format loop 3
        - name: "Encontrar firmas en PPTX"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "Presentación XML Abierta de PowerPoint"
          
        # format loop 4
        - name: "Buscar firmas en XLSX"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Hoja de Cálculo XML Abierto de Microsoft Excel"


          

---