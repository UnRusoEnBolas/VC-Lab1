## Haciendo el setup para trabajar con _virtual environments_
1. Asegurarse de estar usando la mismoa versión de python los dos, yo lo he hecho todo con Python **3.9.1**. Esto se puede mirar ejecutando el siguiente comando en la consola que estés usando:
	```
	python -V
	```
2. Crear el _environment_:
	```
	python -m venv venv
	```
	**Esto te tiene que crear una carpeta _venv_ dentro del directorio.**
3. Activar el _environment_:
	```
	./venv/Scripts/activate
	```
	**A partir de aquí debe salir "(venv)" al principio de la línea de comandos.**
4. Actualizar _pip_ para que nos instale lo mismo:
	```
	python -m pip install --upgrade pip
	```
5. Instalar los módulos desde el fichero _requirements.txt_:
	```
	pip install -r requirements.txt
	```
	Esto instala los módulos en sus versiones especificadas en el fichero (que yo he generado al acabar el _setup_ en mi máquina), así nos aseguramos de tener los mismos módulos y versiones).
6. Correr el siguiente comando:
	```
	python -m ipykernel install --name=lab1
	```
7. Iniciar _jupyter notebook_ en el navegador:
	```
	jupyter notebook
	```
	**A partir de aquí ya se puede empezar a trabajar con normalidad. Asegurarse de que el notebook que se abre esté usando "lab1" arriba a la derecha.**