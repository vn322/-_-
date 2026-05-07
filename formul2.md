### 1. Математический анализ

$\lim_{x \to x_0} f(x) = A \iff \forall \varepsilon > 0 \ \exists \delta > 0 : 0 < |x - x_0| < \delta \Rightarrow |f(x) - A| < \varepsilon$.
$x, x_0, A \in \mathbb{R}, \varepsilon, \delta \in \mathbb{R}_+$. Предел функции в точке.

$f \in C[x_0] \iff \lim_{x \to x_0} f(x) = f(x_0)$. Непрерывность в точке. $C$ — класс непрерывных функций.

Свойства непрерывной на $[a,b]$: 1) Ограниченность: $\exists M>0 : \sup_{x\in[a,b]}|f(x)| \le M$. 2) Достижение граней: $\exists \xi_1, \xi_2 \in [a,b] : f(\xi_1)=\min f, f(\xi_2)=\max f$. 3) Теорема о промежуточном значении: $\forall \gamma \in [m, M] \ \exists c \in [a,b] : f(c)=\gamma$. $m=\min f, M=\max f$.

$f'(x_0) = \lim_{\Delta x \to 0} \frac{f(x_0+\Delta x)-f(x_0)}{\Delta x}$. Производная. $\Delta x$ — приращение аргумента, $f'$ — скорость изменения.

$f(x_1,\dots,x_n)$. Полный дифференциал: $df = \sum_{i=1}^n \frac{\partial f}{\partial x_i} dx_i$. Геометрический смысл: линейная часть приращения функции, уравнение касательной плоскости $z = f(\vec{x}_0) + (\nabla f, \vec{x}-\vec{x}_0)$.

Достаточное условие дифференцируемости: $\exists$ частные производные $\frac{\partial f}{\partial x_i}$ в окрестности и они непрерывны в точке $\vec{x}_0$.

$\nabla f = \left( \frac{\partial f}{\partial x_1}, \dots, \frac{\partial f}{\partial x_n} \right)$. Градиент. Вектор направления наибыстрейшего роста, $df = (\nabla f, d\vec{x})$.

$F'(x) = f(x) \Rightarrow F(x) = \int f(x) dx + C$. Первообразная и неопределенный интеграл. $C \in \mathbb{R}$ — произвольная постоянная.

Интегральная сумма Римана: $\sigma(f, \Pi, \xi) = \sum_{i=1}^n f(\xi_i) \Delta x_i, \ \Delta x_i = x_i - x_{i-1}$. $\int_a^b f(x) dx = \lim_{\lambda(\Pi)\to 0} \sigma$. $\lambda$ — диаметр разбиения, $\xi_i \in [x_{i-1}, x_i]$.

$\int_a^b f(x) dx = F(b) - F(a), \ F'(x)=f(x)$. Формула Ньютона-Лейбница. $F$ — первообразная на $[a,b]$.

Ряд $\sum_{n=1}^\infty a_n$. Критерий Коши: $\forall \varepsilon>0 \ \exists N \ \forall n>N, p\in\mathbb{N} : |S_{n+p}-S_n| < \varepsilon$. $S_n = \sum_{k=1}^n a_k$.

Признаки сходимости: 1) Сравнения: $0 \le a_n \le b_n, \sum b_n < \infty \Rightarrow \sum a_n < \infty$. 2) Даламбера: $\lim |a_{n+1}/a_n| = q < 1 \Rightarrow$ сход. 3) Коши (радикальный): $\lim \sqrt[n]{|a_n|} = q < 1 \Rightarrow$ сход. 4) Интегральный: $\sum a_n \sim \int_1^\infty f(x) dx$ при $a_n=f(n), f\downarrow$.

$\sum a_n$ абсолютно сходится $\iff \sum |a_n| < \infty$. Условно сходится $\iff \sum a_n$ сход., $\sum |a_n|$ расх. Свойство: абсолютно сходящийся ряд сходится при любой перестановке. Произведение Коши: $\sum c_n, \ c_n = \sum_{k=0}^n a_k b_{n-k}$. Если $\sum a_n, \sum b_n$ абс. сходятся, то $\sum c_n = (\sum a_n)(\sum b_n)$.

Функциональный ряд $\sum u_n(x)$. Равномерная сходимость на $E$: $\forall \varepsilon>0 \ \exists N \ \forall n>N, x\in E : |S_n(x)-S(x)| < \varepsilon$. $S_n$ — частичная сумма, $S$ — сумма.

