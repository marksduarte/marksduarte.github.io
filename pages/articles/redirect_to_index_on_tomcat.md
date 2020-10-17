# Redirecionar as requisições para index.html para SPA no Tomcat

---

1. Configure RewriteValve no arquivo `~/conf/server.xml`

` <Host name="localhost" appBase="webapps" unpackWARs="true" autoDeploy="true">`  
` <Valve className="org.apache.catalina.valves.rewrite.RewriteValve" />`  
` </Host>`

2. Crie o arquivo `rewrite.config` em `~/config/Catalina/localhost/`

`RewriteCond %{REQUEST_PATH} !-f `  
`RewriteRule ^/hello/(.*) /hello/index.html`

3. Reinicie o servidor para implementar as alterações.
