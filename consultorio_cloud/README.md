# BeautyClinic — Historia Clínica

Aplicación de escritorio para gestión de historia clínica de consultorio estético.
Funciona completamente **sin internet**, los datos se guardan localmente.

---

## Instalación y uso

### Requisitos
- Python 3.8 o superior → https://python.org/downloads
  - ⚠️ Durante la instalación de Python, tildar **"Add Python to PATH"**

### En Windows
1. Doble clic en `iniciar.bat`
2. La primera vez instala Flask automáticamente (tarda ~30 segundos)
3. Se abre el navegador con la app en http://localhost:5000

### En Mac / Linux
1. Abrir terminal en esta carpeta
2. Ejecutar: `chmod +x iniciar.sh && ./iniciar.sh`
3. Se abre el navegador con la app en http://localhost:5000

---

## Funcionalidades

- **Pacientes**: Ficha completa con datos personales, alergias, fotos
- **Agenda**: Calendario de turnos, confirmación, duración
- **Historial clínico**: Registro de todas las sesiones con detalle técnico
- **Pagos y caja**: Ingresos, egresos, métricas mensuales, múltiples métodos de pago

---

## Dónde se guardan los datos

En la carpeta `instance/consultorio.db` — es una base de datos SQLite (un solo archivo).

**Para hacer backup**: copiar ese archivo a un pendrive o Google Drive periódicamente.

---

## Estructura del proyecto

```
consultorio/
├── app.py              ← Servidor principal
├── requirements.txt    ← Dependencias Python
├── iniciar.bat         ← Lanzador Windows
├── iniciar.sh          ← Lanzador Mac/Linux
├── templates/
│   └── index.html      ← Interfaz de usuario
└── instance/
    └── consultorio.db  ← Base de datos (se crea automáticamente)
```
