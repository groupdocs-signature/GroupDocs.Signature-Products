<% configRef "..\\configs\\search\\config_qrcode.yml" %>
<% set "Operation" (capitalize (get "operation")) %>
<% set "Signaturetype" (capitalize (get "signaturetype")) %>
<% set "Fileformat" (capitalize (get "fileformat")) %>
<% set "ProductName" (dict "products.{product}.name") %>
<% set "ProductFullName" (dict "products.{product}.fullName") %>
<% set "ProductCode" (dict "products.{product}.code") %>
<% set "ProductUrl" (dict "products.{product}.url") %>
<% set "ProgLang" (dict "products.{product}.progLang") %>
<% set "SrcFileExt" (dict "products.{product}.srcFileExt") %>
<% set "DevEnv" (dict "products.{product}.devEnv") %>
<% set "Runtime" (dict "products.{product}.runtime") %>
<% set "RepoName" (dict "products.{product}.repoName") %>
<% set "RepoUrl" (dict "products.{product}.repoUrl") %>
<% set "OtherFormats" (dict "otherformats.qrcode") %>
<% include "..\\landings\\search\\_search.md" %>