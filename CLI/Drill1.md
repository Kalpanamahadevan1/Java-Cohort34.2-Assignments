## Practice Drill 1

### 1.Create the following directory structure. (Create empty files where necessary)
```
hello
├── five
│   └── six
│       ├── c.txt
│       └── seven
│           └── error.log
└── one
    ├── a.txt
    ├── b.txt
    └── two
        ├── d.txt
        └── three
            ├── e.txt
            └── four
                └── access.log
command :

mkdir -p hello/five/six/seven
mkdir -p hello/one/two/three/four

touch hello/five/six/c.txt
touch hello/five/six/seven/error.log
touch hello/one/a.txt
touch hello/one/b.txt
touch hello/one/two/d.txt
touch hello/one/two/three/e.txt
touch hello/one/two/three/four/access.log

explanation : 

- mkdir -p → creates directories including all parent directories.
- First command creates hello/five/six/seven.
- Second command creates hello/one/two/three/four.
- touch → creates empty files.
- Here I have created c.txt, error.log, a.txt, b.txt, d.txt, e.txt, and access.log

```

### 2.Delete all the files having the `.log` extension
```
command : find hello -type f -name "*.log" -delete

explanation : 

- find hello → search inside the hello directory.
- -type f → look for files only.
- -name "*.log" → match files ending with .log.
- -delete → remove them. So, these deletes error.log and access.log

```
### 3.Add the following content to `a.txt`
```
command : echo "Unix is a family of multitasking, multiuser computer operating systems that derive from the original AT&T Unix, development starting in the 1970s at the Bell Labs research center by Ken Thompson, Dennis Ritchie, and others" > hello/one/a.txt

explanation :
- echo "text" → prints the given text.
- > → redirects the text into the file (overwrites if file already exists).
- The full description of Unix is now stored inside a.txt.

Unix is a family of multitasking, multiuser computer operating systems that derive from the original AT&T Unix, development starting in the 1970s at the Bell Labs research center by Ken Thompson, Dennis Ritchie, and others

```
### 4.Delete the directory named `five`
```
command : rm -r hello/five

explanation :
- rm -r → removes a directory and its contents recursively.
- Deletes the entire five folder along with six and c.txt.

```
### 5.Rename the `one` directory to `uno`
```
command : mv hello/one hello/uno

explanation :
- mv → can be used to move or rename files/directories.
- Here it renames the folder one → uno.

```
### 6.Move `a.txt` to the `two` directory
```
command : mv hello/uno/a.txt hello/uno/two/
explanation :
mv → moves a file to another location.

```

Moves a.txt from uno into the two directory.
