# Inheritance
This C program simulates the inheritance of blood types in a family tree. It creates a new family with a user-defined number of generations and assigns each individual random blood type alleles based on those of their parents.

## Requirements
This program requires a C compiler, such as GCC, to build and run.

## Usage
To run the program, simply compile and execute the inheritance.c file. The program will prompt the user to enter the number of generations for the family tree. It will then generate a family tree and print the blood types of each individual.

```ruby
$ gcc inheritance.c -o inheritance
$ ./inheritance
Enter the number of generations: 3
Child (Generation 0): blood type AB
    Parent (Generation 1): blood type BO
        Grandparent (Generation 2): blood type AB
        Grandparent (Generation 2): blood type OO
    Parent (Generation 1): blood type AB
        Grandparent (Generation 2): blood type AB
        Grandparent (Generation 2): blood type AO
 ```
## How it works
The program uses a recursive function create_family to create a new individual and their parents, each with two blood type alleles. If there are still generations left to create, the function recursively calls itself to create two new parents for the current individual. The program then randomly assigns the individual's alleles based on those of their parents.

Once the family tree has been created, the program uses another recursive function print_family to print the blood types of each individual in the family tree. The program first prints the individual's blood type and generation, then recursively prints the blood types of their parents.

Finally, the program uses free_family to free the memory allocated for the family tree.

## Credits
block code https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks
