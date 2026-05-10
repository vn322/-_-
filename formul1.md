### 1. Математический анализ

$\lim_{x \to x_0} f(x) = A \iff \forall \varepsilon > 0 \, \exists \delta > 0 : 0 < |x - x_0| < \delta \Rightarrow |f(x) - A| < \varepsilon$.
$x, x_0, A, \varepsilon, \delta \in \mathbb{R}$ — аргумент, точка сходимости, предел, произвольно малые числа. $f: D \to \mathbb{R}$ — функция.


$f \in C[x_0] \iff \lim_{x \to x_0} f(x) = f(x_0)$.
$C$ — класс непрерывных функций. $x_0$ — точка области определения.


$f'(x_0) = \lim_{\Delta x \to 0} \frac{f(x_0+\Delta x)-f(x_0)}{\Delta x}$.
$\Delta x$ — приращение аргумента. $f'$ — производная в точке $x_0$.


$f(x_0)=\max/\min \Rightarrow f'(x_0)=0$.
Теорема Ферма. $x_0$ — точка локального экстремума внутренней области.


$f \in C[a,b] \cap D(a,b), f(a)=f(b) \Rightarrow \exists \xi \in (a,b): f'(\xi)=0$.
Теорема Ролля. $D$ — дифференцируемые функции.


$\exists \xi \in (a,b): f(b)-f(a) = f'(\xi)(b-a)$.
Теорема Лагранжа. $\xi$ — промежуточная точка.


$\exists \xi \in (a,b): \frac{f(b)-f(a)}{g(b)-g(a)} = \frac{f'(\xi)}{g'(\xi)}, \, g'(x)\neq 0$.
Теорема Коши. $f,g$ — функции на $[a,b]$.


$\int_a^b f(x)dx = \lim_{\lambda(\Pi)\to 0} \sum_{i=1}^n f(\xi_i)\Delta x_i$.
Интеграл Римана. $\Pi$ — разбиение, $\lambda$ — диаметр разбиения, $\xi_i \in [x_{i-1}, x_i]$.


$\int_a^b f(x)dx = F(b)-F(a), \, F'(x)=f(x)$.
Формула Ньютона-Лейбница. $F$ — первообразная.


$\int_a^\infty f(x)dx = \lim_{b\to\infty} \int_a^b f(x)dx$.
Несобственный интеграл. Сходится, если предел конечен.


$\sum a_n$ сходится $\iff \forall \varepsilon>0 \, \exists N \, \forall n>N, p\in\mathbb{N}: |\sum_{k=1}^p a_{n+k}|<\varepsilon$.
Критерий Коши для рядов. $a_n \in \mathbb{C}$.


$R = \frac{1}{\limsup_{n\to\infty} \sqrt[n]{|a_n|}}$.
Радиус сходимости степенного ряда $\sum a_n(x-x_0)^n$.


$f(x) = \sum_{n=0}^\infty \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n$.
Ряд Тейлора. $f^{(n)}$ — $n$-я производная.


$|S_n(x)-S(x)|<\varepsilon \, \forall n>N, x\in E$.
Равномерная сходимость функционального ряда. $S_n$ — частичная сумма, $S$ — сумма.


$\forall \varepsilon>0 \, \exists N: |u_n(x)| \le M_n, \sum M_n < \infty \Rightarrow$ равномерная сходимость.
Признак Вейерштрасса. $M_n$ — мажоранта.


$\sum |a_n| < \infty \Rightarrow \sum a_n$ сходится. $c_n = \sum_{k=0}^n a_k b_{n-k}$.
Абсолютная сходимость и произведение рядов Коши.


---

### 2. Алгебра и аналитическая геометрия

$\frac{x-x_0}{l} = \frac{y-y_0}{m} = \frac{z-z_0}{n}$.
Каноническое уравнение прямой. $(x_0,y_0,z_0)$ — точка, $\vec{s}=(l,m,n)$ — направляющий вектор.


$A(x-x_0)+B(y-y_0)+C(z-z_0)=0$.
Уравнение плоскости. $\vec{n}=(A,B,C)$ — нормальный вектор.


$Ax^2+Bxy+Cy^2+Dx+Ey+F=0 \to \frac{x^2}{a^2}\pm\frac{y^2}{b^2}=1$ и др.
Кривые второго порядка. Приведение к каноническому виду: инварианты или аффинные преобразования.


$A\vec{x}=\vec{b}$. $\text{rank}(A) = \text{rank}(\bar{A})$.
Теорема Кронекера-Капелли. $\bar{A}$ — расширенная матрица.


