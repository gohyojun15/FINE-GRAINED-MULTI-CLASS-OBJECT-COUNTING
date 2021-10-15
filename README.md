# FINE-GRAINED-MULTI-CLASS-OBJECT-COUNTING
This repository contains KR-GRUIDAE dataset in FINE-GRAINED-MULTI-CLASS-OBJECT-COUNTING (ICIP 2021) [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9506384)

### KR-GRUIDAE Dataset
Images of KR-GRUIDAE dataset are captured by ecologists and labeled for five classes: Red-Crowned Crane(RCC), Red-Crowned Crane Juvenile(RCCJ), White-Naped Crane(WNC), White-Naped Crane juvenile(WNCJ) and Anser albifrons (AA).


### Downloads
Dataset is now available at : [[LINK]](https://drive.google.com/file/d/1vXEq55bVaUOn0ugF4xcUp7KtF0nLjkYg/view?usp=sharing)

### Format
1. img (folder): This folder contains images.
2. gt (folder): This folder contains annotation files (.mat)

we verfied the following code for loading annotation files:
```python
from scipy.io import loadmat

mat = loadmat(MAT_FILE_PATH)

mat["RCChead"] # contains the head points of RCC
mat["RCCbody"] # contains the body points of RCC

mat["RCCJhead"] # contains the head points of RCCJ
mat["RCCJbody"] # contains the body points of RCCJ

mat["WNChead"] # contains the head points of WNC
mat["WNCbody"] # contains the body points of WNC

mat["WNCJhead"] # contains the head points of WNCJ
mat["WNCJbody"] # contains the body points of WNCJ

mat["AAhead"] # contains the head points of AA
mat["AAbody"] # contains the body points of AA
```
