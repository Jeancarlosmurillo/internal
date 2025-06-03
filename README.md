# internal

Colección de ejercicios en **Python** organizados en dos módulos independientes, con pruebas unitarias.

## Módulos

### `biblio/` — Gestión de una biblioteca
Lógica para adicionar y consultar títulos de libros, evitando duplicados.

- `libros.py` — modelo/almacén de libros
- `control_libros.py` — lógica de negocio (`ControlBiblioteca`)
- `test_control_libros.py` — pruebas unitarias (con mocks)

### `comida/` — Gestión de un restaurante
Modela un menú de platos y pedidos con múltiples ítems.

- `menu.py` — clases `Plato` y `Menu`
- `restaurante.py` — clases `Pedido` y `Restaurante`

## Ejecutar las pruebas

```bash
# Desde la raíz del repositorio
python -m unittest discover -s biblio -p "test_*.py"
```

## Estructura

```
internal/
├── biblio/
│   ├── libros.py
│   ├── control_libros.py
│   └── test_control_libros.py
└── comida/
    ├── menu.py
    └── restaurante.py
```
