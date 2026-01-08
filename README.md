# 🐱 MishiGPT - Gatito Virtual con IA

<div align="center">
  <img src="lib/images/logo.png" alt="MishiGPT Logo" width="200"/>
  
  ### 💫 Tu compañero digital inteligente y adorable
  
  [![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
  [![Dart](https://img.shields.io/badge/Dart-3.0+-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)
  [![Supabase](https://img.shields.io/badge/Supabase-Backend-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com)
  [![IA](https://img.shields.io/badge/IA-Groq%20LLM-FF6B35?style=for-the-badge&logo=openai&logoColor=white)](https://groq.com)
</div>

---

## 📖 Descripción

**MishiGPT** es una aplicación móvil innovadora que combina la magia de un **gatito virtual interactivo** con el poder de la **Inteligencia Artificial**. Diseñada especialmente para niños de 3 a 12 años, MishiGPT no es solo una mascota virtual: es un **compañero inteligente** que aprende, juega, enseña y protege.

### 🌟 ¿Qué hace especial a MishiGPT?

- 🧠 **IA Conversacional**: Mishi responde preguntas, cuenta historias y enseña de forma natural
- 🎮 **Mascota Virtual**: Cuida a tu gatito alimentándolo, jugando y llevándolo a dormir
- 💬 **Chat Inteligente**: Conversaciones adaptadas a la edad del niño
- 🗣️ **Voz Interactiva**: Habla con Mishi usando tu voz (Speech-to-Text y Text-to-Speech)
- 🎨 **Interfaz Adorable**: Diseño colorido y animaciones encantadoras
- 🔒 **Seguro para Niños**: Contenido apropiado con filtros de seguridad

---

## ✨ Características

### 🏠 Sistema de Habitaciones
- **🍽️ Comedor**: Alimenta a Mishi con diferentes comidas
- **🛋️ Sala**: Juega e interactúa con tu gatito
- **🛏️ Dormitorio**: Lleva a Mishi a dormir cuando esté cansado

### 🎭 Sistema de Estados
- **😋 Hambre**: Mishi necesita ser alimentado regularmente
- **😴 Sueño**: Lleva a tu gatito a dormir cuando esté cansado
- **😊 Felicidad**: Mantén a Mishi contento con atención y cuidados

### 💭 Chat con IA
- Respuestas personalizadas usando el nombre del niño
- Explicaciones adaptadas a la edad del usuario
- Mantiene la magia infantil (Santa Claus, Ratón Pérez, etc.)
- Detección y apoyo en situaciones sensibles (bullying, tristeza)
- Ciencia y educación de forma divertida

### 🎤 Interacción por Voz
- Reconocimiento de voz (Speech-to-Text)
- Síntesis de voz (Text-to-Speech)
- Conversaciones naturales con Mishi

### 🎵 Efectos de Sonido
- Sonidos de gatito (ronroneo, maullidos)
- Efectos de interacción
- Ambiente inmersivo

---

## 🛠️ Tecnologías

### Frontend
- **Flutter 3.0+**: Framework multiplataforma
- **Dart 3.0+**: Lenguaje de programación
- **Riverpod**: Gestión de estado
- **Google Fonts**: Tipografías personalizadas
- **Lottie & Flutter Animate**: Animaciones fluidas

### Backend
- **Supabase**: Backend as a Service
  - Autenticación de usuarios
  - Base de datos PostgreSQL
  - Row Level Security (RLS)
- **Groq API**: Modelo de lenguaje LLM para conversaciones inteligentes

### Integraciones
- **Speech-to-Text**: Reconocimiento de voz
- **Text-to-Speech**: Síntesis de voz
- **Shared Preferences**: Almacenamiento local
- **HTTP/Dio**: Cliente HTTP para APIs

---

## 🚀 Instalación

### Prerrequisitos

1. **Flutter SDK** (3.0 o superior)
   ```bash
   flutter --version
   ```

2. **Dart SDK** (3.0 o superior)

3. **Android Studio** o **VS Code** con extensiones de Flutter

4. **Git**

### Pasos de Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/ChrispinSantacruz/MishiGPT---Version-Alpha.git
   cd MishiGPT---Version-Alpha
   ```

2. **Instalar dependencias**
   ```bash
   flutter pub get
   ```

3. **Configurar variables de entorno**
   
   Copia el archivo de ejemplo y configura tus credenciales:
   ```bash
   cp lib/core/config/env.example.dart lib/core/config/env.dart
   ```
   
   Edita `lib/core/config/env.dart` con tus credenciales:
   ```dart
   class Env {
     static const String supabaseUrl = 'TU_SUPABASE_URL';
     static const String supabaseAnonKey = 'TU_SUPABASE_ANON_KEY';
     static const String groqApiKey = 'TU_GROQ_API_KEY';
     static const String groqApiUrl = 'https://api.groq.com/openai/v1/chat/completions';
     static const String groqModel = 'llama3-8b-8192';
   }
   ```

4. **Configurar Supabase**
   
   Ejecuta el script SQL en tu proyecto de Supabase:
   ```bash
   # Abre supabase_setup_fix.sql en el SQL Editor de Supabase
   # y ejecuta el script
   ```

5. **Ejecutar la aplicación**
   ```bash
   flutter run
   ```

---

## ⚙️ Configuración

### 1. Supabase Setup

1. Crea una cuenta en [Supabase](https://supabase.com)
2. Crea un nuevo proyecto
3. Ve a **Settings** → **API** y copia:
   - URL del proyecto
   - Anon/Public key
4. Ejecuta el script `supabase_setup_fix.sql` en el **SQL Editor**

### 2. Groq API Setup

1. Crea una cuenta en [Groq](https://console.groq.com)
2. Genera una API Key
3. Copia la key en tu archivo `env.dart`

### 3. Permisos de la App

Asegúrate de tener los permisos necesarios en `AndroidManifest.xml`:
- `INTERNET`: Para conexión a APIs
- `RECORD_AUDIO`: Para reconocimiento de voz
- `MODIFY_AUDIO_SETTINGS`: Para efectos de sonido

---

## 📱 Uso

### Registro y Login
1. Abre la aplicación
2. Regístrate con email, nombre y edad (3-12 años)
3. Inicia sesión con tus credenciales

### Interacción con Mishi
1. **Alimentar**: Ve al comedor y selecciona comida
2. **Dormir**: Lleva a Mishi al dormitorio cuando esté cansado
3. **Jugar**: Interactúa en la sala para mantener feliz a Mishi
4. **Chatear**: Habla con Mishi sobre cualquier tema
5. **Voz**: Usa el botón de micrófono para hablar con Mishi

---

## 📂 Estructura del Proyecto

```
lib/
├── core/                      # Configuración y utilidades
│   ├── config/               # Variables de entorno
│   ├── constants/            # Constantes de la app
│   └── utils/                # Utilidades y helpers
├── data/                     # Capa de datos
│   ├── datasources/          # Fuentes de datos (Supabase)
│   ├── repositories/         # Implementación de repositorios
│   └── services/             # Servicios (IA, sonido, etc.)
├── domain/                   # Lógica de negocio
│   ├── entities/             # Entidades del dominio
│   ├── repositories/         # Interfaces de repositorios
│   └── usecases/             # Casos de uso
├── presentation/             # Capa de presentación
│   ├── providers/            # Providers de Riverpod
│   ├── screens/              # Pantallas de la app
│   └── widgets/              # Widgets reutilizables
└── main.dart                 # Punto de entrada
```

---

## 🎨 Características de la IA

MishiGPT utiliza un modelo de lenguaje avanzado con una personalidad única:

- 🌈 **Mantiene la magia infantil**: Respeta la ilusión de Santa Claus, hadas, etc.
- 📚 **Educativo**: Explica conceptos científicos de forma simple y divertida
- 💖 **Empático**: Detecta y apoya en situaciones emocionales difíciles
- 🛡️ **Protector**: Guía en casos de bullying o situaciones de riesgo
- 🎭 **Personalizado**: Usa el nombre del niño y adapta respuestas a su edad

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Si quieres mejorar MishiGPT:

1. Haz un Fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está en fase **Alpha**. Los derechos y licencia serán definidos próximamente.

---

## 👨‍💻 Autor

**Crispin Santacruz**

- GitHub: [@ChrispinSantacruz](https://github.com/ChrispinSantacruz)

---

## 🙏 Agradecimientos

- Flutter y la comunidad de Dart
- Supabase por el increíble BaaS
- Groq por los modelos de IA
- Todos los contribuidores y testers

---

<div align="center">
  
  ### 💝 ¿Te gusta MishiGPT? ¡Dale una estrella! ⭐
  
  **Hecho con 💖 y mucho ☕ por desarrolladores apasionados**
  
  🐱 *"¡Miau! Gracias por cuidar de mí"* - MishiGPT
  
</div>
