*компиляция
javac "название файла"
пример: javac Lesson.javac

*запуск
java "название без расширения"
пример: java Lesson



GIT

Commands:
	git init - команда для инициализации репозитория(создается системная папка которая называется .git)
	git status - что происходит сейчас
	git add название.файла - для того чтоб гит следил за файлом
	git add . - для того чтоб гит следил за всеми файлами
	
	commit - это такой фикс нашей версии чтоб потом с ней можно было работать
	git commit -m(-message) "название сообщения"(любое)
	
	.gitignore - файл который игнорирует git(в такой файл вносятся перечень файлов и папок которые недолжны быть видны)
		его обязательно нужно затрэкать
	
	git commit -m "название коммита" - это ветка проекта(в ней будут(могут) вносится изменения)
	
	git branch - ветка
		разработчик создает новую ветку
	git branch test - создаст новую ветку test
		git branch -D test - удалит ветку test
	git checkout test - переключит нас на ветку test
	git checkout -b new - создаст и сразу переключится на новую ветку new
	
	git merge test - совместит основную ветку с веткой test
	
	
	Работа с github
	git config --global user.name ""
	git config --global user.email ""
	
	//////////////// команды для добавления репозитория на github\\\\\\\\\\\\
	
	echo "# testRepo" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git branch -M main
	git remote add origin https://github.com/jackPotTrash/testRepo.git
	git push -u origin main
	///////////////////////////////////////////////////////////////////////////
	
	Если в репозиторий GitHub добавлены новые коммиты, 
	пока вы работали локально, я бы посоветовал использовать:
	* https://stackoverflow.com/questions/24114676/git-error-failed-to-push-some-refs-to-remote
	git pull --rebase
	git push
	
	
	*md - mark down




usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
