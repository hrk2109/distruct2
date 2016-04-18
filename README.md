<h2>This project has been updated to version 2.2 and has moved back to the author's website: http://distruct2.popgen.org </h2>


# distruct2 - hosted here only for historical purposes
Implements user defined pop order and colors in 'distruct.py' from fastStructure (Raj et al 2014)

This is a modified version of the distruct.py script originally written by Anil Raj and available at www.github.com/rajanil/fastStructure.  It allows the end user to input the desired population order and color scheme for the output plot.  The color hack was implemented by Karl C. Fetter of University of Vermont.

Update: A new version (distruct2.1.py) allows using poporder from a user provided file.  An example of poporder file is provided.  

An example using the test data from fastStructure is provided and includes the following files:
```bash
distruct2.1.py (modified python script)
TestK3.png (output file)
pop (popfile)
poporder (pop order file)
run2.1.sh (execute distruct2)
testoutput_simple.3.log (fastStructure output log)
testoutput_simple.3.meanP (fastStructure K=3 allele frequencies)
testoutput_simple.3.meanQ (fastStructure K=3 ancestry coefficients)
```

<h3> To Download </h3>
```bash
mkdir ~/projects
cd ~/projects
git clone https://github.com/cryptic0/distruct2
```

Then take a look at ```run2.1.sh```.  With this version of distruct, there is no need to make any changes to the python script.  Simply add your pop names in the desired order, one on each line in the supplied 'poporder' file and run distruct2.1.py.  You can also run it using the provided shell script run2.1.sh.   Run the test data by executing ```./run2.1.sh``` and make sure everything works correctly before attempting with your own data.

The downside of using distruct2.1.py is that you MUST provide it with a poporder file.  If you don't it will complain and exit.  If you don't care for population order, use original distruct from Anil Raj's repository.

Contact Vikram Chhatre (vchhatre at uvm dot edu) with any questions.