$$\vec{x} = \vec{x}_0 + \sum_{i=1}^k c_i \vec{v}_i, \, k=n-\text{rank}(A)$$

Общее решение СЛАУ. $\vec{x}_0$ — частное, $\{\vec{v}_i\}$ — фундаментальная система решений (ФСР).


$A\vec{v} = \lambda \vec{v}, \, \det(A-\lambda I)=0$.
Собственные векторы и значения. $\lambda$ — корень характеристического многочлена.


$A(\alpha \vec{u} + \beta \vec{v}) = \alpha A\vec{u} + \beta A\vec{v}$.
Линейный оператор. $\vec{u},\vec{v} \in V, \alpha,\beta \in \mathbb{F}$. Действия: сложение/умножение на скаляр/композиция определяются покомпонентно или матрично.


---

### 3. Дифференциальные уравнения

$y' = f(x,y), \, y(x_0)=y_0$.
Задача Коши. $\exists!$ решение, если $f, \partial f/\partial y$ непрерывны в окрестности $(x_0,y_0)$.


$y'' + p(x)y' + q(x)y = 0$. 

$$W(y_1,y_2)(x) = \det\begin{pmatrix} y_1 & y_2 \\ 
y_1' & y_2' \end{pmatrix} \neq 0$$

Линейное однородное уравнение 2-го порядка. $W$ — определитель Вронского.


$\dot{V}(\vec{x}) = \nabla V \cdot \vec{f}(\vec{x}) \le 0 \Rightarrow$ устойчивость. $\dot{V} < 0 \Rightarrow$ асимптотическая устойчивость.
Теорема Ляпунова. $V(\vec{x}) > 0$ — функция Ляпунова.


$\exists V: V(0)=0, \dot{V}>0$ в области $\Omega \ni 0 \Rightarrow$ 

неустойчивость.Теорема Четаева. $\Omega$ — область, где $V>0$.


$a(x,u)\frac{\partial u}{\partial x} + b(x,u)\frac{\partial u}{\partial y} = c(x,u)$.
Квазилинейное УрЧП 1-го порядка. Решение: система характеристик $\frac{dx}{a} = \frac{dy}{b} = \frac{du}{c}$.


$-\Delta u = f$ в 

$$\Omega, \, u|_{\partial\Omega}=g$. $\int_\Omega \nabla u \cdot \nabla v \, dx = \int_\Omega f v \, dx$$

Эллиптическая задача. Разрешимость: теорема Фредгольма. Гладкость: $u \in H^{s+2}$ при $f \in H^s$.


$W^{k,p}(\Omega) = \{u \in L^p : D^\alpha u \in L^p, |\alpha|\le k\}$. $W^{k,p} \hookrightarrow C^m$ при $k > m + n/p$.
Пространство Соболева и теорема вложения. $D^\alpha$ — слабая производная.


$u(x,t) = \sum_{n=1}^\infty T_n(t) X_n(x)$. $-\Delta X_n = \lambda_n X_n$.
Метод Фурье. $X_n$ — собственные функции, $T_n$ — временные коэффициенты.


$\langle Au_N, \phi_j \rangle = \langle f, \phi_j \rangle, \, u_N = \sum_{i=1}^N c_i \phi_i$.
Метод Галеркина. $\{\phi_i\}$ — базис, $\langle\cdot,\cdot\rangle$ — скалярное произведение.


$\frac{du}{dt} = Au, \, u(0)=u_0 \Rightarrow u(t)=T(t)u_0$. $T(t+s)=T(t)T(s), \lim_{t\to 0}T(t)=I$.
Полугруппы операторов. Сильная непрерывность гарантирует решение задачи Коши.


---

### 4. Комплексный анализ

$f(z)=u+iv$. $\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$.
Условия Коши-Римана. $f$ дифференцируема $\Leftrightarrow$ выполнены условия.


