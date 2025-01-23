# Ownership
**Rule 1: All data in rust has an owner**

**Rule 2: Data can only be held by 1 owner at a time**

`fn main(){`

`let s1 = String::from("Hello!");`

`let s2 = s1;`

`println!("{s1}"); //compile error: borrow of moved value s1`

`}`

^ this would not compile as the value of s1 is now owned by s2

(the heap allocated string is moved from s1 to s2, making s1 not the owner)

How to avoid this error?

we could clone s1 to s2 instead of changing the owner: (this creates a new copy of s1 and heap allocated it to s2)

`fn main(){`

`let s1 = String::from("Hello!");`

`let s2 = s1.clone();`

`println!("{s1}");`

`}`

Rule 2 Also Applies to functions

**Rule 3: When owner moves out of scope it is de-allocated**

`fn main(){`

`let s1 = String::from("Hello!");`

`let s2 = s1;`

`print_string(s2);`

`}`

`fn print_string(s:String){`

`println!("{s}");`

`} // s is now de-allocated`

^ here the value of s2 is now given to the argument of the function