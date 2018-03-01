�Qu� comando utilizaste en el paso 11? �Por qu�?

git reset -- hard HEAD~1

Deshace tanto el stage como el working, borrando como piden el working area.


�Qu� comando o comandos utilizaste en el paso 12? �Por qu�? 

git reset HEAD~1
Deshace el anterior paso, rehaciendo el comit


El merge del paso 13, �Caus� alg�n con?icto? �Por qu�? 

git checkout a18f033b

Note: checking out 'a18f03b'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:

git checkout -b <new-branch-name>

HEAD is now at a18f03b paso 10 a�adido al quijote

No causa ningun conflicto ya que nos estamos moviendo en la misma rama.


El merge del paso 19, �Caus� alg�n con?icto? �Por qu�? 
causa esto: 

C:\Users\pepel\Desktop\PracticaGit>git merge htmlify
Auto-merging don-quijote.md
CONFLICT (content): Merge conflict in don-quijote.md
Automatic merge failed; fix conflicts and then commit the result.
Por que estan en distintas ramas a la misma altura.

El merge del paso 21, �Caus� alg�n con?icto? �Por qu�?

No, por que esta en distinta rama y a distintas alturas 

C:\Users\pepel\Desktop\PracticaGit>git merge styled
Updating 76bc088..691b881
Fast-forward
 don-quijote.md | 19 ++++++++++++++++++-
 1 file changed, 18 insertions(+), 1 deletion(-)


�Qu� comando o comandos utilizaste en el paso 25?
git log --graph

C:\Users\pepel\Desktop\PracticaGit>git log --graph
*   commit 691b881baaac1be35848166fdf47b2d5f62dbf04 (HEAD -> master, styled)
|\  Merge: a18f03b a422bf5
| | Author: joseluis gonzalez <pepe.lu@hotmail.com>
| | Date:   Wed Feb 28 17:24:43 2018 +0100
| |
| |      resolver error >>>>>> htmlify punto 19
| |
| * commit a422bf5e31853828f8e2bc57c2282c6a13dd8ae2 (htmlify)
| | Author: joseluis gonzalez <pepe.lu@hotmail.com>
| | Date:   Wed Feb 28 17:10:31 2018 +0100
| |
| |     paso 18 anado mas info
| |
* | commit a18f03b3aaeb0c93b9edcf9d05ee133b4ce8b058
|/  Author: joseluis gonzalez <pepe.lu@hotmail.com>
|   Date:   Wed Feb 28 16:55:48 2018 +0100
|
|       paso 10 a<C3><B1>adido al quijote
|
* commit 76bc088ad8d0c9c31682ee9390a324f5bebfb8c9
  Author: joseluis gonzalez <pepe.lu@hotmail.com>
  Date:   Wed Feb 28 16:50:45 2018 +0100

      paso 3, creamos md don-quijote

El merge del paso 26, �Podr�a ser fast forward? �Por qu�? 

C:\Users\pepel\Desktop\PracticaGit>git merge --no-ff title
Merge made by the 'recursive' strategy.
 don-quijote.md | 2 ++
 1 file changed, 2 insertions(+)



�Qu� comando o comandos utilizaste en el paso 27? 

C:\Users\pepel\Desktop\PracticaGit> git reset HEAD~1
Unstaged changes after reset:
M       don-quijote.md


�Qu� comando o comandos utilizaste en el paso 28? 

C:\Users\pepel\Desktop\PracticaGit> git reset --hard HEAD~1
HEAD is now at a18f03b paso 10 a�adido al quijote


�Qu� comando o comandos utilizaste en el paso 29? 

C:\Users\pepel\Desktop\PracticaGit>git branch -D title
Deleted branch title (was 4115d80).

�Qu� comando o comandos utilizaste en el paso 30? 

C:\Users\pepel\Desktop\PracticaGit>git reset --hard b6d3836
HEAD is now at b6d3836 Merge branch 'title'


�Qu� comando o comandos usaste en el paso 32? 

C:\Users\pepel\Desktop\PracticaGit>git checkout 76bc088
Note: checking out '76bc088'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:

  git checkout -b <new-branch-name>

HEAD is now at 76bc088 paso 3, creamos md don-quijote

C:\Users\pepel\Desktop\PracticaGit>


�Qu� comando o comandos usaste en el punto 33? 

C:\Users\pepel\Desktop\PracticaGit>git reset 4115d80
Unstaged changes after reset:
M       don-quijote.md