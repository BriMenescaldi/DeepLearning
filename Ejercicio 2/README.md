# **Detector de Gestos: Piedra, Papel o Tijeras**

Este proyecto utiliza Python y un modelo de inteligencia artificial para detectar los gestos de mano que representan **Piedra**, **Papel** y **Tijeras**. ¡Perfecto para interactuar de forma divertida con tu computadora! 🖐️🤘✂️

## **Pasos para Configurar y Ejecutar el Proyecto**

### 1. **Crear un Entorno Virtual**
Primero, asegúrate de tener instalado **Python 3.11**. Luego, crea un entorno virtual ejecutando el siguiente comando en tu terminal:
```bash
python3.11 -m venv env
```

### 2. **Activar el Entorno Virtual**
Activa el entorno virtual según tu sistema operativo:

- **En Windows**:
  ```bash
  .\env\Scripts\activate
  ```

- **En MacOS/Linux**:
  ```bash
  source env/bin/activate
  ```

### 3. **Actualizar `pip`**
Una vez activado el entorno, actualiza el gestor de paquetes `pip` con el siguiente comando:
```bash
pip install --upgrade pip
```

### 4. **Instalar las Librerías Requeridas**
Instala todas las dependencias necesarias desde el archivo `requirements.txt`:
```bash
pip install -r requirements.txt
```

### 5. **Ejecutar los Archivos del Proyecto**

#### a) **Grabar un Nuevo Dataset**
Ejecuta el archivo `record-dataset.py` para capturar y grabar un nuevo dataset con tus propios gestos:
```bash
python record-dataset.py
```

#### b) **Entrenar el Modelo**
Usa el script `train-gesture-classifier.py` para entrenar el modelo con el dataset generado:
```bash
python train-gesture-classifier.py
```

#### c) **Usar el Modelo**
Finalmente, ejecuta el archivo `rock-paper-scissors.py` para probar el modelo y detectar gestos en tiempo real:
```bash
python rock-paper-scissors.py
```

## **⚠️ Importante**
  
> Al trabajar en un entorno virtual (**venv**), es **obligatorio actualizar manualmente las rutas** en los scripts que guardan o cargan el modelo, el dataset y otros archivos relacionados.  
> **No se pueden usar rutas relativas** directamente debido a las configuraciones específicas del entorno virtual.  
> Asegúrate de especificar las rutas absolutas adecuadas según tu sistema.

---

## **Demostraciones**

### **Entrenamiento del Modelo**
El modelo se entrenó con una arquitectura sencilla y datos etiquetados cuidadosamente. Aquí puedes ver una muestra del proceso de entrenamiento:

![Entrenamiento del Modelo](<emojis and other/model_train.jpg>)

### **Resultados de Detección**
Aquí te mostramos cómo el modelo identifica los gestos de mano:

- **Piedra**  
  ![Piedra](<emojis and other/piedra.gif>)

- **Papel**  
  ![Papel](<emojis and other/papel.gif>)

- **Tijeras**  
  ![Tijeras](<emojis and other/tijera.gif>)