# University-Ruby
Administrator@PC-27 MINGW64 ~
$ HELLO
bash: HELLO: command not found

Administrator@PC-27 MINGW64 ~
$  mkdir
mkdir: missing operand
Try 'mkdir --help' for more information.

Administrator@PC-27 MINGW64 ~
$ mkdir hello

Administrator@PC-27 MINGW64 ~
$ cd hello

Administrator@PC-27 MINGW64 ~/hello
$ cd hello/
bash: cd: hello/: No such file or directory

Administrator@PC-27 MINGW64 ~/hello
$ git init
Initialized empty Git repository in C:/Users/Administrator/hello/.git/

Administrator@PC-27 MINGW64 ~/hello (master)
$  ls - al
ls: cannot access '-': No such file or directory
ls: cannot access 'al': No such file or directory

Administrator@PC-27 MINGW64 ~/hello (master)
$ ls -al
total 16
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:23 ./
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:22 ../
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:23 .git/

Administrator@PC-27 MINGW64 ~/hello (master)
$ touch index.com

Administrator@PC-27 MINGW64 ~/hello (master)
$ ls -al
total 16
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:27 ./
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:22 ../
drwxr-xr-x 1 Administrator 197121 0 二月 24 10:23 .git/
-rwxr-xr-x 1 Administrator 197121 0 二月 24 10:27 index.com*

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)


Administrator@PC-27 MINGW64 ~/hello (master)
$ git config -list
error: did you mean `--list` (with two dashes ?)

Administrator@PC-27 MINGW64 ~/hello (master)
$ git conhig --list
git: 'conhig' is not a git command. See 'git --help'.

Did you mean this?
        config

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global user.name "Nini"

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --glbal user.email "cowe501@gmail.com"
error: unknown option `glbal'
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)


Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        index.com

nothing added to commit but untracked files present (use "git add" to track)

Administrator@PC-27 MINGW64 ~/hello (master)
$ git add index.com

Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   index.com


Administrator@PC-27 MINGW64 ~/hello (master)
$ git add hi.html
fatal: pathspec 'hi.html' did not match any files

Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   index.com


Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit -m 'index.html'

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Administrator@PC-27.(none)')

Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   index.com


Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit -m'Hello!NTUB!!'

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Administrator@PC-27.(none)')

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --'NINI'
error: unknown option `NINI'
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)


Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global name'Nini '
error: key does not contain a section: nameNini

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global user.name'Nini '
error: invalid key: user.nameNini

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global user.name'Nini'

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global user.email'cowe501@gmail.com'

Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   index.com


Administrator@PC-27 MINGW64 ~/hello (master)
$ git log
fatal: your current branch 'master' does not have any commits yet

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.diff=auto
color.status=auto
color.branch=auto
color.interactive=true
help.format=html
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
diff.astextplain.textconv=astextplain
rebase.autosquash=true
credential.helper=manager
user.name=Nini
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --global user.email 'cowe501@gmail.com'

Administrator@PC-27 MINGW64 ~/hello (master)
$ git congig --list
git: 'congig' is not a git command. See 'git --help'.

Did you mean this?
        config

Administrator@PC-27 MINGW64 ~/hello (master)
$ git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.diff=auto
color.status=auto
color.branch=auto
color.interactive=true
help.format=html
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
diff.astextplain.textconv=astextplain
rebase.autosquash=true
credential.helper=manager
user.name=Nini
user.email=cowe501@gmail.com
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true

Administrator@PC-27 MINGW64 ~/hello (master)
$ git log
fatal: your current branch 'master' does not have any commits yet

Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit -m'HELLO~~~~'
[master (root-commit) 215f8f9] HELLO~~~~
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.com

Administrator@PC-27 MINGW64 ~/hello (master)
$ git log
commit 215f8f98f978d5f4f6c6a9e99123d14155d57d85
Author: Nini <cowe501@gmail.com>
Date:   Fri Feb 24 11:07:18 2017 +0800

    HELLO~~~~

Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit --m 'NTUB'
On branch master
nothing to commit, working tree clean

