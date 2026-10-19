# Análisis de experiencia estudiantil — Siglo 21

Proyecto de ciencia de datos aplicado a indicadores de experiencia estudiantil, con foco en el comportamiento histórico del Net Promoter Score (NPS) y sus principales variables asociadas. El repositorio reúne el entorno reproducible, los datos de trabajo y la notebook del análisis.

Por razones de confidencialidad, este README no reproduce el enunciado, las consignas ni los criterios de evaluación del desafío.

## Requisitos

- Python 3.11
- `pip`
- Windows PowerShell, macOS o Linux

## Crear e instalar el entorno

Desde la raíz del repositorio, crear un entorno virtual llamado `siglo21`:

### Windows PowerShell

```powershell
python -m venv environment\siglo21
environment\siglo21\Scripts\Activate.ps1
python -m pip install -r environment\requirements.txt
```

Si PowerShell impide ejecutar el script de activación, habilitarlo solo para la sesión actual y volver a activarlo:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
environment\siglo21\Scripts\Activate.ps1
```

### macOS o Linux

```bash
python3 -m venv environment/siglo21
source environment/siglo21/bin/activate
python -m pip install -r environment/requirements.txt
```

## Levantar el entorno de trabajo

Con el entorno activado, iniciar JupyterLab:

```bash
jupyter lab
```

Luego abrir la notebook `Desafio_Tecnico_Siglo_21.ipynb` y seleccionar el kernel del entorno `siglo21` si Jupyter solicita uno.

Para registrar el entorno como un kernel con nombre propio:

```bash
python -m ipykernel install --user --name siglo21 --display-name "Python (siglo21)"
```

## Desactivar el entorno

```bash
deactivate
```

## Estructura principal

```text
.
├── dataset/                         # Datos de trabajo
├── environment/
│   └── requirements.txt             # Dependencias del proyecto
└── Desafio_Tecnico_Siglo_21.ipynb  # Notebook principal
```

