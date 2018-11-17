# Errores y soluciones
Aquí vamos a recopilar los errores que nos vayamos encontrando y sus soluciones:

## Error 1: Falta sincronizar origin/master
Error producido al intentar subir cambios a mi repositorio remoto (origin/master):
~~~~git
$ git push
To https://github.com/ArtesanoMultimedia/Machine-Learning.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/ArtesanoMultimedia/Machine-Learning.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
~~~~

**Problema:**
Mi repositorio local estaba sincronizado con upstream/master, pero no con origin/master.

**Solución:**
~~~~git
$ git fetch origin
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/ArtesanoMultimedia/Machine-Learning
   21fe954..80f14f3  master     -> origin/master

$ git merge origin/master
Already up to date!
Merge made by the 'recursive' strategy.
~~~~

En este caso, el `merge`ha sido automático. Podía no haber sido posible y entonces tendría que haberlo hecho a mano.

**Comprobación:**
~~~~git
$ git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 6 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 28.54 KiB | 9.51 MiB/s, done.
Total 8 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/ArtesanoMultimedia/Machine-Learning.git
   80f14f3..01872f9  master -> master
~~~~