Administrator@PC-27 MINGW64 ~/hello (master)
$ git log
commit 215f8f98f978d5f4f6c6a9e99123d14155d57d85
Author: Nini <cowe501@gmail.com>
Date:   Fri Feb 24 11:07:18 2017 +0800

    HELLO~~~~

Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit --'NTUB'
error: unknown option `NTUB'
usage: git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup <commit>      use autosquash formatted message to fixup specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C/-c/--amend)
    -s, --signoff         add Signed-off-by:
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <default>   how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)


Administrator@PC-27 MINGW64 ~/hello (master)
$ git blame

usage: git blame [<options>] [<rev-opts>] [<rev>] [--] <file>
    <rev-opts> are documented in git-rev-list(1)

    --incremental         Show blame entries as we find them, incrementally
    -b                    Show blank SHA-1 for boundary commits (Default: off)
    --root                Do not treat root commits as boundaries (Default: off)
    --show-stats          Show work cost statistics
    --progress            Force progress reporting
    --score-debug         Show output score for blame entries
    -f, --show-name       Show original filename (Default: auto)
    -n, --show-number     Show original linenumber (Default: off)
    -p, --porcelain       Show in a format designed for machine consumption
    --line-porcelain      Show porcelain format with per-line commit information
    -c                    Use the same output mode as git-annotate (Default: off)
    -t                    Show raw timestamp (Default: off)
    -l                    Show long commit SHA1 (Default: off)
    -s                    Suppress author name and timestamp (Default: off)
    -e, --show-email      Show author email instead of name (Default: off)
    -w                    Ignore whitespace differences
    --indent-heuristic    Use an experimental indent-based heuristic to improve diffs
    --compaction-heuristic
                          Use an experimental blank-line-based heuristic to improve diffs
    --minimal             Spend extra cycles to find better match
    -S <file>             Use revisions from <file> instead of calling git-rev-list
    --contents <file>     Use <file>'s contents as the final image
    -C[<score>]           Find line copies within and across files
    -M[<score>]           Find line movements within and across files
    -L <n,m>              Process only line range n,m, counting from 1
    --abbrev[=<n>]        use <n> digits to display SHA-1s


Administrator@PC-27 MINGW64 ~/hello (master)
$ git blame index.html
fatal: cannot stat path 'index.html': No such file or directory

Administrator@PC-27 MINGW64 ~/hello (master)
$ git blame 'index.html'
fatal: cannot stat path 'index.html': No such file or directory

Administrator@PC-27 MINGW64 ~/hello (master)
$ git remote add origin https://github.com/ChristenHer/University-Ruby.git

Administrator@PC-27 MINGW64 ~/hello (master)
$ git push -u origin master
Counting objects: 3, done.
Writing objects: 100% (3/3), 211 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
Branch master set up to track remote branch master from origin.
To https://github.com/ChristenHer/University-Ruby.git
 * [new branch]      master -> master

Administrator@PC-27 MINGW64 ~/hello (master)
$ git init
Reinitialized existing Git repository in C:/Users/Administrator/hello/.git/

Administrator@PC-27 MINGW64 ~/hello (master)
$ touch NTUB.html

Administrator@PC-27 MINGW64 ~/hello (master)
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        NTUB.html

nothing added to commit but untracked files present (use "git add" to track)

Administrator@PC-27 MINGW64 ~/hello (master)
$ git log
commit 215f8f98f978d5f4f6c6a9e99123d14155d57d85
Author: Nini <cowe501@gmail.com>
Date:   Fri Feb 24 11:07:18 2017 +0800

    HELLO~~~~

Administrator@PC-27 MINGW64 ~/hello (master)
$ git commit -m'NTUB.html'
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
        NTUB.html

nothing added to commit but untracked files present

Administrator@PC-27 MINGW64 ~/hello (master)
$
