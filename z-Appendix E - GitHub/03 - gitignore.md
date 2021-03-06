#.gitignore#

The idea of this file is to exlude things that should not be in the repo, for example we shouldn't be storing the Umbraco core in the repo as NuGet will restore it for us if your project is setup to do so.

Below you will find a `.gitignore` file sample.  It should live at your repo root (but you can have multiple in sub-directories).  You should exlude temporary/runtime files and folders.  Git is also not meant to be a binary storage system so you should exclude `/media` and have a plan on how to back those up.  You can store binary data in Git but it should only be site files like logos.

```
.DS_Store
.AppleDouble
.LSOverride
Icon
._*
.Spotlight-V100
.Trashes
Thumbs.db
ehthumbs.db
Desktop.ini
$RECYCLE.BIN/

[Dd]ebug/
[Bb]uild/
[Rr]elease/
[Bb]in/
[Oo]bj/
src/[Pp]ackages/

node_modules

*.aps
*.bak
*.backup
*.build.csdef
*.cache
*.ilk
*.lib
*.log
*.meta
*.ncb
*.obj
*.orig
*.pch
*.pdb
*.pgc
*.pgd
*.rsp
*.sbr
*.scc
*.sdf
*.sln.docstates
*.suo
*.tlb
*.tlh
*.tli
*.tmp
*.user
*.vspscc
*.[Pp]ublish.xml
*_i.c
*_p.c
.builds
.svn
.hg
.hgignore

dummy.txt

src/*.Umbraco/App_Data/cache/
src/*.Umbraco/App_Data/ClientDependency/
src/*.Umbraco/App_Data/ExamineIndexes/
src/*.Umbraco/App_Data/Logs/
src/*.Umbraco/App_Data/TEMP/
src/*.Umbraco/App_Data/preview/
src/*.Umbraco/App_Data/umbraco.config
src/*.Umbraco/aspnet_client/
src/*.Umbraco/media/
src/*.Umbraco/imagecache/
src/*.Umbraco/install/
src/*.Umbraco/umbraco/
src/*.Umbraco/umbraco_client/

pkg/

*[Rr]e[Ss]harper.user
_ReSharper.*/

*.swp
*~

*.local.css

```
>Note that you will have to change this file to accomodate your specific project.  Make sure to exclude temporary/runtime data like the ~/App_Data/ folder.

[<Back 02 - Branching](02 - Branching.md)

[Next> 04 - Git Extensions](04 - Git Extensions.md)
