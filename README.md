Perceptrón Simple — Aprobación Preliminar de CréditosImplementación desde cero en Python de un Perceptrón Simple aplicado a un caso de negocio bancario para automatizar la aprobación preliminar de créditos evaluando el ingreso mensual y el historial crediticio de los solicitantes.📋 Objetivo del LaboratorioImplementar desde cero una neurona artificial (perceptrón simple) para resolver un problema de clasificación binaria linealmente separable y comprender su mecanismo de aprendizaje iterativo mediante el ajuste de pesos y bias.🏦 Caso de NegocioUn banco desea automatizar la evaluación preliminar de solicitudes de crédito basándose en dos variables de entrada:Ingreso mensual (valor numérico escalado).Historial crediticio (1 = buen historial, 0 = mal historial / sin historial).La salida esperada es:1: Crédito Aprobado.0: Crédito Rechazado.🗂️ Estructura del Proyectoperceptron-simple/
├── .github/
│   └── workflows/
│       └── ci.yml              # Pipeline de Integración Continua (GitHub Actions)
├── src/
│   ├── __init__.py             # Inicializador del paquete Python
│   ├── dataset.py              # Datos de entrenamiento del caso de negocio
│   └── perceptron.py           # Implementación de la clase Perceptron
├── tests/
│   └── test_perceptron.py      # Pruebas unitarias con pytest
├── main.py                     # Script principal de entrenamiento y predicción
└── README.md                   # Documentación del proyecto
🛠️ Tecnologías y HerramientasLenguaje: Python 3.12+Pruebas Unitarias: pytestControl de Versiones: Git & GitHubCI/CD y Calidad: GitHub Actions & SonarCloud🚀 Instalación y Ejecución1. Clonar el repositoriogit clone https://github.com/arnold-ucv/si-lab12-Perceptr-n-Simple.git
cd si-lab12-Perceptr-n-Simple
2. Ejecutar el modelo principalEntrena el perceptrón con el conjunto de datos y evalúa un nuevo solicitante con ingreso 9 y buen historial 1:python main.py
Salida esperada: 1 (Crédito aprobado).3. Ejecutar las pruebas unitariaspip install pytest
python -m pytest
Salida esperada: 2 passed.⚙️ Integración Continua (CI)El repositorio incluye un flujo de trabajo en .github/workflows/ci.yml que se ejecuta automáticamente ante cada push o pull_request, configurando Python 3.12 e invocando pytest para garantizar que el modelo pase todas las validaciones.