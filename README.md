# Aprendizaje Profundo y Visión por Computadora

## Sistema de Reconocimiento Facial para Registro de Asistencia

Este proyecto implementa un sistema de reconocimiento facial basado en redes neuronales convolucionales (CNNs) para automatizar el proceso de registro de asistencia diaria. La solución está diseñada para minimizar errores de los métodos tradicionales y optimizar el control de asistencia, asegurando registros más precisos y eficientes.

### Características principales
- **Uso de OpenCV y PyTorch** para la detección y reconocimiento facial.
- **Modelo basado en ResNet18** para la extracción de características faciales.
- **Comparación de embeddings faciales** para identificar personas con alta precisión.
- **Registro automático de asistencia** con almacenamiento en un archivo CSV.
- **Interfaz de captura de imágenes en Google Colab** para la toma de fotos en tiempo real.

### Requisitos
- Python 3.x
- Google Colab (opcional, pero recomendado para facilidad de ejecución)
- Bibliotecas necesarias:
  ```bash
  pip install opencv-python numpy torch torchvision pandas pytz
  ```

### Uso
1. **Carga y extracción de imágenes de referencia**
   - Subir un archivo ZIP con imágenes de referencia de cada persona a reconocer.
   - Extraer los embeddings faciales y almacenarlos para comparaciones futuras.

2. **Captura y reconocimiento facial**
   - Se toma una foto en tiempo real utilizando la cámara.
   - Se detectan los rostros y se comparan con la base de datos.
   - Si se encuentra una coincidencia, se registra la asistencia.

3. **Almacenamiento de registros**
   - Los datos de asistencia se guardan en `attendance_log.csv`.
   - Se incluye la fecha, hora y nombre del usuario reconocido.

### Mejoras futuras
- Optimización del umbral de similitud para mejorar la precisión.
- Implementación de una base de datos en tiempo real en lugar de archivos CSV.
- Integración con una interfaz gráfica más interactiva.

Este sistema facilita la gestión del personal y mejora la puntualidad en entornos educativos y empresariales. 🚀

