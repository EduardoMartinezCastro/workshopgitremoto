#_Reflog_

Git realiza el seguimiento de las actualizaciones en el extremo de las ramas a través de un mecanismo denominado registros de referencias o "reflogs". 

El comando Reflog proporciona un registro de las actualizaciones de este mecanismo. Esta herramienta puede ser útil para identificar commits o versiones pasadas del repositorio.

### Comando

Algunas de las sintaxis posibles se describen a continuación:

```sh

$ git reflog [show] [<log-options>] [<ref>]
$ git reflog expire [--expire=<time>] [--expire-unreachable=<time>]
	[--rewrite] [--updateref] [--stale-fix]
	[--dry-run | -n] [--verbose] [--all [--single-worktree] | <refs>…​]
$ git reflog delete [--rewrite] [--updateref]
	[--dry-run | -n] [--verbose] <ref>@{<specifier>}…​
$ git reflog exists <ref>

```

### Más información

  Para más información visita [git reflog] (https://git-scm.com/docs/git-reflog)

