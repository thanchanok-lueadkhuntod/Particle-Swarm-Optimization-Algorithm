# Particle Swarm Optimization (PSO)

A straightforward implementation of the Particle Swarm Optimization (PSO) algorithm from scratch using NumPy. I built this to test how well the algorithm optimizes standard benchmark functions.

## Features
* Custom PSO loop written in pure Python + NumPy.
* Tests 4 standard optimization functions: Sphere, Rosenbrock, Rastrigin, and Griewank.
* Includes Matplotlib visualizations for agent tracking (2D contours) and convergence plots.
* Easy to tweak parameters (c1, c2, population size, max iterations).

## Requirements
* Python 3.x
* NumPy
* Matplotlib

## How to Run
Just clone the repo and run the script. It will run a 10-run summary and pop up the plots automatically.

```bash
python pso_algorithm.py
```


## Results & Visualizations
Here is what the outputs look like:
### 1. 10 Runs Summary (All 4 Functions)
Running the algorithm 10 times per function to check stability, mean, standard deviation, and the minimum values found.

```text
Sphere results (10 runs):
run 1: 145.34011671824865
run 2: 137.21847576294417
run 3: 173.50502619532534
run 4: 111.64035587632287
run 5: 150.9642583303414
run 6: 158.57757767245624
run 7: 162.94368243064667
run 8: 148.08239331887978
run 9: 153.45621808192863
run 10: 141.6675547170663
mean = 148.339565910416
std.dev = 16.69516185748317
best of 10 = 111.64035587632287

Rosenbrock results (10 runs):
run 1: 0.0032840292169140947
run 2: 0.006115537236109806
run 3: 7.991159342586807e-05
run 4: 0.009442149046570364
run 5: 0.004422836199944898
run 6: 0.004097783836500617
run 7: 0.012733075243002503
run 8: 0.00048477187319691457
run 9: 0.0020426028238094245
run 10 : 0.0032180537221469614
mean = 0.004592075079162145
std.dev = 0.003940125352310468
best of 10 = 7.991159342586807e-05

Rastrigin results (10 runs):
run 1: 246.1402431216123
run 2: 233.4981349530612
run 3: 246.19991552886106
run 4: 210.13434008023415
run 5: 210.1421835645274
run 6: 197.5900325844256
run 7: 217.54361992767213
run 8: 236.46538771264295
run 9: 220.0881826420378
run 10: 254.24283254187154
mean = 227.20448726569458
std.dev = 18.795205494201614
best of 10 = 197.5900325844256

Griewank results (10 runs):
run 1: 510.82174146591683
run 2: 501.08273123667453
run 3: 424.5868181295957
run 4: 580.930553056025
run 5 : 494.9230561870855
run 6: 588.6436167859653
run 7: 498.5244390571483
run 8: 565.5329141571381
run 9: 407.0634352954704
run 10: 559.2078448027286
mean = 513.1317150173749
std.dev = 62.31973616292207
best of 10 = 407.0634352954704
```

### 2. 2D Contour Maps
The landscape of the 4 benchmark functions (Sphere, Rosenbrock, Rastrigin, and Griewank).
![Convergence Plot](Sphere.png)
![Convergence Plot](Rosenbrock.png)
![Convergence Plot](Rastrigin.png)
![Convergence Plot](Griewank.png)

### 3. Agent Tracking (Rosenbrock, 50 particles)
Shows how 50 particles move and swarm toward the minimum over the first 20 iterations.
![Convergence Plot](RosenbrockAgentsI1.png)
![Convergence Plot](RosenbrockAgentsI2.png)
![Convergence Plot](RosenbrockAgentsI3.png)
![Convergence Plot](RosenbrockAgentsI4.png)
![Convergence Plot](RosenbrockAgentsI5.png)
![Convergence Plot](RosenbrockAgentsI6.png)
![Convergence Plot](RosenbrockAgentsI7.png)
![Convergence Plot](RosenbrockAgentsI8.png)
![Convergence Plot](RosenbrockAgentsI9.png)
![Convergence Plot](RosenbrockAgentsI10.png)
![Convergence Plot](RosenbrockAgentsI11.png)
![Convergence Plot](RosenbrockAgentsI12.png)
![Convergence Plot](RosenbrockAgentsI13.png)
![Convergence Plot](RosenbrockAgentsI14.png)
![Convergence Plot](RosenbrockAgentsI15.png)
![Convergence Plot](RosenbrockAgentsI16.png)
![Convergence Plot](RosenbrockAgentsI17.png)
![Convergence Plot](RosenbrockAgentsI18.png)
![Convergence Plot](RosenbrockAgentsI19.png)
![Convergence Plot](RosenbrockAgentsI20.png)

### 4. Convergence Graph (Rosenbrock)
Tracks the global best value dropping and stabilizing. Iterations 1-4 are skipped to zoom in on the actual convergence curve (iterations 5..100).
![Convergence Plot](RosenbrockConvergesI5..100.png)

## Benchmark Setup
* Population (n): 50
* Max Iterations (kmax): 100
* c1, c2: 2.0
