# Aprende json
> winkler-palacios
---

# 🟧 **CURSO COMPLETO DE JSON — Desde cero hasta nivel API**

## 🚀 1. ¿Qué es JSON?

JSON = **J**avaScript **O**bject **N**otation.
Formato para **intercambiar datos** entre frontend ↔ backend.

Se usa en:

* APIs REST
* Apps móviles
* Configs
* Bases NoSQL (MongoDB)

---

# 📌 2. Reglas básicas de JSON

### ✔ Todo JSON inicia con `{ }` (objeto) o `[ ]` (lista).

### ✔ Claves SIEMPRE entre comillas dobles `" "`.

### ✔ No acepta comentarios.

### ✔ Booleanos en minúscula: `true`, `false`.

### ✔ Null: `null`.

---

# 🧱 3. Objeto básico (lo más usado)

```json
{
  "nombre": "Winkler",
  "edad": 23,
  "activo": true
}
```

---

# 🗂 4. Listas (arrays)

### ➤ Lista simple:

```json
{
  "lenguajes": ["JavaScript", "Python", "Go"]
}
```

### ➤ Lista de objetos:

```json
{
  "usuarios": [
    { "nombre": "Ana", "edad": 20 },
    { "nombre": "Winkler", "edad": 23 }
  ]
}
```

---

# 🧩 5. Objetos dentro de objetos

```json
{
  "app": {
    "nombre": "MiProyecto",
    "version": "1.0.0",
    "autor": {
      "nombre": "Infinity",
      "pais": "Perú"
    }
  }
}
```

---

# 🔢 6. Tipos de datos

```json
{
  "texto": "Hola",
  "numero": 10,
  "decimal": 3.14,
  "booleano": false,
  "nulo": null,
  "lista": [1,2,3]
}
```

---

# 📄 7. Strings con saltos de línea

```json
{
  "descripcion": "Hola\nSoy Winkler.\nJSON es fácil."
}
```

---

# 🎯 8. JSON vs JavaScript Objects

### JSON:

```json
{ "nombre": "Infinity" }
```

### JS Object:

```js
{ nombre: "Infinity" }
```

JSON **siempre** necesita comillas.

---

# 🧨 9. Errores comunes

❌ Falta una coma
❌ Comillas simples
❌ Trailing commas (coma al final)
❌ Comentarios
❌ Clave repetida

---

# 🛠 10. Validar JSON

Para comprobar si es válido:

* jsonlint.com
* jsonformatter.org

---

# 🧪 11. Convertir un JSON a string (JavaScript)

```js
JSON.stringify(objeto)
```

---

# 🔄 12. Convertir un string a JSON (JavaScript)

```js
JSON.parse(texto)
```

---

# 📦 13. JSON completo estilo API (nivel profesional)

```json
{
  "api": "exinfinite",
  "version": "1.2.0",
  "autor": {
    "nombre": "Winkler",
    "pais": "Perú"
  },
  "servidor": {
    "puerto": 3000,
    "https": true
  },
  "usuarios": [
    {
      "id": 1,
      "nombre": "Ana",
      "roles": ["admin", "editor"],
      "activo": true
    },
    {
      "id": 2,
      "nombre": "Infinity",
      "roles": ["owner"],
      "activo": true
    }
  ],
  "config": {
    "modo": "produccion",
    "cache": {
      "enabled": true,
      "ttl": 3600
    }
  }
}
```

---

# 🧱 14. JSON gigante para bases de datos (MongoDB style)

```json
{
  "_id": "679ab12c550f",
  "user": {
    "username": "winkler",
    "email": "winkler@example.com",
    "verified": false
  },
  "posts": [
    {
      "id": 101,
      "titulo": "Mi primer post",
      "likes": 120,
      "fecha": "2025-01-01T10:00:00Z",
      "tags": ["dev", "js", "life"]
    }
  ],
  "stats": {
    "followers": 3500,
    "following": 150,
    "reputacion": 98.7
  }
}
```

---

# 🌐 15. Cómo escribir JSON lo más “limpio” posible

```json
{"n":"Winkler","a":23,"ok":true}
```

(Útil para APIs pequeñas)


