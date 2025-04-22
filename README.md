# 🧠 Clasificador de Clústeres en Sepsis (GMM)

Este repositorio contiene una aplicación web interactiva que permite ingresar variables clínicas de un paciente con sepsis y estimar a qué **clúster fisiopatológico** pertenece, basado en un modelo de **Mezclas Gaussianas (GMM)**. Además, reporta la **probabilidad estimada de mortalidad intrahospitalaria** y de **estancia hospitalaria prolongada (>5 días)** asociadas al clúster.

---

## 🌐 Aplicación en vivo

Puedes desplegar la aplicación con GitHub Pages o abrir el archivo [`index.html`](./index.html) directamente en tu navegador.

![App Demo](https://raw.githubusercontent.com/tu-usuario/sepsis-cluster-app/main/demo.gif)

---

## 📊 Metodología

Se aplicó un modelo de **Gaussian Mixture Models (GMM)** a una cohorte de **96 pacientes adultos con sepsis**, utilizando las siguientes variables clínicas:

- Edad
- APACHE II
- SOFA
- Creatinina
- Lactato (hora 0)
- pH (hora 0)
- Índice de choque sistólico (IS-0)
- Delta IS (IS-6 – IS-0)

### 🔬 Variables seleccionadas
Estas variables fueron estandarizadas y procesadas para entrenamiento no supervisado. Se determinaron **5 clústeres** con perfiles clínicos diferenciados.

---

## 📈 Resultados

- **Figura 1:** Clustering visualizado por PCA  
  ![Figura 1](./output%20(2).png)

- **Figura 2:** Mapa de calor con desenlaces por clúster  
  ![Figura 2](./output%20(3).png)

- **Figura 3:** Boxplots comparativos entre clústeres  
  ![Figura 3](./output%20(4).png)

- **Figura 4:** Radar plots de perfiles fisiopatológicos  
  ![Figura 4](./output%20(5).png)

### 📌 Hallazgos clave

- Mortalidad intrahospitalaria por clúster: 25% a 75%
- Estancia prolongada (>5 días): 57% a 75%
- Los clústeres con mayor severidad mostraron elevación de lactato, acidemia y disfunción orgánica múltiple.

---

## 🛠️ Cómo usar

1. Clona este repositorio o descarga el archivo `index.html`.
2. Ábrelo con cualquier navegador moderno.
3. Ingresa los valores clínicos del paciente.
4. Visualiza el clúster estimado, junto con la probabilidad de mortalidad y estancia prolongada.

---

## 📄 Cita sugerida

> Este trabajo es parte de un proyecto de investigación sobre inteligencia artificial aplicada a medicina crítica.  
> Programa GLORIA – Fundación Universitaria de Ciencias de la Salud (FUCS), Bogotá, Colombia.

---

## 🧑‍💻 Autor

**John Sprockel**  
Profesor - Investigador en inteligencia artificial aplicada a salud  
[@jjsprockel](mailto:jjsprockel@fucsalud.edu.co)

