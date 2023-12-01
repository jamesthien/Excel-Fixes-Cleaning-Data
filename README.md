# Excel-Fixes-Cleaning-Data

## Clean Date time if dd/mm/yyyy vs dd-mm-yyyy
=IF(ISNUMBER(J2),TEXT(J2,"dd-mm-yyyy"),IF(ISNUMBER(DATEVALUE(J2)),TEXT(DATEVALUE(J2),"dd-mm-yyyy"),SUBSTITUTE(J2,"/","-")))
