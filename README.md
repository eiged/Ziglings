# Ziglings

[OG Zigling  readme link](https://codeberg.org/ziglings/exercises/src/branch/main/README.md)

Noting down here info about each exercie :
1. Zig functions are private by default but the main() function should be public.
2. The @import() function is built into Zig. It returns a value which represents the imported code. It's a good idea to store the import as a constant value with the same name as the import. For the curious: Imports must be declared as constants because they can only be used at compile time rather than run time. Zig evaluates constant values at compile time.
3. General type / var assignement stuff : const u8, var i32...
4. When Zig can infer the size of the array, you can use '\_' for the size. It can also infer the type of the value. 
Len property : const length = arrayName.len.<br>
 var foo: [3]u32 = [3]u32{ 42, 108, 5423 }; -> var foo = [\_]u32{ 42, 108, 5423 };
5. Array operators only operate at compile time. Also for loops : for (\<item array>) |item| { \<do something with item> }
6. Single chars use ' '. Strings use " ". Strings are stored as array of bytes.
7. Nothing special. Can declare multi line strings with \\\ at the beginning of the line
8. Quiz. If we want to declare something to memory without defining yet, we can use 'undefined' : var test: [3]u8 = undefined;
9. Basic if/else. Special thing is that Zig accepts booleans as conditions. It does not allow other types to be automatically converted into boolean values.
10. Ifs can be used as expressions too -> const foo: u8 = if (a) 2 else 3;
11. Basic while. Condition must be a boolean too.
12. 'while' statements can have an optional 'continue expression' which runs every time the while loop continues.
13. continue expression vs continue statement to pass this iteration of the loop
14. while -> break
15. for (items) |item| { }
16. for can also use an index of the current iteration. for (items, 0..) |item, index| { }
17. Quiz2. Nothing special, classic fizzbuzz

