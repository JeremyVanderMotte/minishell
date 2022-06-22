# minishell

The goal of this project is to recreate a shell (bash is the reference).

We need to recode some buitlin commands :
- `cd`
- `pwd`
- `env`
- `export`
- `echo`

When launched, the program display a prompt and we are able to use it like a shell. We can type builtin command or not.  
If this is not a builtin command, the program will try to find a path using the `$PATH` variable where the command is. It will try every path is founding until he succeed to execute the command. If not, it will print `command not found`.  
The program have behavior like bash while typing special command like `cat | cat | ls`.
  
Allowed commands :  
- buitlin or command used in bash (ls, cat, ps, ...)
- pipe ( `|` )
- Redirection ( `<`, `>`, `>>`)
- Heredoc ( `<<` )

⚠️ The program doesn't treat any other symbols.   
The program can take mutliple pipe and multiple redirection.  
The program sets the exit code to the correct one while executing command.
