# search
Search engine in the terminal.


# How to run?

    curl -s https://raw.githubusercontent.com/amogusussy/search/main/search >> ~/.local/bin/search
    
    echo "PATH=$PATH:~/.local/bin/" | tee -a ~/.bashrc # Make sure that ~/.local/bin is in $PATH
    
Then you can run it with this syntax:

    $ search example [-i,-t,-v, -s]


# Optimization

This uses Librex' API, which isn't very fast. You can host it on your local machine for better speeds with these commands:

    git clone https://github.com/hnhx/librex/
    cd librex
    php -S localhost:8080


Or, refer to [its wiki](https://github.com/hnhx/librex/wiki/How-to-host-LibreX) for use with Nginx.

Then, you can change the `ST` variable to the URL of your own instance. For example, with the above example of using localhost, you would change it to `ST = "http://localhost:8080/"`

In the future I might make this easier with config files.



---

If you've found any issues in my code, feel free to make an issue, or a pull request. 