Признак Вейерштрасса: $\forall x\in E, |u_n(x)| \le M_n, \ \sum M_n < \infty \Rightarrow$ равномерная сходимость. $M_n$ — числовая мажоранта.

Свойства равномерной сходимости: 1) Если $u_n \in C(E)$ и ряд сходится равномерно, то $S(x) \in C(E)$. 2) Почленное интегрирование: $\int_a^b S(x)dx = \sum \int_a^b u_n(x)dx$. 3) Почленное дифференцирование: если $u_n \in C^1$ и $\sum u_n'(x) \rightrightarrows$, то $S'(x) = \sum u_n'(x)$.

Степенной ряд $\sum a_n (x-x_0)^n$. Радиус сходимости: $R = \left( \limsup_{n\to\infty} \sqrt[n]{|a_n|} \right)^{-1}$ или $R = \lim |a_n/a_{n+1}|$ (при существовании). Сходится абсолютно и равномерно на $[x_0-r, x_0+r] \ \forall r < R$.

Ряд Тейлора: $f(x) = \sum_{n=0}^\infty \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n$. Разложение возможно, если $f \in C^\infty$ и остаток $r_n(x) = f(x) - S_n(x) \to 0$ при $n\to\infty$.

Несобственный интеграл 1-го рода: $\int_a^\infty f(x)dx = \lim_{b\to\infty} \int_a^b f(x)dx$. 2-го рода: $\int_a^b f(x)dx = \lim_{\varepsilon\to 0^+} \int_a^{b-\varepsilon} f(x)dx$ ($b$ — особая точка). Сходится, если предел конечен.

Теорема Ферма: $f$ дифф. в $x_0$, $x_0$ — точка локального экстремума внутренней области $\Rightarrow f'(x_0)=0$.

Теорема Ролля: $f \in C[a,b] \cap D(a,b), f(a)=f(b) \Rightarrow \exists \xi \in (a,b) : f'(\xi)=0$.

Теорема Лагранжа: $f \in C[a,b] \cap D(a,b) \Rightarrow \exists \xi \in (a,b) : f(b)-f(a) = f'(\xi)(b-a)$.

Теорема Коши: $f,g \in C[a,b] \cap D(a,b), g'(x)\neq 0 \Rightarrow \exists \xi \in (a,b) : \frac{f(b)-f(a)}{g(b)-g(a)} = \frac{f'(\xi)}{g'(\xi)}$.



### 2. Алгебра и Аналитическая геометрия

Прямая в $\mathbb{R}^3$: каноническая $\frac{x-x_0}{l} = \frac{y-y_0}{m} = \frac{z-z_0}{n}$. Параметрическая: $\vec{r}(t) = \vec{r}_0 + t\vec{s}$. Общее (пересечение плоскостей): система двух линейных уравнений. $\vec{s}=(l,m,n)$ — направляющий вектор.

Плоскость: общее $Ax+By+Cz+D=0$. Через точку: $A(x-x_0)+B(y-y_0)+C(z-z_0)=0$. $\vec{n}=(A,B,C)$ — нормальный вектор.

Взаимное расположение: прямая и плоскость: угол $\sin \phi = \frac{|\vec{s}\cdot\vec{n}|}{\|\vec{s}\|\|\vec{n}\|}$. Параллельность: $\vec{s}\cdot\vec{n}=0$. Две прямые: скрещиваются, если $\det(\vec{s}_1, \vec{s}_2, \overrightarrow{M_1M_2}) \neq 0$.

Метрические приложения: расстояние от $M_0$ до прямой с $\vec{s}$: $\rho = \frac{\|\overrightarrow{M_1M_0} \times \vec{s}\|}{\|\vec{s}\|}$. До плоскости: $\rho = \frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}$. Угол между плоскостями: $\cos \phi = \frac{|\vec{n}_1\cdot\vec{n}_2|}{\|\vec{n}_1\|\|\vec{n}_2\|}$.

Кривые 2-го порядка: $Ax^2+2Bxy+Cy^2+2Dx+2Ey+F=0$. Инварианты: $I_1=A+C, I_2=\det\begin{pmatrix} A & B \\ B & C \end{pmatrix}, I_3=\det\begin{pmatrix} A & B & D \\ B & C & E \\ D & E & F \end{pmatrix}$. Приведение: поворот $\cot 2\alpha = \frac{A-C}{2B}$, перенос в центр. Канонические: эллипс $\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$, гипербола $\frac{x^2}{a^2}-\frac{y^2}{b^2}=1$, парабола $y^2=2px$.

