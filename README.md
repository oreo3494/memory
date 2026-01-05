# Password Generator

Just a password generator, yep, thats it

# Try it, how?

Two ways, you can give it a try : 

## The release page 
An easy way to do it; head to the [release page](https://github.com/oreo3494/password-generator/releases). There, download the executable respective to your system. 
 - As a `Windows` user, you may want to choose either `32 bit` or a `64 bit`, `.exe` file... \

 - `Linux` 
 Your system may not allow you to execute it by default... However you can modify its permissions using `chmod`.\
 Here's an example command :
```sh
$ chmod +X /path/to/binary/
```
 Of course replace `/path/to/binary` with the address to executable.


## Build from Source 
1. Before we even start... make sure you've `Rustup` (Rust toolchain installer) installed on your system... Don't have it installed? [Rust Book](https://doc.rust-lang.org/stable/book/ch01-01-installation.html) lends you some help.\

2. Clone this repository : 
```sh
git clone https://github.com/oreo3494/password-generator/
```
To install git, head to [git-scm.com](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)'s installation guide.

3. Change your current directory to to `password-generator`
```sh
cd /path/to/password-generator
```

5. Use `cargo`  to build an executable out its source code :
```
cargo build --release
```

⚠️ Copying to Clipboard won't work on wayland based display... instead, you would want to compiled with `--features wayland` flag,
```sh
cargo build --release --features wayland
```

5. If building ends up successful, there should be an executable present at `/target/release` with name `password-generator`.
