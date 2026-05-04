# 📖 Pokedex API Collection

Colección de peticiones HTTP para la API **Pokedex**, construida con [Bruno](https://www.usebruno.com/). Permite gestionar Pokémon a través de un servidor local.

---

## 🚀 Base URL

```
http://localhost:8080/pokedex
```

> Asegúrate de tener el servidor corriendo localmente antes de ejecutar las peticiones.

---

## 📋 Endpoints

### 1. Create Pokemon
| Campo   | Valor                          |
|---------|--------------------------------|
| Método  | `POST`                         |
| URL     | `http://localhost:8080/pokedex/pokemon` |
| Body    | JSON                           |

**Cuerpo de la petición:**
```json
{
  "name": "Pikachu",
  "type": "Electric",
  "level": 1,
  "weakness": "None"
}
```

**Descripción:** Crea un nuevo Pokémon en la Pokédex enviando sus datos en el cuerpo de la petición.

---

### 2. Get Pokemon
| Campo   | Valor                                     |
|---------|-------------------------------------------|
| Método  | `GET`                                     |
| URL     | `http://localhost:8080/pokedex/pokemon/{id}` |
| Body    | N/A                                       |

**Descripción:** Obtiene la información de un Pokémon específico por su ID. El ejemplo usa el ID `5`.

---

## ⚙️ Configuración

| Parámetro        | Valor   |
|------------------|---------|
| Encode URL       | ✅ Sí   |
| Timeout          | 0 ms    |
| Follow Redirects | ✅ Sí   |
| Max Redirects    | 5       |
| Auth             | Inherit |

---

## 🛠️ Requisitos

- [Bruno](https://www.usebruno.com/) (cliente de API)
- Servidor de la API Pokedex corriendo en `localhost:8080`

---

## 📂 Estructura de la colección

```
Pokedex/
├── opencollection.yml      # Configuración de la colección
├── Create Pokemon.yml      # POST - Crear un Pokémon
├── Get Pokemon.yml         # GET  - Obtener un Pokémon por ID
└── README.md               # Documentación
```

---

## 📄 Licencia

Este proyecto es de uso libre con fines educativos y de prueba.

