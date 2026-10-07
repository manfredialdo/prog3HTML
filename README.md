
# 🌐 Entornos de Desarrollo Blindados (Codespaces + Docker)

## 💡 La Idea
Este proyecto demuestra cómo eliminar por completo la fricción del onboarding técnico en startups y agencias. En lugar de pasar horas configurando herramientas locales, creamos **Entornos como Código (EaC)** listos para usar en la nube a través de GitHub Codespaces, totalmente configurados y protegidos.

---

## 🚀 Cómo utilizar el curso

Para ejecutar este proyecto y probar el entorno automatizado en la nube, sigue estos tres sencillos pasos:

### 1. Haz un Fork de este proyecto
Para tener tu propia copia editable de este repositorio, haz clic en el botón **Fork** arriba a la derecha en la página de GitHub.

### 2. Abre el proyecto en GitHub Codespaces
Una vez en tu fork, haz clic en el botón verde **Code**, selecciona la pestaña **Codespaces** y haz clic en **Create codespace on main**. 

> ⚡ *El entorno tardará un minuto en construirse la primera vez ya que descarga el contenedor de Docker y las extensiones de productividad automáticamente.*

### 3. ¡Listo para programar!
* Abre cualquier archivo HTML (como `04_medios_y_enlaces.html`) en el editor.
* Gracias a la automatización del archivo `.devcontainer.json`, **evitamos por completo el uso de la extensión Live Server**. El entorno levantará un servidor web real en segundo plano y te abrirá la vista previa automáticamente a la derecha de tu pantalla.

---

## 🏗️ Estructura del Documento HTML

```mermaid
flowchart TD
    HTML["html (lang=es)"] --> HEAD["head"]
    HTML --> BODY["body"]

    %% Contenido de head
    HEAD --> META["meta (charset=UTF-8)"]
    HEAD --> TITLE["title: Medios y Enlaces"]

    %% Contenido de body
    BODY --> H1["h1: Ejemplo de Medios en HTML"]
    
    BODY --> H2Img["h2: Imagen"]
    BODY --> IMG["img (src=./assets/imagen.png)"]

    BODY --> H2Vid["h2: Video"]
    BODY --> VID["video (controls)"]
    VID --> SRCVid["source (video/mp4)"]

    BODY --> H2Aud["h2: Audio"]
    BODY --> AUD["audio (controls)"]
    AUD --> SRCAud["source (audio/mp3)"]

    BODY --> H2Link["h2: Enlaces"]
    BODY --> P1["p"]
    P1 --> A1["a (href=google.com)"]
    BODY --> P2["p"]
    P2 --> A2["a (href=google.com, target=_blank)"]

    %% Estilos opcionales
    classDef tag fill:#e1f5fe,stroke:#01579b,stroke-width:2px;
    class HTML,HEAD,BODY,META,TITLE,H1,H2Img,IMG,H2Vid,VID,SRCVid,H2Aud,AUD,SRCAud,H2Link,P1,A1,P2,A2 tag;
