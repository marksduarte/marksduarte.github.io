1. Abra o terminal de comando (cmd) como Administrador;
2. Digite o comando no terminal de acordo com sua versão do Office:

- Office 2016 (32-bit) instalado no Windows de 32-bit

  `cscript "C:\Program Files\Microsoft Office\Office16\OSPP.VBS" /dstatus`

- Office 2016 (32-bit) instalado no Windows de 64-bit

  `cscript "C:\Program Files (x86)\Microsoft Office\Office16\OSPP.VBS" /dstatus`

- Office 2016 (64-bit) instalado no Windows de 64-bit

  `cscript "C:\Program Files\Microsoft Office\Office16\OSPP.VBS" /dstatus`

3. Serão exibidas informações sobre os detalhes da chave de licença e seus 5 últimos caracteres.

4. Você pode utilizar esses 5 últimos caracteres exibidos para remover a chave:

- Office 2016 (32-bit) instalado no Windows de 32-bit

  `cscript "C:\Program Files\Microsoft Office\Office16\OSPP.VBS" /unpkey:<LAST 5 CHARACTERS>`

- Office 2016 (32-bit) instalado no Windows de 64-bit

  `cscript "C:\Program Files (x86)\Microsoft Office\Office16\OSPP.VBS" /unpkey:<LAST 5 CHARACTERS>`

- Office 2016 (64-bit) instalado no Windows de 64-bit

  `cscript "C:\Program Files\Microsoft Office\Office16\OSPP.VBS" /unpkey:<LAST 5 CHARACTERS>`

5. Espero ter ajudado!
