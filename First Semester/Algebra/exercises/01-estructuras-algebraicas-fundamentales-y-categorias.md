# Problemas — Estructuras algebraicas fundamentales y categorías

**Referencia principal:** `First Semester/Algebra/ref/doc.pdf`  
**Capítulo:** 1  
**Secciones:** 1.1 y 1.2

> Este archivo reúne problemas de práctica alineados con las definiciones y ejemplos del capítulo: leyes de composición, magma, semigrupo, monoide, grupo y nociones básicas de categoría.

---

## Parte A — Leyes de composición y estructuras algebraicas

1. Sea \(A = \mathbb{Z}\). Defina la operación
   \[
   a * b = a + b + 1.
   \]
   Determine si \((A, *)\) es magma, semigrupo, monoide o grupo. Si existe elemento identidad, encuéntrelo. Si es grupo, halle el inverso de un elemento arbitrario.

2. Considere los siguientes ejemplos y clasifique cada uno como magma, semigrupo, monoide o grupo. Indique además si la operación es conmutativa:
   - \((\mathbb{N}, +)\)
   - \((\mathbb{Z}, +)\)
   - \((\mathbb{N}, \cdot)\)
   - \((\mathcal{P}(X), \cup)\)
   - \((\mathcal{P}(X), \cap)\)
   - \((\mathrm{End}(X), \circ)\), donde \(\mathrm{End}(X)\) es el conjunto de funciones \(X \to X\)

3. Dé un ejemplo de:
   - una ley de composición entre dos conjuntos distintos que NO sea operación interna;
   - una operación interna que no sea asociativa;
   - un semigrupo que no sea monoide;
   - un monoide que no sea grupo.

4. En el conjunto \(A = \{0,1,2\}\), defina la operación
   \[
   a \star b = \max\{a,b\}.
   \]
   Verifique si \((A,\star)\) es un monoide. Determine su elemento identidad y diga si es grupo.

5. En el conjunto \(A = \{0,1,2\}\), defina la operación
   \[
   a \diamond b = \min\{a+b,2\}.
   \]
   Estudie si la operación es asociativa. Si lo es, determine si \((A,\diamond)\) es monoide o grupo.

6. Pruebe que en un monoide el elemento identidad es único.

7. Pruebe que en un grupo el inverso de cada elemento es único.

8. Sea \(G\) un grupo. Demuestre que para todo \(a \in G\),
   \[
   (a^{-1})^{-1} = a
   \qquad\text{y}\qquad
   (ab)^{-1} = b^{-1}a^{-1}.
   \]

9. Demuestre que \((\mathbb{Z}_n, +)\) es un grupo abeliano para todo \(n \ge 1\).

10. Usando la convención del texto, considere
    \[
    (\mathbb{Z}_n)^* = \{[a]\in \mathbb{Z}_n : [a]\neq [0]\}
    \]
    con la multiplicación módulo \(n\).
    - Estudie los casos \(n=4\), \(n=6\) y \(n=7\).
    - Determine en cuáles casos se obtiene un grupo.
    - Explique qué relación observa con la primalidad de \(n\).

11. Dé un ejemplo de operación externa \(A \times B \to B\) y explique por qué NO puede considerarse una operación interna en \(B\).

12. Sea \(M\) un semigrupo que tiene identidad por la izquierda \(e\) y tal que cada elemento \(a\in M\) tiene inverso por la izquierda \(b\in M\), es decir, \(ba=e\). Demuestre que \(M\) es un grupo.

---

## Parte B — Introducción a categorías

13. Escriba con precisión la definición de categoría identificando:
    - objetos,
    - morfismos,
    - composición,
    - identidades,
    - asociatividad.

14. En la categoría **Set**, considere
    \[
    A=\{1,2\},\quad B=\{a,b,c\},\quad C=\{\alpha,\beta\}.
    \]
    Defina funciones \(f:A\to B\) y \(g:B\to C\), calcule \(g\circ f\) y verifique explícitamente la propiedad de identidad usando \(id_A\) e \(id_B\).

15. Demuestre que el morfismo identidad de un objeto en una categoría es único.

16. Sea \(f:A\to B\) un morfismo en una categoría. Suponga que existe \(g:B\to A\) con
    \[
    g\circ f = id_A
    \]
    y \(h:B\to A\) con
    \[
    f\circ h = id_B.
    \]
    Demuestre que \(g=h\).

17. En la categoría **Set**, pruebe que un morfismo es un isomorfismo si y solo si es biyectivo.

18. En la categoría **Mag**, tome
    \[
    (\mathbb{Z},+) \quad\text{y}\quad (\mathbb{Z},+).
    \]
    Estudie si las aplicaciones siguientes son homomorfismos de magmas:
    - \(f(x)=2x\)
    - \(g(x)=x+1\)
    - \(h(x)=-x\)

19. En la categoría **Vect\(_K\)**, explique por qué la composición de aplicaciones lineales vuelve a ser lineal. Luego verifique esa propiedad para dos transformaciones lineales concretas entre espacios \(K^2\) y \(K^3\).

20. Dé un ejemplo de un morfismo en **Top** que sea continuo pero no sea isomorfismo. Explique con cuidado por qué falla la condición de isomorfismo.

---

## Parte C — Conexión entre monoides y categorías

21. Sea \((M,*)\) un monoide. Construya una categoría \(\mathcal{C}_M\) con un solo objeto \(\bullet\) tal que
    \[
    \mathrm{Hom}_{\mathcal{C}_M}(\bullet,\bullet)=M.
    \]
    Defina la composición usando la operación de \(M\) y verifique los axiomas de categoría.

22. Recíprocamente, sea \(\mathcal{C}\) una categoría con un único objeto \(A\). Demuestre que
    \[
    \mathrm{Hom}_{\mathcal{C}}(A,A)
    \]
    tiene estructura de monoide con la composición.

23. Explique por qué un grupo puede verse como una categoría con un solo objeto en la que todos los morfismos son isomorfismos.

24. Compare las siguientes tres ideas y explique sus diferencias CON CLARIDAD:
    - igualdad de objetos,
    - isomorfismo de objetos,
    - igualdad de morfismos.

---

## Reto final

25. Redacte un cuadro comparativo donde aparezcan las estructuras
    \[
    \text{magma} \to \text{semigrupo} \to \text{monoide} \to \text{grupo}
    \]
    indicando en cada paso qué propiedad adicional se exige. Luego explique cómo la noción de categoría abstrae la composición y la identidad que ya aparecen en estas estructuras.
