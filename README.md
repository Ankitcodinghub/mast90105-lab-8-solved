# mast90105-lab-8-solved
**TO GET THIS SOLUTION VISIT:** [MAST90105 Lab 8 Solved](https://www.ankitcodinghub.com/product/mast90105-lab-and-workshop-8-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112939&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MAST90105 Lab 8 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1 Lab

In this lab, you will learn how to use R to find a minimum of function and to generate random variables from a given CDF which does not have its inverse in closed form.

1. Function nlm() in R can be used to find a minimum of a nonlinear function.

a. Define a function )) in R and use nlm() to find the minimum of this function.

b. As you have learned, to generate a random variable Z from a continuous distribution with given CDF FZ(z), one can follow these steps:

i. Generate U ∼ U(0,1)

ii. Compute Z = FZ−1(U)

The quantile function FZ−1(q) might not be available in closed form and can be computed numerically. For a strictly increasing CDF FZ(z) there exists a unique solution to the equation: FZ(zq) = q. It implies the function GZ(z) = (FZ(z)−q)2 attains its minimum (which is zero) at z = zq. The point zq at which this minimum is attained can be found using nlm() function in R, and one can follow these steps to generate a random variable Z in this case:

i. Generate U ∼ U(0,1)

ii. Compute Z = argminz(FZ(z) − U)2

Use this approach to generate a sample of size N = 1000 from a continuous random variable with the PDF:

,

Draw a histogram of the generated data.

2. A similar approach can be used to generate a random pair (X,Y ) from a continuous bivariate distribution with given joint CDF FX,Y (x,y). Define

,

where FX(x) and fX(x) are the marginal CDF and PDF of X, respectively. Assuming FX(x) and FY |X(y|x) are strictly increasing and continuously differentiable functions of x and y, respectively, one can follow these steps to generate a random pair (X,Y ):

a. Generate independent UX ∼ U(0,1) and UY ∼ U(0,1)

b. Compute

c. Compute

The inverse CDFs FX−1 and can be computed numerically using nlm() function if they are not available in closed form.

a. Bonus: Show that the joint CDF of (X,Y ) generated using the algorithm above is FX,Y .

b. Use this algorithm to generate a sample of size N = 1000 from a continuous bivariate random variable (X,Y ) with the joint PDF:

,

Draw a scatter plot of the generated data.

2 Workshop

1. a. A random sample X1,…,Xn of size n is taken from a Poisson distribution with mean λ &gt; 0.

i. Show the maximum likelihood estimator of λ is λˆ = X¯.

ii. Suppose with n = 40 we observe 5 zeros, 7 ones, 12 twos, 9 threes, 5 fours, 1 five, and 1 six. What is the maximum likelihood estimate of λ.

b. Find the maximum likelihood estimator, θˆ, if X1,··· ,Xn is a random sample from the following probability density function:

f(x;θ) = (1/2)exp(−|x − θ|),−∞ &lt; x &lt; ∞,0 &lt; θ &lt; ∞

This involves minimizing , which is difficult. Try n = 5 and a sample 6.1, -1.1, 3.2, 0.7, 1.7.Then deduce the MLE.

2. Let f(x;θ) = θxθ−1, 0 &lt; x &lt; 1, θ ∈ Ω = {θ : 0 &lt; θ &lt; ∞} and let X1,…,Xn denote a random sample from this distribution. Note that

a. Sketch the p.d.f. of X for θ = 1/2 and θ = 2.

b. Show that ) is the maximum likelihood estimator of θ.

c. For each of the following three sets of observations from this distribution compute the maximum likelihood estimates and the methods of moments estimates.

X Y

Z

0.0256 0.9960 0.4698

0.3051 0.3125 0.3675

0.0278 0.4374 0.5991

0.8971 0.7464 0.9513

0.0739 0.8278 0.6049

0.3191 0.9518 0.9917

0.7379 0.9924 0.1551

0.3671 0.7112 0.0710

0.9763 0.2228 0.2110

0.0102 0.8609 0.2154

(Pni=1 ln(xi) = −18.2063, Pni=1 ln(yi) = −4.5246, Pni=1 ln(zi) = −10.42968, Pni=1 xi = 3.7401, Pni=1 yi = 7.0592, Pni=1 zi = 4.6368.)

3. Let X1,…,Xn be a random sample from the exponential distribution whose p.d.f. is f(x;θ) = (1/θ)exp(−x/θ), 0 &lt; x &lt; ∞, 0 &lt; θ &lt; ∞.

a. Show that X¯ is an unbiased estimator of θ.

b. Show that the variance of X¯ is θ2/n. What is a good estimate of θ if a random sample of size 5 yielded the values 3.5, 8.1, 0.9, 4.4 and 0.5?

4. Let X1,…,Xn be a random sample from a distribution having finite variance σ2. Show that is an unbiased estimator of σ2. HINT: Write

!

and compute E(S2).

5. Let X1,…,Xn be a random sample of size n from the distribution with p.d.f. f(x;θ) = (1/θ)x(1−θ)/θ, 0 &lt; x &lt; 1.

a. Show the mean of X is E(X) = 1/(1 + θ).

b. Show the maximum likelihood estimator of θ is

c. Is the MLE unbiased? (You can do this using integration by parts combined with

rules about expectation of the sample mean.)

d. Show the method of moments estimator of θ is

.