$f'(z_0) = |f'(z_0)| e^{i \arg f'(z_0)}$.
Геометрический смысл: $|f'|$ — коэффициент растяжения, $\arg f'$ — угол поворота.


$\oint_\gamma f(z)dz = 0$, если $f$ голоморфна в области $D \supset \gamma$.
Теорема Коши. $\gamma$ — замкнутый спрямляемый контур.


$f^{(n)}(z_0) = \frac{n!}{2\pi i} \oint_\gamma \frac{f(z)}{(z-z_0)^{n+1}} dz$.
Интегральная формула Коши. $n \in \mathbb{N}_0$.


$f(z) = \sum_{n=-\infty}^\infty c_n (z-z_0)^n$. $\text{Res}(f,z_0) = c_{-1}$.
Ряд Лорана и вычет. Особые точки: устранимая ($c_n=0, n<0$), полюс ($c_{-m}\neq 0, c_n=0, n<-m$), существенно особая (бесконечно много $c_{n<0}$).


---

### 5. Дискретная математика

$C_n^k = \frac{n!}{k!(n-k)!}, A_n^k = \frac{n!}{(n-k)!}, P_n = n!$.
Сочетания, размещения, перестановки. $n,k \in \mathbb{N}$.


$|\bigcup_{i=1}^n A_i| = \sum |A_i| - \sum |A_i\cap A_j| + \dots + (-1)^{n-1}|\bigcap A_i|$.
Формула включений-исключений. $A_i$ — конечные множества.


$(a+b)^n = \sum_{k=0}^n C_n^k a^{n-k}b^k$.
Бином Ньютона.


$F(x_1,\dots,x_n)$ СДНФ/СКНФ. Минимизация: таблица простых импликант $\to$ покрытие $\to$ метод Куайна-Мак-Класки.
Булевы функции. Эквивалентные преобразования сохраняют таблицу истинности.


$A(x) = \sum_{n=0}^\infty a_n x^n$. $\{a_n\} \leftrightarrow A(x) \cdot B(x) = \sum c_n x^n, c_n = \sum a_k b_{n-k}$.
Производящие функции. Свойство: умножение соответствует свертке.


$a_n + c_1 a_{n-1} + \dots + c_k a_{n-k} = 0 \Rightarrow \lambda^k + c_1 \lambda^{k-1} + \dots + c_k = 0$.
Линейные рекуррентные соотношения. Решение: $a_n = \sum P_j(n) \lambda_j^n$.


---

### 6. Теория вероятностей и математическая статистика

$\mathbb{P}: \mathcal{F} \to [0,1], \mathbb{P}(\Omega)=1, \mathbb{P}(\cup A_i) = \sum \mathbb{P}(A_i)$.
Аксиомы вероятности. $\mathcal{F}$ — $\sigma$-алгебра событий.


$\mathbb{P}(A|B) = \frac{\mathbb{P}(AB)}{\mathbb{P}(B)}$. $\mathbb{P}(A) = \sum \mathbb{P}(A|H_i)\mathbb{P}(H_i)$.
Условная вероятность и формула полной вероятности. $H_i$ — полная группа.


$\mathbb{P}(H_i|A) = \frac{\mathbb{P}(A|H_i)\mathbb{P}(H_i)}{\sum \mathbb{P}(A|H_j)\mathbb{P}(H_j)}$.
Формула Байеса.


$P_n(k) = C_n^k p^k (1-p)^{n-k}$.
Схема Бернулли. $p$ — вероятность успеха.


$F_X(x) = \mathbb{P}(X < x)$. Дискретная: $p_i = \mathbb{P}(X=x_i)$. Непрерывная: $F'(x)=f(x) \ge 0, \int f dx = 1$.
Функция распределения и плотность.


$\mathbb{E}[X] = \sum x_i p_i$ или $\int x f(x) dx$. $D[X] = \mathbb{E}[X^2] - (\mathbb{E}X)^2$.
Математическое ожидание и дисперсия. Свойства: линейность $\mathbb{E}$, аддитивность $D$ при независимости.


$\text{cov}(X,Y) = \mathbb{E}[XY] - \mathbb{E}X\mathbb{E}Y$. $\rho = \frac{\text{cov}}{\sqrt{DX}\sqrt{DY}}$.
Ковариация и коэффициент корреляции. $|\rho| \le 1$.


$\mathbb{P}(|X-\mathbb{E}X| \ge \varepsilon) \le \frac{DX}{\varepsilon^2}$.
Неравенство Чебышева. $\varepsilon > 0$.


$\frac{1}{n}\sum X_i \xrightarrow{P} \mathbb{E}X$ (ЗБЧ). $\frac{\sum X_i - n\mu}{\sigma\sqrt{n}} \xrightarrow{d} \mathcal{N}(0,1)$ (ЦПТ).
Предельные теоремы. $X_i$ — независимые одинаково распределённые.


$\varphi_X(t) = \mathbb{E}[e^{itX}]$. $\varphi_{X+Y} = \varphi_X \varphi_Y$.
Характеристическая функция. Свойства: определяет распределение однозначно.


$F_n^*(x) = \frac{1}{n}\sum_{i=1}^n \mathbb{I}_{(-\infty, x)}(x_i)$. $\bar{x} = \frac{1}{n}\sum x_i, s^2 = \frac{1}{n-1}\sum (x_i-\bar{x})^2$.
Эмпирическая функция распределения и выборочные моменты.


$$L(\theta) = \prod_{i=1}^n f(x_i;\theta)$. $\hat{\theta}_{MLE} = \arg\max_\theta L(\theta)$$

Функция правдоподобия и оценки максимального правдоподобия.


$\alpha = \mathbb{P}(\text{откл. } H_0 | H_0)$. $1-\beta = \mathbb{P}(\text{откл. } H_0 | H_1)$. $\chi^2 = \sum \frac{(O_i-E_i)^2}{E_i}$.
Уровень значимости, мощность критерия, критерий согласия Пирсона. $H_0, H_1$ — гипотезы.


---

### 7. Численные методы

$$\|\vec{x}\|_1 = \sum |x_i|, \|\vec{x}\|_2 = \sqrt{\sum x_i^2}, \|\vec{x}\|_\infty = \max |x_i|$. $\|A\| = \sup_{\|\vec{x}\|=1} \|A\vec{x}\|$$

Нормы векторов и матриц. Согласованность: $\|A\vec{x}\| \le \|A\|\|\vec{x}\|$.


$A = LU$. Прямой ход: приведение к треугольному виду. Обратный ход: подстановка.
Метод Гаусса и LU-разложение. $L$ — нижнетреугольная, $U$ — верхнетреугольная.


$$\vec{x}^{(k+1)} = B\vec{x}^{(k)} + \vec{c}$. Сходимость $\iff \rho(B) < 1$$

Итерационные методы СЛАУ. $\rho$ — спектральный радиус.


$L_n(x) = \sum_{i=0}^n y_i \prod_{j \neq i} \frac{x-x_j}{x_i-x_j}$. $P_n(x) = \sum_{k=0}^n f[x_0,\dots,x_k] \prod_{i=0}^{k-1}(x-x_i)$.
Интерполяция Лагранжа и Ньютона. $f[\cdot]$ — разделённые разности.


$y_{n+1} = y_n + h f(x_n, y_n)$. $y_{n+1} = y_n + \frac{h}{6}(k_1+2k_2+2k_3+k_4)$.
Методы Эйлера и Рунге-Кутта 4-го порядка. $h$ — шаг, $k_i$ — промежуточные наклоны.


$\vec{e}_k = \vec{v}_k - \sum_{j=1}^{k-1} \frac{\langle \vec{v}_k, \vec{e}_j \rangle}{\langle \vec{e}_j, \vec{e}_j \rangle} \vec{e}_j$. $\sum |\langle f, \varphi_n \rangle|^2 \le \|f\|^2$

Процесс Грама-Шмидта и неравенство Бесселя. $\{\varphi_n\}$ — ортогональная система.


$\sum |\langle f, \varphi_n \rangle|^2 = \|f\|^2$ при полноте системы.
Равенство Парсеваля.


$x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}$ 