СЛАУ $A\vec{x}=\vec{b}$. Методы: Гаусса (прямой/обратный ход), Крамера ($x_i = \det A_i / \det A$), матричный ($\vec{x}=A^{-1}\vec{b}$). Теорема Кронекера-Капелли: совместна $\iff \text{rank}(A) = \text{rank}(\bar{A})$. $\bar{A}$ — расширенная матрица.

Структура решения: $\vec{x} = \vec{x}_0 + \sum_{i=1}^{k} c_i \vec{v}_i$, $k=n-\text{rank}(A)$. $\vec{x}_0$ — частное решение неоднородной, $\{\vec{v}_i\}$ — ФСР однородной $A\vec{x}=\vec{0}$. ФСР — максимальная линейно независимая система решений.

Собственные значения и векторы: $A\vec{v} = \lambda \vec{v}, \ \vec{v} \neq \vec{0}$. Характеристический многочлен: $\chi_A(\lambda) = \det(A - \lambda I)$. Корни $\lambda_i$ — собственные значения. Геометрическая кратность: $\dim \ker(A-\lambda I)$. Алгебраическая: кратность корня $\chi_A$.

Линейный оператор $\mathcal{A}: V \to W$: $\mathcal{A}(\alpha \vec{x} + \beta \vec{y}) = \alpha \mathcal{A}(\vec{x}) + \beta \mathcal{A}(\vec{y})$. Примеры: дифференцирование, интегрирование, матричное умножение. Задание: матрицей $[\mathcal{A}]$ в базисе $\{\vec{e}_i\}$: $\mathcal{A}(\vec{e}_j) = \sum_i a_{ij} \vec{e}_i$. Свойства: $\ker \mathcal{A}, \text{Im } \mathcal{A}$ — подпространства, $\dim \ker \mathcal{A} + \dim \text{Im } \mathcal{A} = \dim V$. Действия: $(\mathcal{A}+\mathcal{B})\vec{x} = \mathcal{A}\vec{x}+\mathcal{B}\vec{x}$, $(\mathcal{A}\circ\mathcal{B})\vec{x} = \mathcal{A}(\mathcal{B}\vec{x})$. Матрица композиции: $[\mathcal{A}\circ\mathcal{B}] = [\mathcal{A}][\mathcal{B}]$.



### 3. Дифференциальные уравнения

ДУ 1-го порядка: $y' = f(x,y)$. Теорема Коши: если $f, \frac{\partial f}{\partial y}$ непрерывны в области $D \ni (x_0,y_0)$, то $\exists!$ решение $y=\varphi(x)$ на $|x-x_0|<h$, удовлетворяющее $y(x_0)=y_0$.

Линейное ДУ 2-го порядка: $y'' + p(x)y' + q(x)y = f(x)$. Однородное: $f(x)\equiv 0$. Линейная зависимость $\{y_1,\dots,y_n\}$: $\exists c_i$, не все 0: $\sum c_i y_i(x) \equiv 0$.

Определитель Вронского: $W(y_1,\dots,y_n)(x) = \det \begin{pmatrix} y_1 & \dots & y_n \\ y_1' & \dots & y_n' \\ \vdots & \ddots & \vdots \\ y_1^{(n-1)} & \dots & y_n^{(n-1)} \end{pmatrix}$. Решения однородного линейно независимы $\iff W(x) \neq 0$ в любой точке.

ФСР — набор из $n$ линейно независимых решений однородного уравнения. Общее решение: $y = \sum_{i=1}^n c_i y_i(x)$.

Линейное неоднородное: $y = y_0 + \sum c_i y_i$, $y_0$ — частное решение. Метод вариации постоянных: $y_0 = \sum c_i(x) y_i(x)$, система $\sum c_i'(x) y_i^{(k)}(x) = 0 \ (k=0,\dots,n-2), \ \sum c_i'(x) y_i^{(n-1)}(x) = f(x)$.

Устойчивость по Ляпунову: решение $\vec{x}(t)$ устойчиво, если $\forall \varepsilon>0 \ \exists \delta>0 : \|\vec{x}(0)-\vec{x}_0\|<\delta \Rightarrow \|\vec{x}(t)-\vec{x}_0\|<\varepsilon \ \forall t\ge 0$. Асимптотически устойчиво, если дополнительно $\lim_{t\to\infty} \vec{x}(t) = \vec{x}_0$.

