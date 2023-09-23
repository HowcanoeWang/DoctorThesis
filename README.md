# DoctorThesis

Here is the LaTeX source code of my PhD thesis. You can access the final pdf at the attachment of [Releases](https://github.com/HowcanoeWang/DoctorThesis/releases/tag/v230923)

# Compile

You can import the full projects to Overleaf using the following settings

![image](https://github.com/HowcanoeWang/DoctorThesis/assets/19968935/aab30e17-2e91-4ac3-b9b7-2c602c3d480f)

---

Or you can set the Vscode local compiler and LaTex workshop plugin, and use the configs in the `.vscode/` folder (`ctrl` + `alt` + `B`) shortcut to compile

Please ensure to use the following build command:

![image](https://github.com/HowcanoeWang/DoctorThesis/assets/19968935/175420e4-230c-49dd-897b-b1b8470a9ab3)

# Reference management

The BibTex reference `styles/bibtex.bib` is produced by Zotero and [Better BibTex](https://retorque.re/zotero-better-bibtex/) zotero plugin

# Editing track

The editing tracking is made by `changes` latex package, by manually editing the latex source code `\added{...}`, `\replace{new}{old}`, `\deleted{...}` to produce changing trace marks. After finishing all editing, using the `pyBatchMerge.ipynb` to accept all changes.

> Please note, the tool only can remove the `\added{}`, `\replace`, and `\deleted{}` in **one** line. Please search and edit manually others in multiple lines before compiling.
>
> e.g. The following is in one line, it works
> ```latex
> \added{The purple monkey danced on top of the flying toaster while juggling three rubber ducks and reciting the alphabet backwards}.
> ```
>
> But this is not in one line, does not work
> ```latex
> \added{
>    The purple monkey danced on top of the flying toaster while
>    juggling three rubber ducks and reciting the alphabet backwards
> }.
> ```