$$\|\varphi(x)-\varphi(y)\| \le q\|x-y\|, q<1 \Rightarrow x^*=\varphi(x^*)$$

Метод Ньютона и принцип сжимающего отображения. $\varphi$ — итерационная функция.


$$\nabla f(\vec{x}^*) = 0$. $\vec{x}_{k+1} = \vec{x}_k - \alpha_k \nabla f(\vec{x}_k)$$

Стационарные точки и метод градиентного спуска. $\alpha_k$ — шаг спуска.


---

### 8. Функциональный анализ и методы оптимизации

$\sup_n \|T_n x\| < \infty \, \forall x \in X \Rightarrow \sup_n \|T_n\| < \infty$.
Теорема Банаха-Штейнгауза. $T_n \in \mathcal{L}(X,Y)$, $X$ — банахово.


$T: X \to Y$ биективен, линеен, непрерывен $\Rightarrow T^{-1}$ непрерывен.
Теорема Банаха об обратном операторе. $X,Y$ — банаховы пространства.


$J[y] = \int_a^b L(x,y,y') dx$. $\frac{\partial L}{\partial y} - \frac{d}{dx}\frac{\partial L}{\partial y'} = 0$.
Функционал и уравнение Эйлера-Лагранжа. Необходимое условие экстремума.


$L_{y'y'} > 0$ (Лежандр), сопряжённых точек нет на $(a,b]$.
Достаточные условия экстремума. Сопряжённая точка: $h(a)=0, h(\xi)=0$ для уравнения Якоби.
