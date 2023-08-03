`pyEIT` is a python-based, open-source framework for Electrical Impedance Tomography (EIT). The design priciples of `pyEIT` are **modularity, minimalism, extensibility and OOP.**

## Install Requirements

All requirements are provided inside the `requirements.txt`.

    pip3 install -r requirements.txt # Linux, macOS, Windows
    pip install -r requirements.txt  # Windows
## 2. Run the examples

From the example folder, pick one demo and run!

**Note:** the following images may be outdated due to that the parameters of a EIT algorithm may be changed in different versions of `pyEIT`. And it is there in the code, so just run the demo.

### 2.1 (2D) forward and inverse computing

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/one_obj_cent.ipynb`

# ![1obj_center](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/1obj_center.png)

REMARK:

Three different image reconstruction methods are shown
The number of electrodes in each row is equal
The image reconstruction method in each colomn is same

Result:

Jacobian is the slowest and Backprojection is the fastest method
GREIT is the trade off between Jacobian and Backprojection for time and resolution

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/one_obj_side.ipynb`

# ![1obj_side](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/1obj_side.png)

REMARK:

Three different image reconstruction methods are shown
The number of electrodes in each row is equal
The image reconstruction method in each colomn is same

Result:

Jacobian is the slowest and Backprojection is the fastest method
GREIT is the trade off between Jacobian and Backprojection for time and resolution

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/two_obj_sides.py`

# ![2obj_sides](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/2obj_sides.png)
REMARK:

Three different image reconstruction methods are shown
The number of electrodes in each row is equal
The image reconstruction method in each colomn is same

Result:

Jacobian is the slowest and Backprojection is the fastest method
GREIT is the trade off between Jacobian and Backprojection for time and resolution
All three methods are good with goal of the detection of the number of the separated objects

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/twoD_obj_sides.py`

# ![2Dobj_sides](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/2Dobj_sides.png)

REMARK:

Three different image reconstruction methods are shown
The number of electrodes in each row is equal
The image reconstruction method in each colomn is same
The target is trying to detect two objects with same conductivity but different size

Result:

Jacobian is the slowest and Backprojection is the fastest method
GREIT is the trade off between Jacobian and Backprojection for time and resolution

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/adjandopp.py`

# ![adjandoppr](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/adjandoppr.png)

REMARK:

Three different image reconstruction methods are shown
The number of electrodes in any case is equal
The image reconstruction method in each colomn is same
The target is trying to compare adjacent with opposite injection pattern

Result:

Opposite injection pattern showes separated objects clearer
GREIT is the best and Backprojection is the worst

#-----------------------------------------------------------------------------------#

**Using** `codes/examples/geometry.py`

# ![triangelandcircle](https://github.com/Oveys96/eit_seminar/blob/main/codes/images/triangelandcircle.png)

REMARK:

Three different image reconstruction methods are shown
The number of electrodes in any case is equal
The image reconstruction method in each colomn is same
The target is trying to detect the object like triangle with sharp edges with adjacent and opposite injection pattern

Result:

GREIT almost fails even in separating the objects
Jacobian has the highest resolution
Adjacent injection pattern causes better results for objects with sharp edges
Simulating the edges is difficult task and almost all these methods fail in it. We should use other tools for post processing the image






## Contact

Email: oveys.javanmardtilaki@uni-rostock.de
