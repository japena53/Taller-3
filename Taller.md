# Taller-3
Procesos estocastivos
{
 "metadata": {
  "name": "",
  "signature": "sha256:77beaff26aaeffc9c165d9f73ca5907d5544d48990aab267d59c05cfa63c23c4"
 },
 "nbformat": 3,
 "nbformat_minor": 0,
 "worksheets": [
  {
   "cells": [
    {
     "cell_type": "markdown",
     "metadata": {},
     "source": [
      "<h1>Taller 3</h1>\n",
      "\n",
      "1)\n",
      "\n",
      " \n",
      "  <p>$$ fx (x)  = \\frac{x^k-1 {e}^{-x/\\Theta}}  {\\Theta \\Gamma (k)} I  (0,\\infty) (x)$$</p>\n",
      "  \n",
      " <p>$ E [ x ]  = (k)\\Theta $</p>\n",
      " \n",
      " <p>$ E [ x ]^2  = (k)\\Theta^2  $</p>\n",
      " \n",
      "  <p>$ E [ x ]  = \\int\\limits_ {-\\infty}^\\infty fx (x) = \\int_0^\\infty \\mathrm{X} \\frac{1}{\\Theta  \\Gamma (k)}  X^{(k-1)} {e}^{-x/\\Theta} {\\mathrm d x} = \\frac{1}{\\Theta^k \\Gamma (k)}$</p>\n",
      " <p>$\\int_0^\\infty \\mathrm{X^k} {e}^{-x/\\Theta}{\\mathrm d x}$</p>\n",
      "\n",
      "<p>$u= \\frac{\\mathrm x}{\\mathrm \\Theta}$</p>\n",
      "<p>$x= u\\Theta$</p>\n",
      "\n",
      "<p>$ E [ x ]  = \\frac{1}{\\Theta^k \\Gamma (k)}\\int_0^\\infty \\mathrm{u\\Theta^k} {e}^u \\Theta du \\frac{\\mathrm \\Theta}{\\mathrm \\Gamma k} \\int_0^\\infty \\mathrm{u^k} {e}^{-u} du = \\frac{\\Theta \\Gamma (k+1)}{ \\Gamma (k)} = {\\Theta k}$</p>\n",
      "\n",
      "<p>$ E [ x ]^2  = \\int\\limits_ {-\\infty}^\\infty {x^2 } f(x) dx = \\int\\limits_ {0}^\\infty {x^2 } \\frac{1}{\\Theta^k \\Gamma (k)} x^{k-1} {e}^{-k/\\Theta} dx = \\frac{1}{\\Theta^k \\Gamma (k)} \\int\\limits_ {0}^\\infty x^{k+1} {e}^{-k/\\Theta} dx$</p>\n",
      "\n",
      "\n",
      "<p>$u= \\frac{\\mathrm x}{\\mathrm \\Theta}$</p>\n",
      "\n",
      "<p>$x= u\\Theta$</p>\n",
      "\n",
      "<p>$dx= \\Theta du$</p>\n",
      "\n",
      "<p>$ E [x^2]  = \\frac{1}{\\Theta^k  \\Gamma (k)} \\int\\limits_ {0}^\\infty u\\Theta^{k+1} {e}^{u}du\\Theta = \\frac{\\Theta^2}{ \\Gamma (k)} \\int\\limits_ {0}^\\infty u^{k+1} {e}^{-u} du = \\frac{\\Theta^2 \\Gamma (k + 2)}{ \\Gamma (k)}$</p>\n",
      "<p>$ \\frac{\\Theta^2 (k+1) k\\Gamma (k)}{ \\Gamma (k)} = (k+1)k \\Theta^2$</p>\n",
      "\n",
      "<p>$ \\implies var[x] =  E [x^2] - E [x]^2  = (k+1)K\\Theta^2 - (k\\Theta)^2 = K^2\\Theta^2 + k\\Theta^2 - K^2\\Theta^2  = K\\Theta^2 $</p>\n",
      "\n",
      "\n",
      "2)\n",
      "\n",
      "<p>$\n",
      " f(x,y) = \\left\\{ \n",
      "  \\begin{array}{l l}\n",
      "    \\frac{xy}{ 96}  0 <x<4, 1<y<5& \\quad \\\\\n",
      "    0 & \\quad \n",
      "  \\end{array} \\right.$</p>\n",
      "  \n",
      "  \n",
      " <p>$ E [x],  E [y], E [xy] y E [2x + 3y]$</p>\n",
      " \n",
      "<p>$ E [x]=  \\int\\limits_ {x=0}^4 \\int\\limits_ {y=1}^5 x f(x,y) dxdy \\int\\limits_ {x=0}^4 \\int\\limits_ {y=1}^5 x  \\frac{xy}{ 96} dxdy = \\frac{1}{ 96} \\int\\limits_ {y=1}^5 x(xy) dy = \\frac{1}{ 96} \\int\\limits_ {y=1}^5 x^2y dy =  \\left.\\frac{x^2y^2}{2}\\right|_1^5 = x^2 \\frac{24}{2}.\\frac{1}{96} = \\int\\limits_ {x=0}^4 x^2 \\frac{24}{192}= \\frac{24}{192} \\int\\limits_ {x=0}^4 x^2 \\frac{24}{192}. \\frac{x^3}{3} \\left.\\frac{}{}\\right|_0^4 = $  </p>\n",
      "\n",
      "<p>$\\frac{24}{192}. \\frac{64}{3} =\\frac{8}{3}  \\implies E [x]= \\frac{8}{3}$</p>\n",
      "\n",
      "<p>$E [y] = \\int\\limits_ {x=0}^4 \\int\\limits_ {y=1}^5 y(f(x,y))dxdy  = \\int\\limits_ {x=0}^4 \\int\\limits_ {y=1}^5 y\\frac{xy}{96} dxdy = \\frac{1}{ 96} \\int\\limits_ {y=1}^5 y(xy)dy = \\frac{1}{ 96} \\int\\limits_ {y=1}^5 xy^2 dy = \\frac{1}{ 96}x \\frac{y^3}{3} \\left.\\frac{}{}\\right|_1^5 = \\frac{1}{ 96} \\left(\\frac{125x}{3}- \\frac{1x}{3} \\right  ) = \\frac{1}{ 96} \\left(\\frac{124x}{3}\\right) = \\int\\limits_ {0}^4 \\frac{124x}{288}x$</p>\n",
      "\n",
      "\n",
      "<p>$\\frac{124x}{288} \\int\\limits_ {0}^4 xdx = \\frac{124x}{288} \\left(\\frac{x^2}{2}\\right) \\left.\\frac{}{}\\right|_0^4 $</p>\n",
      "\n",
      "<p>$\\frac{124x}{288} \\left(\\frac{2}{16}\\right)= \\frac{31}{9} \\implies E [y] = \\frac{31}{9}$</p>\n"
     ]
    },
    {
     "cell_type": "code",
     "collapsed": false,
     "input": [],
     "language": "python",
     "metadata": {},
     "outputs": []
    }
   ],
   "metadata": {}
  }
 ]
}