Теорема Ляпунова: $\exists V(\vec{x}) \in C^1$, положительно определенная ($V(0)=0, V(\vec{x})>0$), $\dot{V}(\vec{x}) = \nabla V \cdot \vec{f}(\vec{x}) \le 0 \Rightarrow$ устойчивость. Если $\dot{V}(\vec{x}) < 0$ при $\vec{x}\neq 0 \Rightarrow$ асимптотическая устойчивость.

Теорема Четаева: $\exists V(\vec{x}) \in C^1$, область $\Omega: V(\vec{x})>0, 0\in\partial\Omega$, на границе $\Omega$ $V=0$, в $\Omega$ $\dot{V}(\vec{x})>0 \Rightarrow$ неустойчивость.

Линейное УрЧП 1-го порядка: $a(x,y)\frac{\partial u}{\partial x} + b(x,y)\frac{\partial u}{\partial y} = c(x,y)u + d(x,y)$. Система характеристик: $\frac{dx}{a} = \frac{dy}{b} = \frac{du}{cu+d}$. Первые интегралы $\Phi_1(x,y,u)=C_1, \Phi_2(x,y,u)=C_2$. Общее решение: $F(\Phi_1, \Phi_2)=0$ или $u = \Psi(\Phi_1)$.



### 4. Комплексный анализ

Функция комплексного переменного: $f(z) = u(x,y) + i v(x,y), \ z=x+iy$. Дифференцируемость в $z_0$: $\exists \lim_{\Delta z \to 0} \frac{f(z_0+\Delta z)-f(z_0)}{\Delta z} = f'(z_0)$.

Условия Коши-Римана: $\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \ \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$. Необходимы и достаточны при непрерывности частных производных.

Геометрический смысл производной: $f'(z_0) = |f'(z_0)| e^{i \arg f'(z_0)}$. $|f'(z_0)|$ — коэффициент локального растяжения бесконечно малых отрезков. $\arg f'(z_0)$ — угол поворота касательной к любой кривой через $z_0$. Конформность при $f'(z_0) \neq 0$.

Теорема Коши об интеграле: если $f(z)$ голоморфна в области $D$ и непрерывна на $\bar{D}$, $\gamma \subset D$ — кусочно-гладкий замкнутый контур, то $\oint_\gamma f(z) dz = 0$.

Интегральная формула Коши: $f^{(n)}(z_0) = \frac{n!}{2\pi i} \oint_\gamma \frac{f(z)}{(z-z_0)^{n+1}} dz, \ z_0 \in \text{int}(\gamma)$. Следствие: голоморфная функция бесконечно дифференцируема.

Степенной ряд с комплексными членами: $\sum_{n=0}^\infty a_n (z-z_0)^n$. Радиус сходимости $R$ вычисляется формулами Коши-Адамара или Даламбера. Сходится абсолютно и равномерно в $|z-z_0| \le r < R$.

Ряд Лорана: $f(z) = \sum_{n=-\infty}^\infty c_n (z-z_0)^n = \sum_{n=0}^\infty a_n (z-z_0)^n + \sum_{n=1}^\infty \frac{b_n}{(z-z_0)^n}$. Сходится в кольце $r < |z-z_0| < R$. Коэффициенты: $c_n = \frac{1}{2\pi i} \oint_\gamma \frac{f(\zeta)}{(\zeta-z_0)^{n+1}} d\zeta$.

Особые точки: изолированная $z_0$. 1) Устранимая: $\lim_{z\to z_0} f(z)$ конечен, $b_n=0 \ \forall n\ge 1$. 2) Полюс порядка $m$: $b_m \neq 0, b_k=0 \ \forall k>m$, $\lim_{z\to z_0} |f(z)| = \infty$. 3) Существенно особая: бесконечно много $b_n \neq 0$, предел не существует.

Вычет: $\text{Res}(f, z_0) = c_{-1} = \frac{1}{2\pi i} \oint_\gamma f(z) dz$. Для полюса порядка $m$: $\text{Res}(f, z_0) = \frac{1}{(m-1)!} \lim_{z\to z_0} \frac{d^{m-1}}{dz^{m-1}} [(z-z_0)^m f(z)]$. Основная теорема: $\oint_\gamma f(z) dz = 2\pi i \sum \text{Res}(f, z_k)$.



### 5. Уравнения математической физики

Пространство Соболева $W^{k,p}(\Omega) = \{ u \in L^p(\Omega) : D^\alpha u \in L^p(\Omega), \ |\alpha| \le k \}$. Норма: $\|u\|_{W^{k,p}} = \left( \sum_{|\alpha|\le k} \|D^\alpha u\|_{L^p}^p \right)^{1/p}$. $D^\alpha$ — слабая производная. $H^k = W^{k,2}$.

