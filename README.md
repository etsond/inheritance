# Inheritance
This C program simulates genetic inheritance of blood type through a family tree. It does this by creating a struct person which represents an individual in the family tree. Each person has two pointers to their parents, and two alleles, which represent their blood type.

## Requirements
This program requires a C compiler, such as GCC, to build and run.

## Usage
```ruby
$ gcc inheritance.c -o inheritance
$ ./inheritance

 ```
## How it works
The program uses a recursive function create_family to create a new individual and their parents, each with two blood type alleles. If there are still generations left to create, the function recursively calls itself to create two new parents for the current individual. The program then randomly assigns the individual's alleles based on those of their parents.

Once the family tree has been created, the program uses another recursive function print_family to print the blood types of each individual in the family tree. The program first prints the individual's blood type and generation, then recursively prints the blood types of their parents.

Finally, the program uses free_family to free the memory allocated for the family tree.

## Credits
block code https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks
