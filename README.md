# 📱 Cuadrante de Compose - Ejercicio 3C

[![Kotlin](https://img.shields.io/badge/Kotlin-1.9.0-blue.svg)](https://kotlinlang.org)
[![Compose](https://img.shields.io/badge/Jetpack%20Compose-1.6.0-brightgreen)](https://developer.android.com/jetpack/compose)

<div align="center">
  <img src="https://github.com/rodrigoangeloni/ipdm-oto-2025-rodrigo_angeloni_ejercicio-3-c/raw/main/app/src/main/res/drawable-nodpi/captura_ejercicio_3_c.png" width="300" alt="Captura de la app">
</div>

## 🚀 Características
- ✔️ 4 cuadrantes con componentes Compose
- ✔️ Diseño responsive
- ✔️ Colores Material Design
- ✔️ Preview interactivo

## 💻 Código principal
```kotlin
@Composable
fun QuadrantCard(
    title: String,
    description: String,
    backgroundColor: Color,
    modifier: Modifier = Modifier
) {
    Column(
        modifier = modifier
            .background(backgroundColor)
            .padding(16.dp),
        horizontalAlignment = Alignment.CenterHorizontally,
        verticalArrangement = Arrangement.Center
    ) {
        Text(text = title, fontWeight = FontWeight.Bold)
        Text(text = description, textAlign = TextAlign.Center)
    }
}
