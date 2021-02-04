The output i of both the c and the go program just became a different random number every time i ran the code. This is because the two threads interfere with eachother, because
both processes are trying to read, modify and write the value of i at the same time.
