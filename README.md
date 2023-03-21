WBDS_proyecto_final_La_Camp_GLCL


Alumna: Gianina Leonor Cuya Lozada 

El detalle de los comandos utilizados se encuentra en el archivo adjunto Proyecto_final_Gianina_Cuya.ipynb y fueron corridos en Jupyter 
También se adjuntaron los archivos generados por los programas utilizados: orf_finder, pyrodigal, prokka, eggmapper(en la web)


Objetivos- Primera parte

- Realizar la predicción de ORFs de la accesión NC_014976.1 del genoma completo de 'Bacillus subtilis'
- Comparar los resultados obtenidos con las herramientas orf_finder y pyrodigal para la predicción de ORFs
- Realizar la anotación del genoma con el servidor en línea prokka

Objetivos - Segunda parte

- Obtención del genoma de Bacillus subtilis accesión CP002468.1
- Predicción de los CDS del genoma de Bacillus subtilis CP002468.1
- Búsqueda de secuencias proteínicas del genoma de Bacillus subtilis CP002468.1
- Búsqueda de dominios funcionales en las proteínas relacionadas a la ruta de la subtilisina

Objetivos - Tercera parte
- Buscar en las secuencias anotadas por prokka la secuencia de de la proteina subtilisina
- Buscar en el Protein Data Bank la proteína más parecida a la secuencia de subtilisina de nuestro organismo evaluado y revisar sus características


En el terminal del Git bash
La carpeta "WBDS_Proyecto_final_La_Camp"
que contiene las subcarpetas "eggmapper", "jupyter_pyrodigal", "orf_finder", "pyrodigal"

#Subir los archivos al github
cd WBDS_Proyecto_final_La_Camp
git config --global user.name Gianina
git config --global user.email correo@hotmail.com
ls
git init
ls -al ~/.ssh
ssh-keygen -t rsa -C correo@hotmail.com
cat /c/Users/Lenovo/.ssh/id_rsa.pub

#copiar la clave que está en el archivo id_rsa.pub
#En la web de git hub, Ir a "settings", 
#clic en "SSH and  GPG keys" crear un nuevo "SSH key",  
#colocar el nombre "Title" y pegar la clave copiada en el recuadro "Key"
#clic en el recuadro verde "Add SSH Key".

#Volver al terminal y digitar:
ssh -T git@github.com

ls
git remote add origin https://github.com/glcuya/Proyecto_final_WBDS.git
git status
git add *
git status
git commit -m "proyecto"
git status
git push origin master


