# 🛠️ Guía de Instalación y Ejecución de Actividades Multimedia

Este documento detalla los requerimientos y pasos necesarios para la instalación y despliegue local de los proyectos desarrollados para la asignatura.

**Estudiante:** Chavez Condori Jorge Abel  
**Docente:** Ph.D. Moises Martin Silva Choque  
**Fecha de Entrega:** 15 de junio de 2026  

---

## 🧰 Herramientas del Entorno de Desarrollo
* IDE Visual Studio 2026 (Lenguaje C# / Windows Forms)
* SQL Server Management Studio 2022
* Motor Gráfico Unity
* Plataformas complementarias: Mixamo, Hugging Face (MusicGen y Qwen3-TTS) y GitHub

---

## 🗄️ Paso 1: Configuración de la Base de Datos (Actividad A)
La aplicación de clasificación requiere los patrones RGB guardados en el servidor local:
1. Abra **SQL Server Management Studio 2022 (SSMS)**.
2. Conéctese a su instancia local y cree una Base de Datos llamada `texturaPracticaA`.
3. Abra una nueva pestaña de consulta (*New Query*) y ejecute íntegramente el archivo `Script BD.txt` provisto en la raíz. Esto creará la estructura `[dbo].[MuestrasTextura]` e insertará las 40 muestras calibradas de Césped, Tierra, Cemento y Asfalto.

*Nota si tiene algun error con la conexion a BD vaya a explorador de soluciones, Click derecho en `Solucion Practica_Individual_IncisoA` seguido de administrar paquetes Nu Get para la solucion, Busque `System.Data.SqlClient` e instalelo en el proyecto.
---

## 🚀 Paso 2: Ejecución de los Proyectos de Escritorio (Actividades A y B)
1. Descargue y descomprima los archivos `Practica_Individual_IncisoA.zip` o `Practica_Individual_IncisoB.zip`.
2. Haga doble clic sobre el archivo de solución con extensión `.sln` para abrirlo en **Visual Studio 2026**.
3. *Nota para la Actividad A:* Asegúrese de que la cadena de conexión (`ConnectionString`) apunte correctamente a su servidor SQL local.
4. Presione **F5** o haga clic en el botón **Iniciar** para ejecutar la interfaz de Windows Forms.

---

## 🎮 Paso 3: Ejecución de la Animación 3D (Actividad C - Unity)
1. Descomprima el paquete `Practica_Individual_IncisoC.zip`.
2. Abra **Unity Hub**, seleccione **Add project from disk** y busque el directorio descompreso.
3. Abra el proyecto con la versión instalada de su Editor Unity.
4. En el panel *Project*, ubique la carpeta `Scenes`, haga doble clic sobre la escena de la animación y presione el botón **Play (▶️)** en la parte superior central para reproducir la sincronización multimedia de audio y movimiento.
