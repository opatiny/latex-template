# LaTex in VS Code

**Summary:** Procedure on how to install latex to work locally on a computer.

If you want to have some LaTex projects locally on a computer and be able to have color highlighting, completion, etc, you have to install some software. There is a VS Code extension which acts as an editor, but you still have to install a latex distribution, all the packages, and a tool to build your .tex file.

## Installing Tex Live

The latex distribution that we will use is Tex Live.
Is there a distrib installed by default on fedora?

Link to official documentation: https://www.tug.org/texlive/acquire.html

In the official documentation, they say that you should install the software by downloading a compressed folder. This is what I did (it was a really bad idea), but apparently you can also just do:

```bash
sudo dnf install texlive-scheme-full
```

This should provide you with all the packages you need.

## Installing individual LaTex packages

You can install individual packages by using:

```bash
sudo dnf install 'tex(hyperref.sty)'
```

## Installing LaTex Workshop vscode extension

Open VS Code, go to the extensions panel and install the "LaTex workshop" extension.

## Installing `latexmk`

This is the tool that allows you to build your tex file. It is called a "latex recipe". 

```bash
sudo dnf install latexmk
```
