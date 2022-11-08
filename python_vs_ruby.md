
# Python vs Ruby

A small comparison of Python and Ruby

### Version manager

To select the right version both languages offer
different version managers.
```
(ana)conda                     rvm or rbenv
```

### Package installation

In Python we have packages fron https://pypi.org/ ,
in Ruby we have gems from https://rubygems.org/

```
Python Packages                Ruby Gems
pip install ..                 gem install ..
```

### For loops in Python/Ruby

In both languages we can do simple "for" loops
```
for i in range(0, 6):          for i in 0..5
  if i < 2: continue             next if i < 2
  print(i)                       puts i
                               end
```

### Type checks

Both languages are dynamically typed languages, but
sometimes it is good to know the type
```
type(x) is str                 x.is_a? String             
isinstance(x, str)             x.instance_of? String
```

### Functions

In Python we need to remember the colon ":" at the end of a line,
in Ruby we need to remember the "end" after a block or function.
```
def hello(text):               def hello(text)
  print(text)                    puts(text)
                               end
```

### String formatting

In Python we need to add an "f" as prefix for formatted strings,
in Ruby we need to add a hash "#" for string interpolation.
```
x = "World"                    x = "World"
print(f"Hello {x}")            puts("Hello #{x}")
```

### Debugging / Debugger

In Python we can use "print" for debugging, in Ruby "puts",
and both languages have powerful debuggers

```
# Python Debugger              # Ruby Debugger
import pdb                     require 'pry'
pdb.set_trace()                binding.pry
```

### List comprehension         Block enumeration 

In Python we have list comprehension, in Ruby we can use blocks 
```
for x in [1,2,3]: print(x**2)  (1..3).each do |x| puts x**2; end
```

for example if we want to map a function
```
[i+1 for i in [1, 2, 3]]       [1, 2, 3].map{ |i| i+1 }   
=> [2, 3, 4]                   => [2, 3, 4]
```
or
```
def square(i):                 def square(i)
  return i*i                     return i*i
                               end

list(map(square, [1, 2, 3]))   [1, 2, 3].map{ |i| square(i) }   
=> [1, 4, 9]                   => [1, 4, 9]
```