Теорема вложения: 1) Если $kp > n$, то $W^{k,p}(\Omega) \hookrightarrow C^m(\bar{\Omega})$ для $m < k - n/p$. 2) Если $kp < n$, то $W^{k,p}(\Omega) \hookrightarrow L^q(\Omega)$ для $1 \le q \le np/(n-kp)$ (компактное вложение при ограниченной области).

Эллиптическая задача: $-\nabla \cdot (A \nabla u) + c u = f$ в $\Omega$, $u|_{\partial\Omega} = g$. Обобщенное решение: $u \in H^1_0(\Omega): \int_\Omega (A\nabla u \cdot \nabla v + c u v) dx = \int_\Omega f v dx \ \forall v \in H^1_0(\Omega)$. Теорема Лакса-Мильграма гарантирует единственную разрешимость. Гладкость: если $f \in H^s$, то $u \in H^{s+2}$. Задача на собственные значения: $-\Delta u = \lambda u$, $u|_{\partial\Omega}=0$. $\exists$ дискретный спектр $0 < \lambda_1 \le \lambda_2 \le \dots \to \infty$, $\{u_k\}$ ортонормированы в $L^2$.

Метод Фурье для смешанной задачи: $u(x,t) = \sum_{k=1}^\infty T_k(t) X_k(x)$. $X_k$ — собственные функции оператора Лапласа с граничными условиями. $T_k(t)$ находятся из ОДУ для временной части с начальными условиями, разложенными по $\{X_k\}$.

Метод Галеркина: $u_N(x,t) = \sum_{k=1}^N c_k(t) \phi_k(x)$, $\{\phi_k\}$ — базис $H^1_0$. Подстановка в уравнение, умножение на $\phi_j$, интегрирование дает систему ОДУ для $c_k(t)$. При $N \to \infty$ $u_N \to u$ в $L^2(0,T; H^1_0)$.

Сильно непрерывная полугруппа $\{T(t)\}_{t\ge 0}$: $T(0)=I, \ T(t+s)=T(t)T(s), \ \lim_{t\to 0^+} T(t)x = x$. Генератор $A$: $Ax = \lim_{t\to 0^+} \frac{T(t)x-x}{t}$. Задача Коши $u' = Au, u(0)=u_0$ имеет решение $u(t)=T(t)u_0$. Для параболических уравнений $T(t)$ — аналитическая полугруппа, обеспечивает гладкость и затухание.



### 6. Дискретная математика

Сочетания: $C_n^k = \binom{n}{k} = \frac{n!}{k!(n-k)!}$. Размещения: $A_n^k = \frac{n!}{(n-k)!}$. Перестановки: $P_n = n!$. С повторениями: $\bar{C}_n^k = \binom{n+k-1}{k}$, $\bar{A}_n^k = n^k$, $\bar{P}_n = \frac{n!}{n_1! \dots n_k!}$.

Формула включений-исключений: $|\bigcup_{i=1}^m A_i| = \sum |A_i| - \sum_{i<j} |A_i \cap A_j| + \dots + (-1)^{m-1} |\bigcap_{i=1}^m A_i|$.

Бином Ньютона: $(x+y)^n = \sum_{k=0}^n \binom{n}{k} x^{n-k} y^k$. Свойства: $\binom{n}{k} = \binom{n}{n-k}$, $\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$, $\sum_{k=0}^n \binom{n}{k} = 2^n$, $\sum_{k=0}^n (-1)^k \binom{n}{k} = 0$.

Булева функция $f: \{0,1\}^n \to \{0,1\}$. Принцип двойственности: $f^*(x_1,\dots,x_n) = \overline{f(\overline{x_1},\dots,\overline{x_n})}$. СДНФ: $f = \bigvee_{f(\alpha)=1} (x_1^{\alpha_1} \dots x_n^{\alpha_n})$, $x_i^1=x_i, x_i^0=\overline{x_i}$. СКНФ: $f = \bigwedge_{f(\alpha)=0} (x_1^{\overline{\alpha_1}} \vee \dots \vee x_n^{\overline{\alpha_n}})$.

Минимизация: 1) Простые импликанты (объединение термов, отличающихся одной переменной). 2) Таблица импликант: строки — импликанты, столбцы — наборы $f=1$. Отметка обязательных. 3) Алгоритм Куайна-Мак-Класки: группировка по числу единиц, попарное склеивание, исключение поглощенных термов, выбор минимального покрытия.

