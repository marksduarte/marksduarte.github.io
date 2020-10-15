# Deploy do arquivo WAR diretamento no Tomcat

1. Configure o usuário no arquivo de configuração tomcat-users.xml

   `<user username="username" password="secr3t" roles="manager-gui, manager-script, manager-jmx"/>`

2. Verifique o local de instalação do Maven e adicione a propriedade `<server>` no arquivo **settings.xml** do Maven. 

   `<server>`  
   ` <id>server-id</id>`  
   ` <username>username</username>`  
   ` <password>secr3t</password>`  
   `</server>`

3. Configure o Tomcat Maven Plugin no pom.xml

   `<plugin>`  
   ` <groupId>org.apache.tomcat.maven</groupId>`  
   ` <artifactId>tomcat7-maven-plugin</artifactId>`  
   ` <version>2.0</version>`  
   ` <configuration>`  
   ` <server>server-id</server>`  
   ` <url>http://localhost:8080/manager/text</url>`  
   ` <path>/app</path>`  
   ` </configuration>`
   `</plugin>`  
4. Execute o comando  

   ` mvn install tomcat7:deploy`
