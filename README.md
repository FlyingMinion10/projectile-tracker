# 🎯 Trackeador de Proyectiles

## Descripción
Sistema de detección y seguimiento de proyectiles en tiempo real utilizando procesamiento de imágenes y Machine Learning. Captura video desde cámara o archivo, identifica proyectiles y extrae su trayectoria.

## Tecnologías utilizadas
- **Python 3.10+**
- **OpenCV** – Procesamiento de video
- **TensorFlow** o **PyTorch** – Entrenamiento de modelos
- **NumPy** – Operaciones numéricas
- **Matplotlib** – Visualización de datos

## Instalación

```bash
# Clonar el repositorio
git clone https://github.com/usuario/proyecto-detector-proyectiles.git
cd proyecto-detector-proyectiles

# Crear un entorno virtual
python -m venv venv

# Activarlo
# En Windows
.env\Scriptsctivate
# En Linux/macOS
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt
```

## Uso

```bash
# Para detección en tiempo real con cámara
python main.py --source camara

# Para detección en un video local
python main.py --source ruta/a/tu/video.mp4
```

## Entrenamiento del modelo

```bash
# Entrenar un nuevo modelo
python train.py --dataset ruta/al/dataset
```
Se requiere un dataset etiquetado donde cada proyectil esté claramente marcado en las imágenes.

## Estructura del proyecto

```
proyecto-detector-proyectiles/
│
├── main.py             # Script principal de detección
├── train.py            # Script de entrenamiento
├── model/              # Modelos entrenados y checkpoints
├── data/               # Datasets y videos de prueba
├── utils/              # Funciones de apoyo
├── requirements.txt    # Dependencias del proyecto
└── README.md           # Documentación
```

## Requisitos de hardware
- CPU con soporte AVX
- (Opcional) GPU con CUDA para acelerar el entrenamiento y la inferencia
- Cámara de alta velocidad recomendada (mínimo 60 fps)

## Licencia
Distribuido bajo la licencia [MIT](LICENSE).

## Autor
Desarrollado por **[Tu Nombre]**.
