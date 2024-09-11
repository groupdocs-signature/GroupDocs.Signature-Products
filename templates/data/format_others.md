    items: 
          
        # format loop 1
        - name: "<% dict "common-content.format-operations.{OperationLow}.pdf" %>"
          format: "PDF"
          link: "/signature/<% get "ProdCode" %>/<% get "OperationLow" %>/pdf/"
          description: "<% dict "common-content.format-formats.pdf.description" %>"
          
        # format loop 2
        - name: "<% dict "common-content.format-operations.{OperationLow}.docx" %>"
          format: "DOCX"
          link: "/signature/<% get "ProdCode" %>/<% get "OperationLow" %>/docx/"
          description: "<% dict "common-content.format-formats.docx.description" %>"
          
        # format loop 3
        - name: "<% dict "common-content.format-operations.{OperationLow}.jpeg" %>"
          format: "JPEG"
          link: "/signature/<% get "ProdCode" %>/<% get "OperationLow" %>/jpeg/"
          description: "<% dict "common-content.format-formats.jpeg.description" %>"
          
        # format loop 4
        - name: "<% dict "common-content.format-operations.{OperationLow}.pptx" %>"
          format: "PPTX"
          link: "/signature/<% get "ProdCode" %>/<% get "OperationLow" %>/pptx/"
          description: "<% dict "common-content.format-formats.pptx.description" %>"
          
        # format loop 5
        - name: "<% dict "common-content.format-operations.{OperationLow}.xlsx" %>"
          format: "XLSX"
          link: "/signature/<% get "ProdCode" %>/<% get "OperationLow" %>/xlsx/"
          description: "<% dict "common-content.format-formats.xlsx.description" %>"


          
