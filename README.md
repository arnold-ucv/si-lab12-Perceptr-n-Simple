# Perceptrón Simple — Aprobación Preliminar de Créditos

Implementación desde cero en Python de un **Perceptrón Simple**, aplicado a un caso de negocio bancario para automatizar la aprobación preliminar de créditos mediante la evaluación de dos variables: el ingreso mensual y el historial crediticio de los solicitantes.

## 📋 Objetivo del laboratorio

Implementar desde cero una neurona artificial (Perceptrón Simple) para resolver un problema de clasificación binaria linealmente separable y comprender su mecanismo de aprendizaje iterativo mediante el ajuste de pesos (*weights*) y sesgo (*bias*).

## 🏦 Caso de negocio

Un banco desea automatizar la evaluación preliminar de las solicitudes de crédito utilizando dos variables de entrada:

| Variable | Descripción |
|---|---|
| Ingreso mensual | Valor numérico escalado que representa los ingresos del solicitante. |
| Historial crediticio | Valor binario: `1` = buen historial, `0` = mal historial o sin historial. |

**Variable de salida:**

| Valor | Resultado |
|:---:|---|
| `1` | ✅ Crédito aprobado |
| `0` | ❌ Crédito rechazado |

## 🗂️ Estructura del proyecto

```text
perceptron-simple/
│
├── .github/
│   └── workflows/
│       └── ci.yml              # Pipeline de integración continua
│
├── src/
│   ├── __init__.py             # Inicializador del paquete
│   ├── dataset.py              # Datos de entrenamiento
│   └── perceptron.py           # Implementación de la clase Perceptron
│
├── tests/
│   └── test_perceptron.py      # Pruebas unitarias con pytest
│
├── main.py                     # Entrenamiento y predicción
└── README.md                   # Documentación del proyecto
```

## 🛠️ Tecnologías y herramientas

| Tecnología | Uso |
|---|---|
| Python 3.12+ | Lenguaje de programación |
| pytest | Ejecución de pruebas unitarias |
| Git | Control de versiones |
| GitHub | Repositorio y colaboración |
| GitHub Actions | Integración continua (CI) |
| SonarCloud | Análisis de calidad del código |

## 🚀 Instalación y ejecución

### 1. Clonar el repositorio

```bash
git clone https://github.com/arnold-ucv/si-lab12-Perceptr-n-Simple.git
```

Ingresar al directorio del proyecto:

```bash
cd si-lab12-Perceptr-n-Simple
```

### 2. Ejecutar el modelo principal

Ejecutar el siguiente comando para entrenar el perceptrón y realizar una predicción:

```bash
python main.py
```

**Ejemplo de evaluación:**

- Ingreso mensual: `9`
- Historial crediticio: `1`

**Salida esperada:**

```text
1 (Crédito aprobado)
```

### 3. Ejecutar las pruebas unitarias

Instalar pytest:

```bash
pip install pytest
```

Ejecutar las pruebas:

```bash
python -m pytest
```

**Salida esperada:**

```text
2 passed
```

## ⚙️ Integración continua (CI)

El repositorio incorpora un flujo de trabajo de integración continua mediante **GitHub Actions**, configurado en el archivo:

```text
.github/workflows/ci.yml
```

Este proceso se ejecuta automáticamente cada vez que se realiza un `push` o un `pull_request` hacia el repositorio.

El flujo de trabajo contempla las siguientes actividades:

1. Configuración del entorno de ejecución con Python 3.12.
2. Instalación de las dependencias necesarias.
3. Ejecución de las pruebas unitarias mediante pytest.
4. Verificación del correcto funcionamiento del modelo.

El objetivo es garantizar que las modificaciones realizadas en el código no afecten el funcionamiento del perceptrón.

## 🎯 Resultado del laboratorio

Al finalizar este laboratorio, se habrá implementado un Perceptrón Simple capaz de aprender a partir de datos de entrenamiento y realizar clasificaciones binarias para la aprobación preliminar de solicitudes de crédito.

Asimismo, se comprenderá el funcionamiento del aprendizaje supervisado mediante el ajuste iterativo de pesos y bias, junto con la importancia de las pruebas unitarias y la integración continua en el desarrollo de software.

---

**Desarrollado por:** Arnold Edward Villanueva Huamaní

**Repositorio:** [si-lab12-Perceptrón-Simple](https://github.com/arnold-ucv/si-lab12-Perceptr-n-Simple)
