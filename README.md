# 👋 ¡Hola! Soy Gerardo Blázquez  

💻 Estudiante de DAM | Big Data & IA  
📌 Portfolio: [gcodev.es](https://gcodev.es/)  

---

## 🔷 Acerca de mí  

Soy estudiante de Desarrollo de Aplicaciones Multiplataforma (DAM) en la UAX, especializado en **Big Data e Inteligencia Artificial**.  
Me interesa el desarrollo de software eficiente, la optimización de procesos y el aprendizaje continuo.  

---

### Frontend  
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E) ![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)  

### Backend  
![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=yellow) ![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-025E8C?style=for-the-badge&logo=database&logoColor=white)  

### Cloud & Otros  
![AWS](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  
---

## 🔷 Formación  
*Grado Superior en Desarrollo de Aplicaciones Multiplataforma (DAM)**  
  **Universidad Alfonso X el Sabio (UAX)**  
  _Septiembre 2024 – Actualmente_  
  - Formación en desarrollo de aplicaciones web y móviles.  
  - Programación orientada a objetos (Java, Python, JavaScript, Kotlin).  
  - Gestión de bases de datos relacionales (MySQL, SQL).  
  - Especialización en **Big Data e Inteligencia Artificial** con proyectos prácticos.

---


## 🔷 Proyectos Destacados  

## Sistema de Recomendaciones Cruzadas  
Este proyecto surge de la necesidad de analizar las preferencias de usuario, generando recomendaciones cruzadas personalizadas entre **cuatro categorías**:  

🎬 Películas | 📺 Series | 📚 Libros | 🎮 Videojuegos  


**Descripción**  
El usuario introduce un título de referencia, selecciona su categoría y elige una o varias categorías de destino para recibir sugerencias relevantes.  


**Tecnologías y Diseño**  
- **Dataset:** unificación de datos desde Kaggle (20k+ registros).  
- **APIs externas:**  
  - TMDb → películas y series  
  - Google Books → libros  
  - RAWG → videojuegos  
- **Algoritmos:**  
  - Inicialmente se probó la librería **Sentence Transformers** con embeddings, desarrollando una versión en local con esta arquitectura.  
  - Debido a limitaciones de infraestructura en la versión gratuita de **Render**, se implementó una versión optimizada con **TF-IDF + similitud coseno**, filtrado por géneros y ponderaciones personalizadas (overview, género, palabras clave constantes).  
- **Backend:** Flask en **Render**, modularizado en GitHub.  
- **Frontend:** consumo de APIs REST con políticas CORS.

  
**Flujo de Recomendación**  
1. El usuario envía título, categoría origen y categorías destino.  
2. El backend vectoriza la descripción, filtra por género y aplica similitud.  
3. Los candidatos se seleccionan de dataset + APIs (60/40).  
4. Se validan y completan datos antes de mostrarse.  
5. El frontend presenta resultados en **cards interactivas** con imágenes, puntuación, título y año.  


**Experiencia de Usuario (UX)**  
- Carruseles horizontales de recomendaciones.  
- Barra de carga con mensajes de progreso.  
- Botón **“Buscar más”** con autoscroll horizontal.  
- Resultados en 20-40s aprox., optimizados con caché.  


**Resultados y Conclusiones**  
- Dataset enriquecido con: **6.000 películas, 7.000 series, 2.000 libros y 14.000 videojuegos**.  
- Recomendaciones precisas, relevantes y multimediales.  
- Combina **NLP, integración de APIs y arquitectura cliente-servidor**, optimizando recursos en un entorno con limitaciones (Render Free Tier).  

---


## 🔷 Contacto  
✉️ Email: gerardo.blazquez32@gmail.com
🌐 LinkedIn: [linkedin.com/in/gerardoblazquez](https://www.linkedin.com/in/gerardo-bl%C3%A1zquez-moreno-a71551195/)  
