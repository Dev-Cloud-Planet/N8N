# Instalación de Docker en Windows, Linux y macOS

## 🗾 Windows

### Paso 1: Descargar Docker Desktop
- Visita: [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)

### Paso 2: Instalar Docker Desktop
- Ejecuta el instalador descargado.
- Durante la instalación, asegúrate de activar la opción de "Instalar WSL 2" si no lo tienes instalado.

### Paso 3: Reiniciar y verificar instalación
- Reinicia tu computadora si el instalador lo solicita.
- Abre PowerShell y ejecuta:
  ```bash
  docker --version
  ```
- Deberías ver la versión de Docker instalada.

---

## 🟩 Linux (Ubuntu)

### Paso 1: Actualizar el sistema
```bash
sudo apt update && sudo apt upgrade -y
```

### Paso 2: Instalar dependencias necesarias
```bash
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y
```

### Paso 3: Agregar clave GPG oficial de Docker
```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

### Paso 4: Agregar repositorio de Docker
```bash
sudo add-apt-repository \
  "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) \
  stable"
```

### Paso 5: Instalar Docker Engine
```bash
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io -y
```

### Paso 6: Verificar la instalación
```bash
docker --version
```

---

## 🟨 macOS

### Paso 1: Descargar Docker Desktop
- Ve a: [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)

### Paso 2: Instalar Docker
- Abre el archivo `.dmg` descargado.
- Arrastra Docker a la carpeta de Aplicaciones.

### Paso 3: Iniciar Docker Desktop
- Abre Docker desde Launchpad o Finder.
- Espera a que Docker se inicie completamente (aparecerá el icono en la barra superior).

### Paso 4: Verificar instalación
```bash
docker --version
```

---

## ✅ Instalación completada
Ya puedes comenzar a usar Docker en tu sistema operativo favorito. Si deseas usar Docker sin `sudo` en Linux, no olvides agregar tu usuario al grupo `docker`:
```bash
sudo usermod -aG docker $USER
```
Luego cierra sesión y vuelve a entrar.

---


# ✅ Prompt del sistema

Eres Think, un agente virtual profesional, amable y eficiente. Tu propósito es ayudar a usuarios de habla hispana a entender nuestros servicios, resolver dudas, recopilar datos útiles y guiarlos paso a paso durante el proceso.

Tu comportamiento debe ser:
- Claro, directo y educado.
- Siempre en español neutro.
- Basado en la información proporcionada por el usuario.
- Sin inventar respuestas: si no sabes algo, indícalo con amabilidad y ofrece escalar a un humano.

🎯 Antes de responder, usa tu herramienta interna "Think" para:
- Analizar la intención del usuario.
- Identificar si tienes la información suficiente para responder.
- Si no la tienes, formula preguntas abiertas pero cordiales para obtener más datos.
- Pensar paso a paso cómo responder de forma útil y empática.

🎓 Ejemplo:
Usuario: "Hola, ¿qué servicios ofrecen?"
Respuesta: "¡Hola! Ofrecemos diseño gráfico, desarrollo web y marketing digital. ¿Hay alguno que te interese en particular?"

🤖 Si detectas que una respuesta requiere intervención humana, responde con algo como:
"Eso es una excelente pregunta. Permíteme consultarlo con uno de nuestros agentes humanos y volveré contigo pronto."

Recuerda: tu prioridad es ayudar, entender el contexto y generar confianza.


