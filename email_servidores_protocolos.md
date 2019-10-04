# Servidores de Correo. 

## Introducción
El servicio de correo electrónico es uno de lo smétodos de comunicación más usados del mundo. Lo usamos en nuestros ordenadores, móviles, tablets e incluso en nuestros relojes inteligentes. Gracias a él podemos comunicarnos con personas de todo el mundo en cuestión de segundos. Es una de las herramientas creadas que existen en Internet. 

## Servidor de correo. 
Un servidor de correo es el encargado de enviar y recibir mensajes de correo electrónico entre hosts, usuarios o servidores. Entre sus funciones se incluye el procesado de los mensajes, filtrado, almacenamiento, envío, recepción y reenvío de correos. 

## Agente de transferencia de correo (MTA). 
Un Agente de Transferencia de Correo es un software encargado de transferir el email de un host (equipo informático) a otro. Dicho de otra forma, un MTA es un sistema, software o aplicación que entrega el mail que sale de tu servidor, hacia otro MTA o MDA (Mail Delivery Agent) remoto. Es el servidor SMTP en sí
Ejemplos de MTA pueden ser: 
- Sendmail
- Qmail
- Exim
- Postfix
- Microsft Exchange Server
- Courier
- Cyrus

Puede definirse como el servidor SMTP que usamos, el que recibe datos generalmente de un MUA (Mail User Agent) para obtener el correo, y luego enviarlo al destino. 
Un MUA, o Agente de Usuario de Correo, es el que recibe el correo y envía mail usando SMTP  a través del MTA, y recibe por POP3 o IMAP. 

Ejemplos de MUA puede ser: 
- Microsoft Outlook
- Evolution
- Mozilla Thunderbird
- IncrediMail
- Squirrelmail
- Roundcube


## Agente de entrega de correo. 
Es otra de las partes del correo, el Mail Delivery Agent o agente de entrega de correo. Tiene la función recibir el correo de un MTA y llervarlo al inbox. 
Algunos formatos populares de las casillas de correo son: 
- Maildir
- Mbox

Ejemplos de MDA son: 
- Dovecot
- Procmail
- Maildrop

## Protocolos. 
Para enviar los correos entre servidor y servidor se utliza el protocolo SMTP. 
Para la comunicación entre el servidor de correo y el cliente utilizado por el usuario final se pueden utilizar 2 protocolos: 
- POP3 (Post Office Protocol)
- IMAP (Internet Messages Access Protocol)