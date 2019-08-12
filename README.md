### Practica-N1
SISTEMAS EMPRESARIALES
> ###  1 ¿ Explique que son los sistemas empresariales?
>
 ####     Es un sistema que tiene impacto  muy importante en el funcionamiento
 ####     de la programacion o del negocio y cuya falta traeria graves problemas.
>
> ###  2 Describa cuales son las caracterizticas mas importantes de una aplicacion empresarial
>
####     Acceso a base de datos , operaciones transaccionales cumple con las propiedades ACID
####     otra caracteriztica es que son escalables y tienes escalabilidad vertical como horizontal
####     otra carcateriztica es que siempre deben brindar un servicio disponible sin parar
####     tambien son seguras no cualquier usuario pueden acceder a otro lugar sin tener permiso
####     permiten integracion con otras tecnologias, tienen una arquitectura multicapa.
>
> ###  3 Investigue y proponga cinco instituciones que requiriran aplicaciones de mision critica.
> ###    Justifique su respuesta.
* #### 1) correo electrónico
#### un elemento vital en la comunicación corporativa, cuya caída parece 
#### convertir todo en un caos. En  el caso de las aplicaciones de nivel operativo puede ser aún peor,
#### pues puede quedar detenida la actividad principal de la organización,
#### con todas las consecuencias que esto implica para el negocio.
* #### 2) ministerio de salud 
#### el cual necesitaria una aplicacion que tenga escalabilidad porque siempre va ir
#### en forma de crecimiento los usuarios la natalidad por ejemplo, debera ser flexible 
#### para los cambios de actualizacion que habria, debera tener seguridad 
#### no cualquier persona solo personal autorizado puede tener los datos e informacion de las personas 
#### que utilizen tal aplicacion. 
* #### 3) universidad publica de el alto 
#### necesitaria una aplicacion de mision critica ya que el manejo de recursos economicos y 
#### humanos debe ser transparente debe tener total flexibilidad y sobre todo seguridad no 
#### debe existir ninguna vulneracion de sus datos ademas que debe ser presiso y eficiente.
* #### 4) manaco
#### la zapateria manaco deberia tener una aplicacion de misison critica 
#### ya que deberia tener accesibilidad de ver los modelos y precios que ofrecen a sus usuarios 
#### y poder venderlos ofrecerlos via online por lo tanto deberia tener flexibilidad a crecer
#### y tener seguridad para q no puedan vulnerar sus datos ademas de eso ser escalable.
* #### 5) helados panda
#### deberia acceder a una aplicacion de mision critica para poder promocionar sus helados
#### y tener mas acercamiento con las personas y poder vender sus productos de manera online
#### publicando sus precios y sabores.
>    
> ###  4 Explique cuales son las diferencias entre escalabilidad horizontal y escalabilidad vertical
+ ####   la escalabilidad horizontal se refiere al incremento de componentes.
+ ####   la escalabilidad vertical se refiere a actualizaciones o modernizacion de componentes existentes.
>
> ###  5 Que es un servidor web y un servidor de aplicaciones
>
+ ####   un servidor web es un programa informático que procesa una aplicación del lado del servidor, 
####   realizando conexiones bidireccionales o unidireccionales y síncronas o asíncronas con el cliente
####   y generando o cediendo una respuesta en cualquier lenguaje o Aplicación del lado del cliente.
>
+ ####   Un servidor de aplicacion es un dispositivo de software que proporcionan servicios de aplicación 
####   a las computadoras cliente.
####   Generalmente gestiona la mayor parte (o la totalidad) de las funciones de la lógica de negocio
####   y acceso a los datos de la aplicación.
>
> ###  6 Con un grafico explique como funciona el protocolo HTTP
![Alt text](https://user-images.githubusercontent.com/53720544/62845954-5810eb00-bc9a-11e9-8c5b-6b06e6f86f88.gif)

>
> ###  7 Explique los elementos importantes de REQUEST EN HTTP
>
+ #### elementos clave de la secuencia de solicitud
+ #### Método http (la acción a realizar)
+ #### la página para acceder (una url)
+ #### parámetros de forma (como argumentos para un método)
+ #### facilita todos los datos de la solicitud actual a través HTTP Request,
#### un objeto sobre el que podremos consultar información sobre el cliente 
#### que realiza la solicitud y datos que pueda estar enviando.
>
> ### 8 Explique los elementos importantes de RESPONSE EN HTTP
>
+ #### Elementos clave de la corriente de respuesta
+ #### Un codigo de estado (Para si la solicitud fue exitosa)
+ #### tipo de contenido (TEXTO, IMAGEN, HTML, ETC)
+ #### El contenido (EL HTML REAL, IMAGEN, ETC)
+ #### Tienen como cometido imprimir en el documento HTML generado un mensaje o valor de variable. 
#### Este método es tan comúnmente utilizado que existe una abreviación del mismo de manera
#### a facilitar su escritura:
>
+ #### Otro elemento interesante de este objeto Response es el método Redirect. 
#### Este método nos permite el enviar automáticamente al internauta a una página
#### que nosotros decidamos.
> 
> ### 9 Describe con un grafico la arquitectura JAVA EE
####
>
> ### 10 Explique que son los contenedores, componentes, y servicios de JAVA EE
>
#### Un contenedor es un entorno de ejecucion que provee al componente
#### una serie de servicios.
+ ### java EE define tipos de contenedores los cuales son:
   * contenedor web
   * contenedor de negocio (o de EJBs)
#### Un componente es una unidad de software que forma parte
#### de una aplicación
+ ### Java EE define los siguientes tipos de componentes:
   * Componente cliente: Cliente AWT, Swing, Applet y
     navegador Web
   * Componente web: Servlet, JSP y JSF
   * Componente de negocio: EJB
+ ### Cada tipo cubre necesidades concretas y se basan en APIs
     especificas.
#### Son los servicios que deben ofrecer los contenedores Java EE.
#### Java EE define los siguientes servicios:
   * De directorio: para la indexación y búsqueda de
     componentes y recursos
   * De despliegue: para poder personalizar los componentes y
     recursos
   * De transaccionalidad: para poder ejecutar distintas acciones
   * en una misma unidad transaccional
   * De seguridad: para poder autenticar y autorizar a los
     usuarios de la aplicación
   * De acceso a datos: para facilitar el acceso a Bases de Datos
   * De conectividad: para poder acceder fácilmente a distintos EIS
   * De mensajería: para poder comunicarse con otros componentes, aplicaciones o EIS
> ### 11 Investigue los métodos más utilizados de las clases HttpServlet, 
> ### HttpServletRequest y HttpServletResponse, y para cada uno de los métodos muestre un ejemplo. 

#### public abstract class HttpServlet extends GenericServlet: 
#### Es la clase de la cual se debe extender para crear un servlet HTTP.
#### De la clase que extiende obtiene los métodos ya definidos además de los cuales define:
* doGet(HttpServletRequest req, HttpServletResponse resp): Es el método llamado para procesar información que haya sido enviado con el método GET. Este método es llamado concurrentemente para cada cliente por lo que hay que estar atento por posibles variables compartidas que causen problemas.
* doPost(HttpServletRequest req, HttpServletResponse resp): Ídem al anterior pero para el método POST, en general se implementa sólo un método y el otro lo referencia.



