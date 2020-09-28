# Contributing notes to the Student Notes project
## Choosing a license
This template doesn't include any sort of license to leave the freedom of licensing to notes authors.
However, it is *strongly* recommended that you license your work.
You could pick one from the following list; these are tailored towards documentation and are therefore recommended.
- FreeBSD Documentation License
- GNU Free Documentation License (GFDL)
- GNU Simpler Free Documentation License (GSFDL)
- Any Creative Commons license

## Update the README
The README should include the course title along with the academic year and the language the notes have been written in.
You can also include a short description and a list of authors of the notes.

## Don't upload PDF(s) in the repository
Binary files don't belong in a Git repository.
This template includes automatic compilation of LaTeX files; the compiled output will be available in the 'Release' tab of the repository.

## Don't break CI
As said above, this template will automatically compile your LaTeX notes.
Try to not break the automated build system e.g.: by putting your main .tex file(s) in a subdirectory.
Compilation commands are visibile in .travis.yml

## Lint your documents
Before pushing, check that your document produces no warnings with linters such as **lacheck** or **chktex**.
When sending a pull request, a bot will try to compile your document and will check if your document produces any warnings; this is crucial to writing high quality notes and avoid weird rendering errors

## Optimise your images
Please try to keep image sizes small, using any sort of optimization (pngquant, imagemagick transforms, etc)

