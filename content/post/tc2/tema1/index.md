---
title: tema1
date: 2024-02-26
tags: [tc2]
---

# Tema 1: Algunas distribuciones de probabilidad continuas.

## 1.1 Distribución uniforme:

### Descripción:
Se trata de una distribución de probabilidad continua en el intervalo \\([a, b]\\).

### Función de densidad de probabilidad:
La función de densidad de probabilidad es:

$$
f(x) = \begin{cases} 
\frac{1}{b-a} & \text{si } a \leq x \leq b \\
0 & \text{si } x < a \text{ o } x > b 
\end{cases}
$$

### Función de distribución:
La función de distribución es:

$$
F(x) = \begin{cases} 
0 & \text{si } x < a \\
\frac{x-a}{b-a} & \text{si } a \leq x \leq b \\
1 & \text{si } x > b 
\end{cases}
$$

### Medidas de tendencia central y dispersión:
- Esperanza matemática: \\(E(X) = \frac{a+b}{2}\\)
- Varianza: \\(Var(X) = \frac{(b-a)^2}{12}\\)

### Coeficientes de asimetría:
- Coeficiente de asimetría de tercer orden: \\(g_1 = 0\\)
- Coeficiente de asimetría de cuarto orden: \\(g_2 = -\frac{6}{5}\\)

## 1.2 Distribución Gamma:

### Descripción:
La distribución Gamma es utilizada para modelar tiempos de espera hasta que ocurra un número determinado de eventos.

### Función de densidad de probabilidad:
La función de densidad de probabilidad es:

$$
f(x; k, \theta) = \frac{1}{\Gamma(k)\theta^k} x^{k-1} e^{-\frac{x}{\theta}}
$$

donde \\(k\\) es el parámetro de forma y \\(\theta\\) es el parámetro de escala.

### Función de distribución:
La función de distribución es expresada con la función gamma incompleta:

$$
F(x; k, \theta) = \begin{cases}
0 & \text{si } x < 0 \\
\frac{1}{\Gamma(k)} \gamma(k, \frac{x}{\theta}) & \text{si } x \geq 0
\end{cases}
$$

### Medidas de tendencia central y dispersión:
- Esperanza matemática: \\(E(X) = k\theta\\)
- Varianza: \\(Var(X) = k\theta^2\\)

## 1.3 Distribución Exponencial:

### Descripción:
La distribución exponencial modela el tiempo entre eventos en un proceso de Poisson.

### Función de densidad de probabilidad:
La función de densidad de probabilidad es:

$$
f(x; \lambda) = \lambda e^{-\lambda x}
$$

donde \\(\lambda\\) es la tasa de ocurrencia.

### Función de distribución:
La función de distribución es:

$$
F(x; \lambda) = \begin{cases}
0 & \text{si } x < 0 \\
1 - e^{-\lambda x} & \text{si } x \geq 0
\end{cases}
$$

### Medidas de tendencia central y dispersión:
- Esperanza matemática: \\(E(X) = \frac{1}{\lambda}\\)
- Varianza: \\(Var(X) = \frac{1}{\lambda^2}\\)

## 1.4 Distribución Beta:

### Descripción:
La distribución Beta es utilizada para modelar variables aleatorias que tienen un rango limitado entre 0 y 1.

### Función de densidad de probabilidad:
La función de densidad de probabilidad es:

$$
f(x; \alpha, \beta) = \frac{x^{\alpha-1}(1-x)^{\beta-1}}{B(\alpha, \beta)}
$$

donde \\(B(\alpha, \beta)\\) es la función Beta.

### Función de distribución:
La función de distribución es:

$$
F(x; \alpha, \beta) = \begin{cases}
0 & \text{si } x < 0 \\
I_x(\alpha, \beta) & \text{si } 0 \leq x \leq 1 \\
1 & \text{si } x > 1
\end{cases}
$$

### Medidas de tendencia central y dispersión:
- Esperanza matemática: \\(E(X) = \frac{\alpha}{\alpha+\beta}\\)
- Varianza: \\(Var(X) = \frac{\alpha\beta}{(\alpha+\beta)^2(\alpha+\beta+1)}\\)

## 1.5 Distribución Normal:

### Descripción:
La distribución normal es una de las distribuciones más comunes en estadísticas y modela muchos fenómenos naturales.

### Función de densidad de probabilidad:
La función de densidad de probabilidad es:

$$
f(x; \mu, \sigma) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

donde \\(\mu\\) es la media y \\(\sigma\\) es la desviación estándar.

### Función de distribución:
La función de distribución es:

$$
F(x; \mu, \sigma) = \frac{1}{2} \left[1 + \text{erf}\left(\frac{x-\mu}{\sigma \sqrt{2}}\right)\right]
$$

### Medidas de tendencia central y dispersión:
- Esperanza matemática: \\(E(X) = \mu\\)
- Varianza: \\(Var(X) = \sigma^2\\)