Производящая функция $\{a_n\}$: $A(x) = \sum_{n=0}^\infty a_n x^n$. Свойства: $A(x)B(x) = \sum c_n x^n, c_n = \sum_{k=0}^n a_k b_{n-k}$. $A'(x) = \sum n a_n x^{n-1}$. $A(x)/(1-x) = \sum (\sum_{k=0}^n a_k) x^n$.

Линейное рекуррентное соотношение: $a_n + c_1 a_{n-1} + \dots + c_k a_{n-k} = 0$. Характеристический многочлен: $\lambda^k + c_1 \lambda^{k-1} + \dots + c_k = 0$. Корни $\lambda_j$ с кратностями $r_j$. Общее решение: $a_n = \sum_{j} P_j(n) \lambda_j^n$, $\deg P_j < r_j$. Коэффициенты из $a_0,\dots,a_{k-1}$.



### 7. Теория вероятностей и математическая статистика

Вероятностное пространство $(\Omega, \mathcal{F}, \mathbb{P})$. $\mathcal{F}$ — $\sigma$-алгебра событий. Аксиомы: 1) $\mathbb{P}(A) \ge 0$. 2) $\mathbb{P}(\Omega)=1$. 3) $\mathbb{P}(\bigcup A_i) = \sum \mathbb{P}(A_i)$ для попарно несовместных. Классическая: $\mathbb{P}(A) = \frac{|A|}{|\Omega|}$. Геометрическая: $\mathbb{P}(A) = \frac{\mu(A)}{\mu(\Omega)}$.

Условная вероятность: $\mathbb{P}(A|B) = \frac{\mathbb{P}(AB)}{\mathbb{P}(B)}$. Формула умножения: $\mathbb{P}(A_1 \dots A_n) = \mathbb{P}(A_1) \mathbb{P}(A_2|A_1) \dots \mathbb{P}(A_n|A_1 \dots A_{n-1})$. Независимость: $\mathbb{P}(AB)=\mathbb{P}(A)\mathbb{P}(B)$. Полная вероятность: $\mathbb{P}(A) = \sum \mathbb{P}(A|H_i)\mathbb{P}(H_i)$. Байес: $\mathbb{P}(H_k|A) = \frac{\mathbb{P}(A|H_k)\mathbb{P}(H_k)}{\sum \mathbb{P}(A|H_i)\mathbb{P}(H_i)}$.

Схема Бернулли: $P_n(k) = \binom{n}{k} p^k (1-p)^{n-k}$. Локальная Муавра-Лапласа: $P_n(k) \approx \frac{1}{\sqrt{npq}} \varphi\left(\frac{k-np}{\sqrt{npq}}\right), \ \varphi(x)=\frac{1}{\sqrt{2\pi}}e^{-x^2/2}$. Интегральная: $\mathbb{P}(k_1 \le \mu \le k_2) \approx \Phi\left(\frac{k_2-np}{\sqrt{npq}}\right) - \Phi\left(\frac{k_1-np}{\sqrt{npq}}\right)$. Теорема Пуассона: $P_n(k) \to \frac{\lambda^k e^{-\lambda}}{k!}$ при $n\to\infty, p\to 0, np=\lambda$.

Случайная величина (СВ): $F_X(x) = \mathbb{P}(X < x)$. Свойства: неубывающая, непрерывная справа, пределы $0$ и $1$. Дискретная: $p_i = \mathbb{P}(X=x_i)$. Распределения: Биномиальное $B(n,p)$, Пуассона $\Pi(\lambda)$, Геометрическое $P(X=k)=p(1-p)^{k-1}$. Непрерывная: $f(x)\ge 0, \int f dx=1, F(x)=\int_{-\infty}^x f(t)dt$. Распределения: Равномерное $U[a,b]$, Экспоненциальное $E(\lambda)$, Нормальное $N(\mu,\sigma^2)$, Гамма $\Gamma(\alpha,\beta)$.

Многомерная СВ $(X,Y)$. Совместная ФР: $F_{X,Y}(x,y)=\mathbb{P}(X<x, Y<y)$. Совместная плотность: $f_{X,Y}(x,y)=\frac{\partial^2 F}{\partial x \partial y}$. Маргинальные: $f_X(x) = \int f_{X,Y}(x,y) dy$.

