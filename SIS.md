
# <font color=gold>SIS Model with constant number of carriers:</font>

## Carriers :
***

<font color=lightgreen>    

### Carriers are those individuals , who although apparantely healthy themselves, harbour injection which can be transmitted to others .
### Sometime carrier may be flies, mosqutos, etc . Infection may also be derived indirrectly through virus contaminated food or liquid rather than by dirrect contact with an infective .



***

### Let constant number of carriers $C$ spread infection among susceptible individuals along with the infected individuals $I$ , then

### Model becomes , 

$$

\frac{dS}{dt} = \beta \ S(I + C) + \gamma \ I \ ..........(1)
$$

$$
\frac{dI}{dt} = \beta \ S(I + C)-\gamma \ I \ ..........(2)
$$

$$S_0 > 0 \ ,\ I_0 \geq 0$$

### and , 
$S_0 + I_0 = N = S(t) + I(t) .$

### Using ,
$S = N-I$ in $(2)$ we get as ,

$$

\frac{dI}{dt} = \beta \ (N-I)(I+C)-\gamma \ I

$$

$$
\frac{dI}{dt} = \beta \left(NI + NC - I^2 -IC  \right)-\gamma \ I 
$$
### or ,
$$
\frac{dI}{dt}  = \beta \left(N-C-\frac{\gamma}{\beta}\right)I + \beta \ NC -\beta \ I^2
$$

$$Let\ ,\ \frac{\gamma}{\beta} = \rho $$

$$
\implies \frac{dI}{dt} = \beta NC + \beta\left(N-C-\rho\right) - \beta I^2
$$
### Multiplying both sides by $\beta , $  we get as , 
$$
\beta \frac{dI}{dt} = \beta^2NC + \beta^2\left(N-C-\rho\right) - \beta^2 I^2
$$

$$Let, \ \beta I = J$$

$$\implies \beta \frac{dI}{dt} = \frac{dJ}{dt}$$
$$\frac{dJ}{dt} = \beta^2NC + \beta \left(N-C-\rho \right)J - J^2$$

### or , 

$$\frac{dJ}{dt} = -\left | \left(J-\alpha_1\right)\left(J-\alpha_2\right) \right|$$

### Where, $\alpha_1+\alpha_2 = \beta\left(N-C-\rho\right)$ 

$\alpha_1  \alpha_2 = -\beta^2NC$

$\therefore \left(\alpha_1 -\alpha_2\right)^2 = \left(\alpha_1 +\alpha_2\right)^2-4\alpha_1  \alpha_2 $
               
$\left(\alpha_1 -\alpha_2\right)^2 = \beta^2\left(N-C-\rho\right)^2 - 4\left(-\beta^2NC\right)$    

$$
\alpha_1-\alpha_2 = \sqrt{\beta^2\left(N-C-\rho\right)^2 + 4\left(\beta^2NC\right)}
$$

$$
\alpha_1 = \frac{1}{2}\left[\beta\left(N-C-\rho\right)+ \sqrt{\beta^2\left(N-C-\rho\right)^2 + 4\left(\beta^2NC\right)}\right]
$$

$$
\alpha_2 = \frac{1}{2}\left[\beta\left(N-C-\rho\right)- \sqrt{\beta^2\left(N-C-\rho\right)^2 + 4\left(\beta^2NC\right)}\right]
$$

### Seprating the Variables , 

$$
\int\frac{dJ}{\left(J-\alpha_1\right)\left(J-\alpha_2\right)} = 
-\int dt$$

$$
\implies \frac{1}{\alpha_1-\alpha_2}\int\left(\frac{1}{J-\alpha_1}-\frac{1}{J-\alpha_2}\right)dJ = -\int dt
$$

$$
\implies \frac{1}{\alpha_1-\alpha_2}\left(\log\frac{\left(J-\alpha_1\right)}{\left(J-\alpha_2\right)}\right) = -t + C
$$

### when, $t =0, J(0) = J_0=\beta I_0$ then ,

$$
\frac{1}{\alpha_1-\alpha_2}\log\left(\frac{J_0 - \alpha_1}{J_0-\alpha_2}\right) = C
$$

$$
\therefore \frac{1}{\alpha_1-\alpha_2}\log\left(\frac{J-\alpha_1}{J-\alpha_2}\right) - \frac{1}{\alpha_1-\alpha_2}\log\left(\frac{J_0-\alpha_1}{J_0-\alpha_2}\right) = -t 
$$

$$
\log\frac{J-\alpha_1}{J-\alpha_2} \cdot \frac{J_0-\alpha_2}{J_0-\alpha_1} = -\left(\alpha_1-\alpha_2\right)\cdot t
$$

$$
\frac{J-\alpha_1}{J-\alpha_2}\cdot \left(\frac{J_0-\alpha_2}{J_0-\alpha_1}\right) = e^{-\left(\alpha_1-\alpha_2\right)\cdot t
}
$$

$$
\frac{J-\alpha_1}{J-\alpha_2} = \left(\frac{J_0-\alpha_1}{J_0-\alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t
}
$$

$$
J-\alpha_1 = \left(J-\alpha_2\right)  \left(\frac{J_0-\alpha_1}{J_0-\alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t}
$$

$$
J\left \{ 1 -\left(\frac{J_0+\alpha_1}{J_0+\alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t
}\right\} = \alpha_1-\alpha_2 \cdot \left(\frac{J_0-\alpha_1}{J_0- \alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t}
$$

$$
J = \frac{\alpha_1-\alpha_2 \cdot \left(\frac{J_0-\alpha_1}{J_0- \alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t}}{\left \{ 1 -\left(\frac{J_0+\alpha_1}{J_0+\alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t
}\right\}}
$$

### Since $J = \beta I$ then , 
***
$$
I = \frac{\alpha_1-\alpha_2 \cdot \left(\frac{J_0-\alpha_1}{J_0- \alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t}}{\beta \cdot\left \{ 1 -\left(\frac{J_0+\alpha_1}{J_0+\alpha_2}\right)\cdot e^{-\left(\alpha_1-\alpha_2\right)\cdot t
}\right\}}
$$
***