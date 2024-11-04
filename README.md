java c
ELEN 4810 Midterm Exam 
1. Systems in Time and Frequency. Consider the causal linear, time invariant system corre-sponding to the following block diagram:

Here, D1 denotes an ideal delay by one sample, and the triangular blocks denote multiplication by complex scalars α and β, respectively.
Please answer the following questions: 
Part (a). For what α and β is the system stable?
[Note: for full credit, please specify all possible values of (α, β)]
Part (b). What is the frequency response H(ejω) of the system?
[Note: here, you only need to consider values of (α, β) for which the system is stable]
Part (c). What is the impulse response h[n] of the system? Is this an FIR or IIR system?
Part (d). Consider the constant input x[n] = 1. For what choices of (α, β) is the output y[n] = 0 zero for all n? Please make your answer as broad as possible, or if no such (α, β) exist, explain why.
Part (e). Consider the input x[n] = 1 + 3(−1)n. For what choices of (α, β) is the output y[n] = 0 zero for all n? Again, please make your answer as broad as possible, or if no such (α, β) exist, explain why.
2. LTI Systems in Frequency Domain. A signal x[n] is input to an LTI system with impulse response h[n], producing output y[n]. Below, we plot magnitude and phase of X(ejω) and Y (ejω).
Part (a). Please plot the magnitude and phase of H(ejω). Please label your graph as clearly as possible (including heights), and indicate any points for the magnitude or phase response cannot be determined:

Your answer to Part (a) here: 

Part (b). For which of the following signals x[n] is it possible to determine the impulse response h[n] from the convolution y[n] = x[n] ∗ h[n]? Please briefly explain your answers:
• 1. x[n] = 
• 2. x[n] = cos(nπ/4)
• 3. x[n] = δ[n − 10]
• 4. x[n] = (1/4)nu[n]
3. Sampling and Aliasing. Consider the following block diagram:

Here,
• xc(t) is a continuous time signal
• Haa(jΩ) is a continuous time filter whose frequency response will be specified below
• xf (t) is a continuous-time signal
• The box marked R will be specifed below.
Please answer the following questions: 
Part (a). Suppose that R is an ideal discrete to continuous converter, with period T seconds. We wish to ensure that yc(t) = xc(t代 写ELEN 4810 Midterm Exam 2023R
代做程序编程语言) for the broadest possible set of inputs xc(t).
How should we choose Haa(jΩ)?
[Note: please specify Haa as a function of Ω. Your answer should depend on T]
Part (b). With your choice of Haa from part (a), for which inputs xc can we guarantee that yc(t) = xf (t)?
[Note: Please make your answer as broad as possible for full credit. Please notice that Part (b) of the question asks whether yc = xf , not whether yc = xc!]
Part (c). Now suppose we are interested in reconstructing bandlimited signals xc(t) satisfying
Xc(jΩ) = 0,   |Ω| ≥ ΩM.                         (1)
Suppose further that we know that the input signal xc(t) is real valued. We can use this property to reduce the sampling rate, by making different choices of the filter Haa and the block R.
Please specify a filter Haa(jΩ), a sampling period T, and describe a reconstruction procedure R which ensures yc(t) = xc(t) for all such bandlimited, real-valued xc(t). For full credit, please make T as large as possible!
[Hint: You may find it helpful to note that for a real valued signal xc(t), the Fourier transform. is conjugate symmetric: Xc(jΩ) = Xc(−jΩ)∗ ]
4. Discrete Fourier Transform. and Convolution with a Filterbank. Consider real-valued discrete-time signal x[n], which satisfies

We are given a collection of filters h1[n], . . . , h7[n] satisfying

We wish to compute the (linear) convolutions y1 = x ∗ h1, y2 = x ∗ h2, . . . , y7 = x ∗ h7 of x with each of the filters hi.
Please consider the following proposed procedure: we compute the discrete fourier transforms
X = DFTN {x},
Hi = DFTN {hi}, i = 1, . . . , 7.
and set
yi[n] = DFT−N1{Hi[k]X[k]}, i = 1, . . . , 7.
Please answer the following questions about this procedure: 
Part 1. Suppose we set N = 150. Which of the convolutions is computed correctly? I.e., for which values of i is yi[n] = yi[n] for all n?
Part 2. What is the smallest N for which all of the convolutions are computed correctly? I.e., for which N is yi[n] = yi[n] for all n and all i = 1, . . . , 7?
Part 3. Suppose again that N = 150, but now that we only care about values of n satisfying 10 ≤ n ≤ 118. For which i is it true that
yi[n] = yi[n]   n = 10, . . . , 119 ? (4)









         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
