# LobsterPy

This is a package that enables automatic plotting of Lobster outputs. You can download Lobster on [https://www.cohp.de](https://www.cohp.de). Currently, only VASP/Lobster computations are supported.

## Installation


You can pip install the package by writing ``pip install -e .`` in the main package. It will then use setup.py to install the package. One requirement of this package is [pymatgen](https://github.com/materialsproject/pymatgen).

## Basic usage

* **Automatic analysis and plotting of COHPs:**
    
    You can use ``lobsterpy --description`` for an automated analysis of COHPs for relevant cation-anion bondsor ``lobsterpy --automaticplot`` to plot the results automatically. It will evaluate all COHPs with ICOHP values down to 10% of the strongest ICOHP. You can enforce an analysis of all bonds by using ``lobsterpy --automaticplot --all`` 
  
    It is also possible to start this automatic analysis from Python script. See "examples" for scripts.

  
* **Command line plotter**:
    
    We included options to plot COHPs/COBIs/COOPs from the command line.
    ``lobsterpy --plot 1 2`` will plot COHPs of the first and second bond from ``COHPCAR.lobster``. It is possible to sum or integrate the COHPs as well (``--summed``, ``--integrated``). You can switch to COBIs or COOPs by using ``--cobis`` or ``--coops``, respectively.


* **Further help?**
  
    You can get further information by using ``lobsterpy --help``


## License
Lobsterpy is released under a BSD 3-Clause "New" or "Revised" License. 


## How to cite?
A citation for lobsterpy will follow at a later stage. For now, please cite [pymatgen](https://github.com/materialsproject/pymatgen) and [Lobster](https://www.cohp.de) correctly .

