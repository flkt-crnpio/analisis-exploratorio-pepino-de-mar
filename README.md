# pepino de mar





## uso

si ya lo tenias corriendo y nada mas pasaste a ver otra vez como dice que se 
levanta, solo necesitas iniciar el entorno virtual y levantar el notebook con 

```sh
source env/bin/activate

jupyter notebook
```

si es la primera vez que utilizas este repositorio, sigue las instrucciones.

### instrucciones

existen muchas maneras de levantar un notebook en un entorno virtual de python, 
si tienes preferencias al respecto, has como lo harías normalmente 
y pues estará de mas que te cuente que explores los archivos `.ipynb`

si aun no tienes instalado nada y no sabes ni por donde empezar, esta es, creo, 
la manera más fácil de hacerlo.

copia y pega los comandos en la terminal, en el orden en el que van apareciendo.

1. [brew](https://brew.sh/)
    ```sh
    # instalar brew
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

2. [pipx](https://pypi.org/project/pipx/)
    ```sh
    # instalar pipx con brew
    brew install pipx
    pipx ensurepath

    # optional 
    sudo pipx ensurepath --global 
    ```

3. [virtualenv](https://virtualenv.pypa.io/en/latest/user_guide.html) 
    ```sh
    # instalar viertualenv con pipx
    pipx install virtualenv
    pipx ensurepath
    ```

4. después necesitas abrir nueva terminal para que aplique el path 
para crear y activar tu entorno virutual de python

5. crear el ambiente virtual
    ```sh
    virtualenv env
    ```

6. activar el ambiente virtual
    ```sh
    source env/bin/activate
    ```
    *pa quitar el ambiente virtual utiliza `deactivate`*

7. instala las dependencias
    ```sh
    pip install -r requirements.txt
    ```

8. levanta el notebook
    ```sh
    jupyter notebook
    ```