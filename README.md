# share_activity_2

Jahir Roberto Rivas Vazquez A01204988
Gerardo Melesio Sancen A01203843
Alec Garcia Barba A01022495

This directory contains data from power consumption of the first floor of certain building

"this_week.csv" and "las_week.csv" contain power consumption sampled every 5 minutes
throughout almost a week, this data was colected using hall effect sensors that read current
which was then indirectlly a meassure of power consumption rendering nominal voltages for
tested and monitored equipment.

File "egade.csv" contains data of a different building for different dates following the same
data acquisition system.

File "semanai_prepdata.ipynb" is a jupyter notebook that uses sklearn to train a neural
network that searches to predict power consumpiton given as inputs the day of the week as
a number, year, month, hour and minute.

Data is filtered using digital filter known as moving average with configurable window span.

To use the different files one may just comment different lines in the section that says
"Santafe" or "CEDETEC" and simply comment the oposite, the prediction is rendered using
the same data as the whole file used to test and train.


" predictorr.joblib " is pretrained job used for the prediction in the former file.