Матожидание: $\mathbb{E}[X] = \sum x_i p_i$ или $\int x f(x) dx$. Свойства: линейность, $\mathbb{E}[c]=c$, $\mathbb{E}[XY]=\mathbb{E}X\mathbb{E}Y$ при независимости. Дисперсия: $D[X] = \mathbb{E}[(X-\mathbb{E}X)^2] = \mathbb{E}[X^2] - (\mathbb{E}X)^2$. Свойства: $D[cX]=c^2 D[X]$, аддитивность при независимости. Ковариация: $\text{cov}(X,Y)=\mathbb{E}[XY]-\mathbb{E}X\mathbb{E}Y$. Корреляция: $\rho_{XY} = \frac{\text{cov}(X,Y)}{\sqrt{D[X]}\sqrt{D[Y]}}$. $|\rho| \le 1$.

Характеристическая функция: $\varphi_X(t) = \mathbb{E}[e^{itX}]$. Свойства: $\varphi(0)=1, |\varphi(t)|\le 1, \varphi_{X+Y}=\varphi_X\varphi_Y$ (независимость), однозначно определяет распределение, $\varphi^{(k)}(0) = i^k \mathbb{E}[X^k]$.

Неравенство Чебышева: $\mathbb{P}(|X-\mathbb{E}X| \ge \varepsilon) \le \frac{D[X]}{\varepsilon^2}$. ЗБЧ: $\frac{1}{n}\sum X_i \xrightarrow{P} \mathbb{E}X$. ЦПТ: $\frac{\sum X_i - n\mu}{\sigma\sqrt{n}} \xrightarrow{d} N(0,1)$.

Выборка $\vec{x}=(x_1,\dots,x_n)$. Эмпирическая ФР: $F_n^*(x) = \frac{1}{n} \sum \mathbb{I}_{(-\infty, x)}(x_i)$. Гистограмма/полигон — графическое представление частот. Выборочные моменты: $\bar{x} = \frac{1}{n}\sum x_i, s^2 = \frac{1}{n-1}\sum (x_i-\bar{x})^2$.

Оценки $\hat{\theta}$. Свойства: несмещенность ($\mathbb{E}\hat{\theta}=\theta$), эффективность (мин. дисперсия), согласованность ($\hat{\theta} \xrightarrow{P} \theta$). Функция правдоподобия: $L(\theta) = \prod f(x_i;\theta)$. ММП: $\hat{\theta}_{MLE} = \arg\max_\theta \ln L(\theta)$.

Проверка гипотез: $H_0$ vs $H_1$. Ошибка 1-го рода: $\alpha = \mathbb{P}(\text{откл. } H_0 | H_0)$. Ошибка 2-го рода: $\beta$. Мощность: $1-\beta$. Критерий Пирсона: $\chi^2 = \sum \frac{(n_j - n p_j)^2}{n p_j} \sim \chi^2_{k-r-1}$. Отклоняем $H_0$, если $\chi^2_{набл} > \chi^2_{\alpha, df}$.



### 8. Численные методы

Ортогональная система $\{\varphi_n\}$ в $L^2[a,b]$: $(\varphi_n, \varphi_m) = \int_a^b \varphi_n \varphi_m dx = 0$ при $n\neq m$. Процесс Грама-Шмидта: $\psi_1 = v_1, \ \varphi_1 = \psi_1/\|\psi_1\|$, $\psi_k = v_k - \sum_{j=1}^{k-1} (v_k, \varphi_j)\varphi_j, \ \varphi_k = \psi_k/\|\psi_k\|$.

Неравенство Бесселя: $\sum |c_n|^2 \|\varphi_n\|^2 \le \|f\|^2$. Равенство Парсеваля: $\sum |c_n|^2 \|\varphi_n\|^2 = \|f\|^2$ при полноте системы. $c_n = (f,\varphi_n)/\|\varphi_n\|^2$.

Интерполяция Лагранжа: $L_n(x) = \sum_{i=0}^n y_i \prod_{j \neq i} \frac{x-x_j}{x_i-x_j}$. Погрешность: $R_n(x) = \frac{f^{(n+1)}(\xi)}{(n+1)!} \prod (x-x_i)$.

Интерполяция Ньютона: $P_n(x) = \sum_{k=0}^n f[x_0,\dots,x_k] \prod_{i=0}^{k-1}(x-x_i)$. Разделенные разности рекуррентно: $f[x_i,\dots,x_{i+k}] = \frac{f[x_{i+1},\dots,x_{i+k}] - f[x_i,\dots,x_{i+k-1}]}{x_{i+k}-x_i}$.

