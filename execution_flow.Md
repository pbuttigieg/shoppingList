# Execution flow

This is perhaps the most important file in the repo. 

@Managers: if the quality of this file is not sufficient for you or a third-party to reproduce the results in the repo, do not sign the end-of-employment release forms until it is. You will also be accountable for the scientific integrity of this repository.

This file should detail the steps needed to exactly reproduce the results you obtained by running your code, across all relevant subdirectories. 

If this project has two or more independent execution flows, then duplicate this file and document what each one is for. 

It should walk the user through the entire flow from acquiring and validating the (meta)data, installing/calling on all needed software (with versions), cleaning/prepping it for analysis, running analyses and diagnostics, and generating both intermediate and final results. 

You can substitute this .Md file with a Jupyter notebook or similar filetype if that's your chosen mode of storing the execution flow. If you're an advanced user, consider encoding your workflows in [CWL](https://www.commonwl.org/) or building a Makefile.

The text in this file should make frequent and meaningful cross-references to the documentations files in all of your subdirectories and should also be intelligible and helpful up to 10 years after the project is done. 

This file is *not* a collection of rough notes or something to do last minute: this is a core part of your professional obligation to your employer and the public to ensure reproducibility. 

