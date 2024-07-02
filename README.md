# A Kernel Seedling
TODO: intro

## Building
```shell
make clean | make | sudo insmod proc_count.ko 
```

## Running
```shell
cat /proc/count 
```
There were 111 processes

## Cleaning Up
```shell
sudo rmmod proc_count | make clean 
```

## Testing
```python
python -m unittest
```
The program output was:
Ran 3 tests in 7.993s

OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Linux 5.14.8-arch1-1 
