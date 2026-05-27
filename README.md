[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/XcAsiIew)
# DeadlockExample
Very simple example of deadlock.

1. Compilar

```bash
javac Deadlock.java
```

2. Executar

```bash
java Deadlock
```

## Resultados

```bash
$ java Deadlock
Thread 1: Holding Lock A...
Thread 2: Holding Lock B...
Thread 2: Waiting for Lock A...
Thread 1: Waiting for Lock B...
# Após a correção
$ javac Deadlock.java
$ java Deadlock
Thread 1: Holding Lock A...
Thread 1: Waiting for Lock B...
Thread 1: Acquired Lock B!
Thread 2: Holding Lock A...
Thread 2: Waiting for Lock B...
Thread 2: Acquired Lock B!
```
