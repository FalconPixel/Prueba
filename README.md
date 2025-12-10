# 🟠🔵 Sumo Balls 2D — Mini Battle Game

**Sumo Balls 2D** es un juego competitivo rápido donde **dos jugadores** controlan bolas que deben **empujarse fuera de la arena**.  
¡Quien cae primero, pierde! 🥊⚡

Este proyecto está hecho con **Unity 2D** e incluye mecánicas simples pero muy divertidas como movimiento físico, cámara dinámica y una **arena que se encoge como en un battle royale**.

---

## 🎮 Características del Juego

### 🧩 Jugabilidad
- Dos jugadores controlan una bola cada uno:
  - 🔵 **Jugador Azul** → WASD  
  - 🟠 **Jugador Naranja** → Flechas
- Empuja al otro jugador usando fuerza física realista.
- Si un jugador cae de la plataforma → **pierde la ronda**.

### 📉 Arena que se encoge
La plataforma central se reduce con el tiempo, obligando a los jugadores a enfrentarse más rápido.

- Encogimiento suave y progresivo.
- Tamaño mínimo configurable.
- Añade tensión a cada partida.

### 🎥 Cámara Inteligente
- Sigue el punto medio entre ambos jugadores.
- Suavizado configurable.
- Mantiene la acción centrada y limpia.

---

## 🛠️ Scripts Principales

### **MovimientoBola2D.cs**
Controla la fuerza de movimiento de cada jugador usando:
- WASD  
- Flechas  
- Física con Rigidbody2D  

Incluye opción para elegir tipo de control desde el Inspector.

---

### **CameraController.cs**
La cámara:
- Se mueve suavemente hacia el punto medio entre los dos jugadores.
- Mantiene la profundidad fija (Z = -10).
- Opcionalmente ajusta el zoom según la arena.

---

### **ArenaShrinker.cs**
Sistema de encogimiento de la arena:
- Reduce la escala del objeto “Arena”.
- Velocidad y tamaño mínimo configurables.
- Muy sencillo de integrar.

---

## 📦 Instalación

1. Clona el repositorio:
   ```bash
git clone https://github.com/FalconPixel/Prueba.git
