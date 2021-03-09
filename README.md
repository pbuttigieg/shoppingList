# p_template
A template repository with some recommended elements for projects. 

## About this project
The top-level README.Md should be a narrative piece describing what this repository is for and how to use it (e.g. is the code for HPC systems like Ollie? What would someone need to re-run the code in the repo?). 

The prose in this section should complement and cross-reference, but not reproduce, the content in "project_information.Md". 


## Directories 

Here, add brief notes about what's in each directory of this repo, but *each directory should have it's own README.Md*  with more detail. The description in this top-level README is just for orientation.

Keep the directories to a minimum both in number and depth (if you have a directory tree with >3 levels, that's usually an indication of poor practice). Make sure you only create a directory if it makes sense for your *code* organisation, not the conceptual organisation of the project (they don't always overlap).

Try not to think in ways usually associated with storing normal files in directories. In a repo, each directory should contain code that lets you and those after you perform a clearly defined and largely self-contained group of tasks. Directories can be "sequenced" in the sense that you need to run the code in one directory in order to create the input files for another one. These details should be clearly described in the README.Md files in each directory and subdirectory, as well as in the execution_flow.Md.

How things are grouped really depends on your project, but it should be as modular as possible. For example, if your project requires you to import, assemble, annotate, and analyse several metagenomes, consider having one directory that bundles all the code needed to process one metagenome. Then have another directory or set of directories for generic, cross-cutting work (e.g. comparing metagenomes). This way, if you have to add or remove metagenomes later, you don't have to dig through a massive chunk of code to extract/add lines. You can also modularise based on the function (one directory for import, one for assembly, etc) if (and only if) you're careful and have wrtten good and easily changeable and maintainable iterators or vector-based scripts (e.g. one loop for all contents, NOT one block of code for each data set). 


## Code cross-references

In this section, note if this repo depends on or works with code in any other repos, and how they work together (e.g. link to another .Md document explaining this).


## Issues

This section can be removed after you've read and understood it. 

Use issues to log how you approached every coding challenge you face during your project. Treat each issue as a fine grained subject-specific log book of how you addressed the challenge. Keep these at a medium granularity: that is, "assemble metagenomes" is too broad, "download files" is (usually) too narrow. 

Of course, if you bump into a tough problem at any granularity (even very small), open an issue to log what you've done to overcome it. 

**Make sure you backup all your issues along with your repository, in your AWI project backup location.**

This API call should get them all for you: 

```
https://api.github.com/repos/<repo-owner>/<repo-name>/issues?state=allwill
```

The parameters for that call are documented [here](https://docs.github.com/en/rest/reference/issues)

However, right now the GH API seems to be having its own issues - we'll update this README when we have a solution

