# 🔧 Los Clavitos de Pablito - Sistema de Gestión eCommerce para FERREMAS

## 📘 Introducción

Este proyecto nace como respuesta al caso propuesto por la asignatura **ASY5131 - Integración de Plataformas**, cuyo objetivo es aplicar conocimientos de análisis, planificación e integración de servicios en un contexto real de transformación digital. El caso se centra en **FERREMAS**, una empresa chilena del rubro de ferretería y construcción, con presencia física en diversas regiones del país.

## 🧩 El problema

A raíz de la pandemia del COVID-19 y las restricciones de movilidad, FERREMAS enfrentó una caída significativa en sus ventas debido a la falta de un canal de venta online. La empresa operaba exclusivamente de forma presencial, lo que evidenció una necesidad urgente de modernizar sus procesos mediante la implementación de una **plataforma de comercio electrónico integrada**.

## ✅ La solución

Se propone el desarrollo de un sistema de eCommerce denominado **"Los Clavitos de Pablito"**, que responde a la necesidad de digitalizar los procesos operacionales de FERREMAS. La solución considera:

- Implementación de una **aplicación web multiplataforma** desarrollada en **Angular + Ionic**.
- Integración de múltiples roles de usuarios: Clientes, Administradores, Vendedores, Bodegueros y Contadores.
- Automatización de procesos de compra, gestión de inventario, pagos y despachos.
- Diseño de flujos de negocio a través de diagramas BPMN.
- Arquitectura basada en microservicios con APIs propias y externas.

## 🔌 Tecnologías y APIs utilizadas

### 🖥️ Frontend
- Angular 17
- Ionic Framework

### 🧠 Backend / APIs Internas
- **API de usuarios y gestión de pedidos**: desarrollada con **Express.js**.
- **API de facturación y control financiero**: implementada con **FastAPI (Python)**.

### 🌐 APIs Externas
- **API de PayPal**: integración para pagos seguros en línea.
- **API de MiIndicador.cl**: para consulta del valor actualizado del dólar y conversión automática de precios.

## 🔐 Funcionalidades principales por rol

| Rol          | Funcionalidades clave |
|--------------|------------------------|
| **Cliente**       | Registro, navegación de catálogo, carrito de compras, elección de retiro o despacho, múltiples medios de pago. |
| **Vendedor**      | Gestión de pedidos, aprobación y envío de órdenes a bodega, coordinación de despachos. |
| **Bodeguero**     | Preparación de pedidos, entrega a vendedores. |
| **Contador**      | Verificación de pagos, registro de entregas. |
| **Administrador** | Gestión de cuentas de usuarios, informes de desempeño y estrategias de venta. |

## 🗂️ Arquitectura general

El sistema está compuesto por una arquitectura modular y escalable:
- Frontend híbrido para distribución web y mobile.
- Dos APIs desarrolladas de forma desacoplada.
- Integración de servicios externos REST.
- Comunicación entre servicios vía HTTP (RESTful).

## 📥 Instalación y ejecución del proyecto

### 🔁 1. Clonar el repositorio

```bash
git clone https://github.com/usuario/los-clavitos-de-pablito.git
cd los-clavitos-de-pablito
```

---

### ⚙️ 2. Instalación de dependencias del frontend (Angular + Ionic)

```bash
cd frontend
npm install
ionic serve
```

Esto abrirá automáticamente la aplicación en [http://localhost:8100](http://localhost:8100).

---

### 🌐 3. Levantar API de Express (Node.js)

```bash
cd ../api-express
npm install
node index.js
```

- Asegúrate de tener instalado **Node.js**.
- El servidor se levantará en [http://localhost:3000](http://localhost:3000) (o el puerto definido en tu archivo de configuración).

---

### 🐍 4. Levantar API de FastAPI (Python)

```bash
cd ../api-fastapi
pip install -r requirements.txt
uvicorn main:app --reload
```

- Asegúrate de tener **Python 3.8+** y `pip` instalado.
- Por defecto, la API estará disponible en [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) (Swagger UI).

Si usas entornos virtuales en Python:

```bash
python -m venv venv
source venv/bin/activate  # En Linux/Mac
venv\Scriptsctivate     # En Windows
```

---

## 📈 Conclusión

**"Los Clavitos de Pablito"** representa una solución completa de transformación digital para una empresa tradicional como **FERREMAS**. El proyecto no solo mejora la experiencia del cliente, sino que también optimiza los procesos internos, incrementa la eficiencia operativa y abre nuevas oportunidades de expansión comercial. La integración de tecnologías modernas y APIs externas proporciona una base sólida para el crecimiento futuro del negocio.

---

**Desarrollado como parte de la evaluación académica del módulo ASY5131 - Integración de Plataformas.**