# Vim Cheat Sheet
 
Commands 

Vim as main modes: Normal, Insert, and Visual:

- Normal mode is for navigation and commands.
- Insert mode is for text input.
- Visual mode is for selecting and manipulating text.

------------

- `:q` -> **Fecha um Ficheiro**
- `:q!` -> **Fecha um Ficheiro, sem guardar**
- `:wq` -> **Fecha um Ficheiro, e guarda**

- `r` -> **replace char**
- `x` -> **delete char**
- `dd` -> **delete line**
- `u` -> **undo**, `ctrl + r` -> **redo**

- `:nLinha` -> **Avanca para a linha "nLinha"**
- `o` -> **Insert line bellow**
- `w` -> **Go to next word**
- `b` -> **Go to last word**
- `yy` -> **Copy line**
- `p` -> **Paste line**
- `I (shift + i)` -> **Insert in the begining of the line**
- `A (shift + a)` -> **Insert in the end of the line**
- `G (shift + g)` -> **Go to the end of the file**

- `:!Shell comand` por exemplo `:!gcc *.c` 





- `awk '{print $0}' file.txt    `  -> **Print ao Ficheiro inteiro (same as cat)**
- `awk '{print}' file.txt          `  -> **O mesmo que o anterior**
- `awk -F ":" '{print $1}' file.txt`  -> **Definir limitador**
- `awk '{print $1 $6 $7}' file.txt`        -> **Imprimir colunas 1, 6 e 7**
- `awk '{print $1" "$6" "$7}' file.txt`    -> **Imprimir colunas 1, 6 e 7 separadas por espacos**
- `awk '{print $1"\t"$6"\t"$7}' file.txt`  -> **Imprimir colunas 1, 6 e 7 separadas por tabs**
- `awk 'BEGIN{FS=":"; OFS=";"} {print $1" "$6" "$7}' file.txt`  -> **Definir limitador do ficheiro e o limitador do output**
> BEGIN pattern: means that Awk will execute the action(s) specified in BEGIN once before any input lines are read.
- `awk -F "/" '/^a/ {print $NF}' file.txt`              -> **procura por todas as linhas comecadas por 'a' e da print da ultima coluna** 
- `awk -F "/" '/^a/ {print $NF}' file.txt | sort | uniq`-> **o mesmo que o anterior mas nao mostra repetidos e mostra por ordem alfabetica**
- `df | awk '/\/dev\/loop/ {print $1"\t"$2+$3}'`        -> **procura pelas linhas com "/dev/loop" e da print da primeira coluna mais a soma da segunda com a terceira**
- `awk 'length($0) > 7' file.txt`                       -> **Print so as linhas com length maior do que 7**
- `awk 'if($NF == "/bin/shell") print $0' file.txt`     -> **Print das linhas cuja a ultima coluna e igual a "/bin/shell"**
- `awk 'BEGIN {for(i=1;i<=10;i++) } print "A raiz de i*i e igual a i."'`-> **For loop in AWK**
- `awk '$1 ~ /^[a,b,c]/ {print $0}' file.txt`-> **Print qualquer linha em que o primeiro char e 'a', 'b' ou 'c'**
- `awk '{print substr($0, 4)}' file.txt`     -> **Print qualquer linha, mas so da print a partir do quarto char da linha**
- `awk 'match($0,/a/) {print $0 " tem \'a\' como letra no index" RSTART}' file.txt`-> **Print qualquer linha que tenha o char 'a', e da print ao index do mesmo**
- `df | awk 'NR==7, NR==11 {print NR, $0}` -> **Print da linha [7-11]**
> Note: NR = Number of Records, Numero de linhas.
- `awk 'END {print NR} file.txt' `           -> **Print numero de linhas do ficheiro**
- `awk 'END {print NR} file.txt file.txt2' ` -> **Print numero de linhas dos 2 ficheiros**
> END pattern: means that Awk will execute the action(s) specified in END after all input lines have been read and dealt with.
