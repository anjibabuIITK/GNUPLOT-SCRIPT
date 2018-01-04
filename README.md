# GNUPLOT_script

**A command line sccript file for plotting in gnuplot.**
- This is sample script to plot by using gnuplot

# USAGE :  
    gnuplot plot_with_gnuplot.gnp

# Script:

```shell
#-------------------------EPS FORMAT --------------------#
#set encoding iso_8859_1
#set terminal postscript eps enhanced color font 'Helvetica,20' linewidth 2
#set output 'test.eps'
#------------------- PS FORMAT ----------------------------#
#set encoding iso_8859_1
#set terminal postscript enhanced color solid "Helvetica,20" linewidth 2
#set output "test.ps"
#------------------ PNG FORMAT ----------------------------#
set term png
set terminal postscript enhanced color solid "Helvetica,20" linewidth 2
set output "test.png"
#------------------ JPG FORMAT ----------------------------#
set terminal postscript enhanced color solid "Helvetica,20" linewidth 2
set output "test.jpg"
#
set grid
set xlabel " X lablel name "
set ylabel" Y label name"
set title " Title of the plot"
set border lw 2 # border width
set xrange [1:5] #To adjest xaxis RANGE from lower value to higher value
set yrange [0:10] # To adjest Y axis RANGE from lower to higher vslue
#----------------plotting-----------------------------------#
#plotting file.dat using coumn 1 and 2 with lines and keeping legend for graph.
# w l : with lines
# w lp : with line points
# w p : with points
# pt : point type
# ps : point size
# lw : line width
plot "file.dat" u 1:2 w l title"legend for graph" lw 2 ,"file.dat" u 1:3 w lp title "legend2" lw 2 pt 5 ps 2, "fiel2.dat" u 1:2 w p title"legend3" ps 2 pt 7
#replot
#===============================================================
# Useful stuff
# CONVERT PS to PDF on Linux by using this command
#
# ps2pdf test.ps test.pdf
#
# We can view ps file using gostview on linux terminal
#
# ghostview test.ps or
# gs test.ps
#
#==========================================================#
```


```
#--------------------------------------------------#
#         ANJI  BABU KAPAKAYALA                    #
#            IIT KANPUR, INDIA.                    #
#--------------------------------------------------#
```