Метод Эйлера: $y_{n+1} = y_n + h f(x_n, y_n)$. Погрешность $O(h)$. Методы 2-го порядка: $y_{n+1} = y_n + h f(x_n+h/2, y_n + \frac{h}{2}f(x_n,y_n))$. Метод Рунге-Кутта 4-го порядка: $k_1=f(x_n,y_n), k_2=f(x_n+h/2, y_n+h k_1/2), k_3=f(x_n+h/2, y_n+h k_2/2), k_4=f(x_n+h, y_n+h k_3)$, $y_{n+1}=y_n + \frac{h}{6}(k_1+2k_2+2k_3+k_4)$. Погрешность $O(h^4)$.

LU-разложение: $A = LU$. Алгоритм: $u_{ij} = a_{ij} - \sum_{k=1}^{i-1} l_{ik}u_{kj}$, $l_{ji} = (a_{ji} - \sum_{k=1}^{i-1} l_{jk}u_{ki})/u_{ii}$. Метод Гаусса эквивалентен LU. Обратный ход: $x_i = (b_i - \sum_{j=i+1}^n u_{ij}x_j)/u_{ii}$.

Нормы: Векторные: $\|x\|_1 = \sum |x_i|$, $\|x\|_2 = \sqrt{\sum x_i^2}$, $\|x\|_\infty = \max |x_i|$. Матричные: $\|A\|_1 = \max_j \sum_i |a_{ij}|$, $\|A\|_\infty = \max_i \sum_j |a_{ij}|$, $\|A\|_2 = \sqrt{\lambda_{\max}(A^T A)}$. Свойство: $\|Ax\| \le \|A\|\|x\|$.

Итерационные методы СЛАУ: $x^{(k+1)} = B x^{(k)} + g$. Разложение $A = M - N$, $B = M^{-1}N$. Сходимость $\iff \rho(B) < 1$ или $\|B\| < 1$. Метод Якоби: $M=D$. Зейделя: $M=D+L$.

Нелинейные уравнения $f(x)=0$. Методы 0-го порядка: бисекции. 1-го порядка: $x_{k+1}=\varphi(x_k)$. Принцип сжимающего отображения: $|\varphi'(x)|\le q<1 \Rightarrow$ сходимость. Метод Ньютона: $x_{k+1} = x_k - f(x_k)/f'(x_k)$. Многомерный: $x_{k+1} = x_k - [J_F(x_k)]^{-1} F(x_k)$, $J_F$ — матрица Якоби. Порядок сходимости Ньютона: квадратичный.

Минимизация $f(x) \to \min$. Стационарные точки: $\nabla f(x^*) = 0$. Градиентный спуск: $x_{k+1} = x_k - \alpha_k \nabla f(x_k)$. Наискорейший спуск: $\alpha_k = \arg\min_\alpha f(x_k - \alpha \nabla f(x_k))$. Сходимость линейная для выпуклых функций.



### 9. Функциональный анализ и методы оптимизации

Теорема Банаха-Штейнгауза: Пусть $X$ — банахово, $Y$ — нормированное, $\{T_\alpha\} \subset \mathcal{L}(X,Y)$. Если $\sup_\alpha \|T_\alpha x\| < \infty$ для каждого $x \in X$, то $\sup_\alpha \|T_\alpha\| < \infty$.

Теорема Банаха об обратном операторе: Пусть $X, Y$ — банаховы, $T \in \mathcal{L}(X,Y)$ — биекция. Тогда $T^{-1} \in \mathcal{L}(Y,X)$ (обратный оператор линеен и непрерывен).

Функционал $J[y] = \int_a^b L(x, y(x), y'(x)) dx$. Уравнение Эйлера-Лагранжа: $\frac{\partial L}{\partial y} - \frac{d}{dx}\left(\frac{\partial L}{\partial y'}\right) = 0$. Необходимое условие экстремума.

Достаточные условия: 1) Условие Лежандра: $\frac{\partial^2 L}{\partial y'^2} > 0$ (усиленное). 2) Отсутствие сопряженных точек на $(a,b]$. Уравнение Якоби: $-\frac{d}{dx}(P(x)h') + Q(x)h = 0$, $P=L_{y'y'}, Q=L_{yy} - \frac{d}{dx}L_{yy'}$. Сопряженная точка $\xi$: $\exists h \neq 0, h(a)=h(\xi)=0$. Если нет сопряженных точек, экстремум строгий локальный.
