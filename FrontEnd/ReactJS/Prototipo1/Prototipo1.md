Realicé un prototipo cuando tome unos cursos para ReactJS, en este utilizabamos varios tipos de arquitectura como por ejemplo: Contexts, Hooks, Componentes, entre otros.
<img width="892" height="557" alt="image" src="https://github.com/user-attachments/assets/1e6116da-e0f2-438e-a93d-4fb656fa00d0" />
(Imagen con el ejemplo realizado)

El objetivo de este prototipo era realizar una apliación de tareas en ReactJS. Este no se conectaba a una base de datos, simplemente era algo local mostrando el uso de 
los hooks, context y otros tipos de arquitecturas. 

Como primer punto se creó un hook
<img width="542" height="112" alt="image" src="https://github.com/user-attachments/assets/8a956d78-f6cb-493f-9953-841f03d468a4" />
Este era el encargado de manejar los datos del localStorage, así las tareas creadas se almacenaban en este; con esto al ingresar nuevamente las tareas seguían ahí 
hasta que se borraran datos de navegación; en este se utilizaron los states, esto para ir guardando los datos que se obtenían del localStorage y poder actualizar los datos 
en la aplicación sin necesidad de recargar la página. De igual manera se utilizó el useEffect para la ejecución controlada.
<img width="904" height="486" alt="image" src="https://github.com/user-attachments/assets/4ecbe018-7d52-45c8-9427-f740cb8a99b2" />

Después se creó un contexto general, este era el encargado de almacenar las variables globales con datos relavantes, con esto era más fácil acceder a valores y a states o
hooks como el del localStorage
<img width="742" height="567" alt="image" src="https://github.com/user-attachments/assets/deb0ddac-997e-4551-87d4-cc9e0b4caefe" />

De igual manera se utilizó loadingSkeleton, este era el encargado de dibujar la pantalla de carga, la variable era de tipo state en el contexto global, así se podía acceder
a ella desde cualquier parte del proyecto, activando o desactivando esta, al hacerlo el loader aparecía.
<img width="740" height="423" alt="image" src="https://github.com/user-attachments/assets/1a2ebc71-860f-4add-95e8-5f6251eba54e" />
<img width="395" height="421" alt="image" src="https://github.com/user-attachments/assets/afcdea98-9b16-4e42-9e71-ffbb42362dd5" />

De igual se creaó un modal, este no estaba dentro del contexto principal, por lo tanto, se utilizó portal para poder ingresar a el y poder abrirlo, este modal fue creado para
mostrar la descripción de la tarea al darle click.
<img width="583" height="342" alt="image" src="https://github.com/user-attachments/assets/889083d1-318d-4221-b673-f263082898ec" />
<img width="702" height="456" alt="image" src="https://github.com/user-attachments/assets/169ed975-abf9-4f48-a073-62dce86272a1" />´

Por ultimo se crearon los componentes, estos contenían toda la lógica para realizar la busqueda de los datos, para agregar la tarea, para eliminarla, para ingresar al contexto 
general, entre otras cosas.
<img width="808" height="461" alt="image" src="https://github.com/user-attachments/assets/508a3d27-e900-4b69-bea5-bb85720e70df" />
<img width="678" height="206" alt="image" src="https://github.com/user-attachments/assets/11f0b269-adf6-402a-b6ce-2a7a04ad7533" />
<img width="715" height="154" alt="image" src="https://github.com/user-attachments/assets/afc7d2b0-e3ee-4f54-b72d-49addac57a76" />

