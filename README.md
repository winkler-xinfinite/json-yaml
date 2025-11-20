
Este proyecto esta basado en el curso de JSON y YAML

---

# 🟦 **CURSO COMPLETO DE YAML — Nivel Pro en poco tiempo**

## 🚀 1. ¿Qué es YAML?

YAML = **Y**AML **A**in’t **M**arkup **L**anguage.
Un formato para **configuraciones**, más limpio que JSON y más fácil de leer.

Se usa en:

* Docker
* GitHub Actions
* Kubernetes
* CI/CD
* Configs de apps

---

# 🧱 2. Reglas básicas

### ✔ Usa espacios (NO tabulaciones)

Usualmente **2 espacios**.

### ✔ Clave: valor

```yaml
nombre: Winkler
edad: 23
activo: true
```

### ✔ Tipos de datos

```yaml
numero: 25
decimal: 3.14
texto: "Hola mundo"
booleano: true
nulo: null
```

---

# 🗂 3. Listas

### ➤ Lista simple

```yaml
lenguajes:
  - JavaScript
  - Python
  - Go
```

### ➤ Lista de objetos

```yaml
usuarios:
  - nombre: Ana
    edad: 20
  - nombre: Winkler
    edad: 23
```

---

# 🧩 4. Objetos (mapas)

```yaml
servidor:
  host: localhost
  puerto: 3000
```

---

# 🧱 5. Anidación

```yaml
app:
  nombre: MiProyecto
  baseDatos:
    host: 127.0.0.1
    usuario: root
    password: 1234
```

---

# 📌 6. Comentarios

```yaml
# Esto es un comentario
nombre: "Infinity"
```

---

# 📄 7. Bloques de texto

### ➤ Texto con saltos respetados (`|`)

```yaml
descripcion: |
  ¡Hola!
  Esto mantiene los saltos
  tal cual.
```

### ➤ Texto en una sola línea (`>`)

```yaml
mensaje: >
  Hola esto se junta
  en una sola línea.
```

---

# 🎯 8. Anchors & Aliases (Nivel Avanzado)

Sirve para **reutilizar información**.

```yaml
default: &configBase
  host: localhost
  puerto: 8080

dev:
  <<: *configBase
  modo: desarrollo
```

---

# 🔐 9. Variables con referencias (Kubernetes)

```yaml
env:
  - name: DB_USER
    valueFrom:
      secretKeyRef:
        name: db-secret
        key: username
```

---

# 🧪 10. YAML vs JSON

### JSON:

```json
{"nombre":"Winkler","edad":23}
```

### YAML:

```yaml
nombre: Winkler
edad: 23
```

YAML es **más limpio y más humano**.

---

# 🛠 11. Ejemplo REAL completo (como los de APIs)

```yaml
app:
  nombre: exinfinite
  version: 1.0.0
  entorno: produccion

servidor:
  puerto: 3000
  ssl: true

baseDatos:
  tipo: postgresql
  host: db.exinfinite.com
  usuario: winkler
  password: supersecreto
  replicas:
    - instancia1
    - instancia2

docker:
  imagen: exinfinite/api:latest
  puertos:
    - 80:3000

logs:
  nivel: info
  ruta: /var/log/app.log
```

---

# 🧰 12. Validar YAML

Para comprobar que tu archivo está bien:

* yamlchecker.com
* yamlvalidator.com

---

# 🧨 13. Errores comunes

- ❌ Usar TAB
- ❌ No respetar indentación
- ❌ Mezclar tipos en listas
- ❌ Duplicar claves

