# x86_64-elf-gcc
Setup tool to build GCC cross compiler toolchain for x86_64 elf

## How to install

### Step 1: Run setup.sh
In bash, you can install this with this.
```sh
cd your-workspace
git clone https://github.com/danidoco/x86_64-elf-gcc/
cd x86_64-elf-gcc-main
chmod +x setup.sh
sudo ./setup.sh
```

Note: ```./setup.sh``` can take 30 minutes to an hour.

### Step 2: Edit bashrc
Add a line of code to ```~/.bashrc```.
```sh
export PATH="$PATH:/usr/local/x86_64-elfgcc/bin"
```

### Step 3: Checking
Type this:
```sh
x86_64-elf-gcc
```

And then if you see this message, it's a success.
```
x86_64-elf-gcc: fatal error: no input files
compilation terminated.
```
