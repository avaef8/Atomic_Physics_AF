# Atomic_Physics_AF
Currently this holds my US '26 CMSE201 final project in its edited form. I suggest that the file is personally downloaded because the intention of the code is for it to work using a desired, user inputted, element from 01H to 92U. The code and markdown boxes are not in their formal form but is enough to extrapolate a lot of meaning from the NIST dataset.

You can download the dataset in order to use the code here: https://www.nist.gov/pml/atomic-reference-data-electronic-structure-calculations

*Research Question: How does Shielding Constant change throughout electrons in an atom?*

i.e. How attracted are electrons to the nucleus as they get further out? How does the shielding effect look for each orbital in the elements?


The raw file shows a test run for Radium and a user input for Protactinium. You can see the differences in f-orbital behavior which have different mechanisms than the differences between, for example, Lanthanum and Lead. Download this file, along with the dataset from NIST, to utilize the user input and you can see the data for any element from Hydrogen to Uranium!

Results show that f-orbitals exhibit a higher shielding effect than the patterns in the rest of the atom would predict. Slater's rules of orbital shielding are followed here (increased shielding effects in the order of s<p<d<f). An increase and then a decrease in shielding constant occurs at the f-orbital in some atoms with 58+ protons (Lanthanum not incuded because a d-orbital fills before the f-orbital). This results from the drop in energy seen in the eigenvalues in the dataset used (from NIST). An atom like Radium almost barely produces this f-orbital property, but Lead, Protactinium, and Uranium show the increase in shielding constant in their outer f-orbitals. Further analysis is needed to truly understand the impacts of f-orbitals for elements in and after the Lactinide series, but it is clear that the electrons residing in these outer f-orbitals are often "hanging on like a thread". The Aufbauprinzip ("building-up principle") and Hund's filling rules should be taken into consideration, along with the LDA approximation method. 

The only other approximation method compatible with this code is ScRLDA, which can be called in the path file name when creating the dictionary. LSD and RLDA approximations are not compatible with the code due to orbital naming. LSD method treats spin down and spin up electrons differently, which would require a new layout of code to model its data.
