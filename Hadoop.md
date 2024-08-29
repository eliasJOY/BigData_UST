#### MapReduce Parallelism
- The key reason to perform mapping and reducing is to speed up the executon of a specific process by spilting a process  into number of tasks, this encorages parallelism in job flow.

#### Input split and reorder reader
- Used to spliting data as key and value
- Record reader (RR) are used to split sectences

### Steps In MapReducer:
1. First **Input** of a sentence is put through **Input Split**
2. The o/p of **InputSplit** is words from the sentences.
3. After going through **Record Reader** store the words as key and value pairs with numbers.
4. **Mapper** maps the value and key pairs
5. **Intermediate O/P in disk** Keeps the output under a temporary storage in disk. Also Know as HDFS.
5.a **Combiner** It is an optionsal, local reducer of which prformsas patrial aggregari0nf ampper output brr it
)
6. **Partitioner** Ensures same key goes to the same reducer. Shuffling and sorting happens after partitioning. Also called pre-reducer.
    - This alfo ensures load balancng. 

7. **Reducer** Does the aggregate operations and gives o/p.

Note: No if mappers and reducer depend upon no of Nodes

#### To change block size for specific in a cluster:
> hadoop fs -Ddfs.blocksize=<BLOCK_SIZE> -put <PATH> /hdfs

print("Addition of value1:%d and value2% %(val1,val2))

print(f"this is A:{} and B{}")

### sys. Module 
- Its part of python's standard library which offers you functions that allows you to interact with python intrepretor.
- *sys.exit* used to exit out.
-*sys.path* provides you list of string specifying the search path for the modules used.
- *sys.stdin* is fuile like object that represents standart input stream, used to read **input from user or from imput redirection**/ or input path. Used when input is required from command line.
- *sys.stdin.redline* can be used to read file in a more controlled way.
