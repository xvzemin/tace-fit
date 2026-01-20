# TACE Tutorial

This repository is mainly used to store **TACE** tutorial files, and it can also be used to reproduce the results from TACE papers.  
Since some parameters might differ slightly, the results may vary a little, but the overall trends should remain similar.

For each combination of **target property** and **embedding property**, we will gradually update example files.  
The training procedure is the same for all cases: after installing TACE, simply enter the directory of the property you want to predict.


> **Note:** All necessary scripts and input files are already included in the [TACE example folder](https://github.com/xvzemin/tace/tree/main/example).  
> The `tace-fit` repository is only provided as an additional example to show how to train other properties.

---

## 1. Install TACE

If TACE is already installed, you can skip this step.

```bash
git clone https://github.com/xvzemin/tace.git
cd tace
pip install .
```
## 2. Start training

```bash
git clone https://github.com/xvzemin/tace-fit.git
cd property_your_want_to_predict
tace-train -cn tace.yaml
```