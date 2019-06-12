=================
Email Overview
=================

Los Programas de correo electrónicos y los demonios tienen multiples roles utilizando varios protocolos:

MUA (Agente de Correo de Usuario)
==================================

        Es el papel principal de un cliente de correo electrónico. Un MUA es donde usted podra leer los correos electronicos y redactarlos a otros. El MUA utiliza el Protocolo IMAP (Protocolo de acceso a mensajes de Internet) o POP3 (Protocolo de Oficina Postal) para descargar su correo electronico.
	El Agente de Correo de Usuario: Es utilizado para manejar el flujo correos de usuario, basicamente es el repositorio final del buzon donde el usuario podrá observar sus correos entrantes y salientes en su respectiva bandeja. 

	*Algunas de las suite incluyen:*

	* Thunderbird
	* Mutt
	* Evolution
	* Outlook/Outlook Express

**MSP** (Programa de sumisión de Correo)
========================================

Es el rol que tiene su cliente de correo cuando hace click en "Enviar".
El MSP envia su mensaje al MTA (Agente de Transmision de Correo).


**MTA** (Agente de Transmision de Correo)
=========================================

Es el papel principal de su servidor de correos electrónicos. El MTA es responsable de iniciar el proceso de envio del mensaje a su destinatario. Para ello, busca al destinatario y en envia el mensaje mediante SMTP. 

Las implementaciones del Agente de Transmision de correos (MTA) se utilizan diferentes paquetes de software.

Sendmail fue una de las primeras implementaciones de SMTP. Sendmail es dificil de configurar con macros m4. La version anterior tenia problemas de seguridad.

Existen alternativas a Sendmail, Postfix es una de ellas y tiene una arquitectura caracterizada por binarions separados y division de privilegios. Es el reemplazo directo de SendMail.

**MDA** (Agente de Entrega de Correo)
=====================================

Es el rool que toma el servidor de correo electrónico cuando recibe un correo para usted, El MDA es responsable de almacenar el mensaje para su futura recuperación. El MTA Utiliza SMTP, *LMTP* (Protocolo de Transferencia de Correo Local) u otro protocolo para transferir el mensaje al **MDA**


	
