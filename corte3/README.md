# BOXCHETT

## Descripción de proyecto

BOXCHETT es una empresa tecnológica dedicada al desarrollo de un chatbot inteligente para atención al cliente.  
Su objetivo es mejorar la comunicación entre empresas y usuarios mediante sistemas automatizados disponibles 24/7.

## Información general
- Nombre: BOXCHETT   
- Área: Atención digital al cliente  
- Tipo de solución: Chatbot automatizado  
##  Objetivo del proyecto

Desarrollar un chatbot que permita automatizar la atención al cliente, reducir tiempos de respuesta y mejorar la calidad del servicio.

##  Funcionalidades

- Respuestas automáticas  
- Atención 24/7  
- Registro de consultas  
- Información clara y rápida  


###  Beneficios

- Mejor experiencia del cliente  
- Ahorro de tiempo  
- Servicio moderno  
- Uso eficiente de tecnología
# Explicación del sistema

## ¿Qué hace cada parte?

## Cliente:  
Es la interfaz que usa el usuario (por ejemplo, una página web o app). Permite enviar mensajes al chatbot y recibir respuestas.

## Servidor (Backend):
Es el encargado de procesar las solicitudes. Analiza los mensajes, aplica la lógica de negocio y genera respuestas automáticas.

## Base de datos:
Almacena la información del sistema, como el historial de conversaciones, consultas realizadas y posibles respuestas.

 ¿Qué datos maneja?

## Cliente:
-Mensajes del usuario (texto de entrada).

## Servidor:
-Procesa datos como:

-Mensajes recibidos

-Intención del usuario

-Respuestas generadas

## Base de datos:
-Guarda:

-Historial de chats

-Fecha y hora de consultas

-Datos relevantes para mejorar el servicio

## ¿Cómo se comunican?
-El cliente envía una solicitud al servidor (por ejemplo, un mensaje).

-El servidor procesa la información y consulta la base de datos si es necesario.

-La base de datos devuelve la información al servidor.

-El servidor genera una respuesta y la envía de vuelta al cliente.

## explicación breve
El diagrama muestra cómo funciona BOXCHETT a través de tres componentes: cliente, servidor y base de datos. El cliente envía mensajes al servidor, donde se procesan mediante la lógica de negocio (controladores, servicios, etc.) para generar una respuesta.
Si es necesario, el servidor consulta la base de datos para obtener o guardar información. Finalmente, la respuesta se envía de vuelta al cliente, permitiendo una comunicación automatizada y eficiente.


## Requisitos Funcionales

- **Respuesta Automática:** El sistema debe responder automáticamente a las consultas de los usuarios en un tiempo máximo de 3 segundos.  

- **Disponibilidad Continua:** El chatbot debe estar disponible para los usuarios las 24 horas del día, los 7 días de la semana.  

- **Registro de Consultas:** El sistema debe almacenar todas las consultas realizadas por los usuarios en una base de datos.  

- **Información Clara:** El chatbot debe proporcionar respuestas claras, precisas y comprensibles en cada interacción.  

- **Gestión de Preguntas Frecuentes:** El sistema debe identificar y responder automáticamente preguntas frecuentes previamente configuradas.  

- **Navegación Guiada:** El chatbot debe ofrecer opciones o menús interactivos para guiar al usuario durante la conversación.  

- **Escalamiento a Humano:** El sistema debe transferir la conversación a un agente humano cuando no pueda resolver la consulta.  

- **Atención Simultánea:** El chatbot debe atender múltiples usuarios al mismo tiempo sin afectar su rendimiento.  

- **Historial de Conversaciones:** El sistema debe permitir consultar el historial de conversaciones de cada usuario.  

- **Personalización de Respuestas:** El chatbot debe adaptar sus respuestas según el tipo de consulta o contexto del usuario.  



## Requisitos No Funcionales

- **Rendimiento:** El sistema debe garantizar un tiempo de respuesta menor a 3 segundos en el 95% de las consultas.  

- **Disponibilidad:** El sistema debe tener una disponibilidad mínima del 99% mensual.  

- **Seguridad:** El sistema debe proteger los datos del usuario mediante mecanismos de cifrado y control de acceso.  

- **Usabilidad:** El chatbot debe ser fácil de usar, permitiendo que un usuario interactúe sin necesidad de capacitación previa.  

- **Escalabilidad:** El sistema debe soportar el incremento de usuarios sin degradar su rendimiento.  

- **Compatibilidad:** El chatbot debe funcionar correctamente en navegadores web y dispositivos móviles.  

- **Confiabilidad:** El sistema debe garantizar el almacenamiento seguro y consistente de las conversaciones.

# ARQUITECTURA CHATBOTT BOXCHETT.
<img width="921" height="434" alt="image" src="https://github.com/user-attachments/assets/241d5efe-805b-44e7-83ae-2bf0a162018d" />
<img width="921" height="511" alt="image" src="https://github.com/user-attachments/assets/7c4e1678-21af-48e2-bf45-44e2dbad098d" />
<img width="921" height="452" alt="image" src="https://github.com/user-attachments/assets/7d50c793-4836-404f-860a-8fbd7db5ca9e" />

## FRONTEND.
<img width="813" height="542" alt="image" src="https://github.com/user-attachments/assets/6bdc4e2a-2e43-4566-be16-ed5a1bd1eb18" />
<img width="430" height="509" alt="image" src="https://github.com/user-attachments/assets/f4cd3048-3c99-425c-80f4-f1de2ce226c6" />

## EXPLICACION DE LA LOGICA DE NEGOCIO 
- **Controladores** Se encargan de recibir las solicitudes del usuario y enviarlas al módulo de servicios para su procesamiento.
- **Servicios** Contienen la lógica principal del chatbot. Analizan el mensaje, identifican la intención del usuario y generan la respuesta adecuada.
- **Modelos** Definen la estructura de los datos utilizados en el sistema, como Mensaje y Respuesta.
- **Rutas** Definen los puntos de acceso al sistema, como el envío de mensajes y la consulta del historial.
- **Base de datos** Gestiona el almacenamiento de la información, permitiendo guardar y consultar el historial de conversaciones.
- **Utilidades** Incluyen funciones auxiliares como el procesamiento de texto y la detección de palabras clave.
- **Configuracion** Contiene parámetros generales del sistema como la conexión a la base de datos.
## Base De Batos

<img width="921" height="607" alt="image" src="https://github.com/user-attachments/assets/c3053a3f-cf6c-4183-97a0-9c8cd23cd2c0" />

## Contexto Administrativo
El sistema BOXCHETT apoya una estructura administrativa centralizada, ya que toda la información, el procesamiento de datos y la gestión del chatbot se realizan desde un servidor principal y una base de datos central.

Esto permite que la empresa tenga un mayor control sobre la información de los usuarios, las consultas, los pedidos y el historial de conversaciones. Además, facilita la administración del sistema, la seguridad de los datos y la actualización de las funcionalidades del chatbot desde un único punto.
La estructura centralizada también ayuda a mantener una atención al cliente organizada y eficiente, permitiendo supervisar las operaciones en tiempo real y garantizar respuestas rápidas y uniformes para todos los usuarios.

Gracias a este modelo, BOXCHETT puede ofrecer un servicio automatizado disponible 24/7, optimizando los procesos operativos y mejorando la experiencia del cliente.

#




## integrantes
- Sergio Andres Mejia Alban
- Camilo Alvarez Mota
- Jhonier Fran Escobar 
   
Proyecto académico – Ingeniería de Sistemas
