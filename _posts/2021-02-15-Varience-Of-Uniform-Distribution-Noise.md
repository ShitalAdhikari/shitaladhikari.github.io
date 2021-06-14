
# Finding the Variance of uniform filter


![](https://www.researchgate.net/profile/Anantkumar-Pimpale/publication/316525043/figure/fig1/AS:487799678869504@1493311914825/PDF-for-Uniform-noise.png)

$E(\bar{X}) = \frac{a+b}{2}$

$\sigma^2$ = ?

From Probability density function:

$E(X)= \int xf(x)dx$$

$\sigma^2 = E[(x-\bar{X})^2]$

$E[(x-\bar{X})^2] = \int_{\infty}^\infty (x-\mu)^2f(x)dx$ 

$=\int_{\infty}^\infty(x^2 - 2\mu x + \mu^2)f(x)dx$

$=\int_{\infty}^\infty x^2 f(x)dx - \int_{\infty}^\infty 2\mu x f(x)dx + \int_{\infty}^\infty\mu^2f(x)dx$

$=\int_{\infty}^\infty x^2 f(x)dx - 2\mu\int_{\infty}^\infty x f(x)dx + \int_{\infty}^\infty\mu^2f(x)dx$


Since, $\int_{\infty}^\infty x f(x)dx$ is mean $\mu$


$=\int_{\infty}^\infty x^2 f(x)dx - 2\mu^2 + \mu^2\int_{\infty}^\infty f(x)dx$  

Probability density function under the curve $\int_{\infty}^\infty f(x)dx$ is $1$

$=\int_{\infty}^\infty x^2 f(x)dx - 2\mu \mu + \mu^2$

$=E(x^2) - \mu^2$

$=E(x^2)- [E(x)]^2$

Now we can use the above equation to find the variance of the uniform distribution function

$\sigma^2 = E[(x-\mu)^2]$

$=E(x^2) - [E(x)]^2$

$=\int_{\infty}^\infty x^2 f(x)dx - (\frac{b+a}{2})^2$

$=\int_{-\infty}^a x^2 f(x) + \int_{a}^b x^2 f(x) + \int_{-\infty}^a x^2 f(x) - (\frac{b+a}{2})^2$

Since, probability density function is only between a and b. $1st$ and $3rd$ integral becomes 0.

$=\int_{a}^b x^2 \frac{1}{b-a} dx - (\frac{b+a}{2})^2$

$=\frac{a}{b-a}[\frac{x^3}{3}]_{a}^b- (\frac{b+a}{2})^2$

$=\frac{a}{b-a}[\frac{b^3}{3} - \frac{a^3}{3}]- (\frac{b+a}{2})^2$

$=\frac{(a-b)^2}{12}$


