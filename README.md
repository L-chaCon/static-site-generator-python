## Python Static Site Generator

This is a project created for a backend developer course on [boot.dev](https://www.boot.dev).

### How to run this project

To run this project, you just need to run the following commands in order. You can delete the 
`content` and `static` folders and replace them with whatever you want. These folders currently
contain examples from the [boot.dev](https://www.boot.dev/courses/build-static-site-generator) course.

```zsh
git clone https://github.com/L-chaCon/static-site-generator-python.git site_generator  
cd site_generator  
python3 -m venv .venv  
./main.sh
```

If you want to change the source `static` and `content` folders, just provide them as variables in
the `./main.sh` command. The first argument should be the `static` folder and the second should be
the `content` folder. For example:

```zsh
./main.sh my_static_folder my_content_folder
```

> [!NOTE] Considerations  
> Some considerations are:  
> - There is no inline nesting. This means if you have `**bold *italic* text**`, it will not work.  
> - The markdown has to be correctly formatted to work. This means there should be `\n\n` between blocks.
