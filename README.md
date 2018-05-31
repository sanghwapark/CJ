# CTEQ-JLab PDF and Structure Function sets

The CJ PDFs and structure functions can be obtained by downloading the `CJgrids` program and the desired error grids (described below). Two example programs are also provided.

The CJ15 PDFs are also included in the [LHAPDF distribution](https://lhapdf.hepforge.org/).



## Programs

### Fortran
Check the headers of `CJgrids.f` for details.

Example programs `tst_CJpdf.f` and `tst_CJsfn.f` illustrate the usage of CJgrids to obtain PDFs and Structure Funtions, respectively.

### Python

CJgrids.f is ready to be ported to Python by using [f2py](https://docs.scipy.org/doc/numpy/f2py/). One simply needs to issue
`f2py -c -m CJgrids CJgrids.f` in a terminal, and then `import cjgrids` into one's Python code. An example Python program will be added soon.



## PDF and structure function grids

Grids are available in the GRIDS/ folder, as one zipped subfolder for each desired set. Subfolder names start with `tbl_` followed by the name of the set a

**Note:**
* Grids are available in the range 10-6 ≤ x ≤ 1 and 1.3 ≤ Q ≤ 105 GeV. However, the region where the PDFs are directly constrained by data is 2 x 10-5 < x < 0.9 and 1.3 < Q < 550 GeV. 

### CJ15 global fit

The latest global fit is **CJ15**, see the [original paper](http://inspirehep.net/record/1420566?ln=en) for details. Available grids are
* CJ15nlo: next-to-leading order (NLO)
* CJ15lo: leading order (LO)

CJ15 NLO structure functions are also avaiable (F2 neutral current only for now) as:
* CJ15nlo-F2NC

### CJ12 global fit

The PDF grids from the earlier **CJ12** NLO analysis are also available, although these have been superceded by the CJ15 PDFs. [See the original reference](http://inspirehep.net/record/1206325?ln=en) for details. Available grids are:
* CJ12min
* CJ12mid
* CJ12max 


## Citations

When using the CJ15 PDFs or structure functions, please reference: 
* A. Accardi, L. T. Brady, W. Melnitchouk, J. F. Owens and N. Sato, arXiv:1602.03154, Phys.Rev. D93 (2016) 114017 [(Inspire link)](http://inspirehep.net/record/1420566?ln=en)



## Bugs and other issues

To report bugs and technical issues, please use the [CJ github issue tracker](https://github.com/JeffersonLab/CJ/issues). We will take care of these as soon as we can.

For any other question, please contact Alberto Accardi at "accardi_at_jlab.org". 



