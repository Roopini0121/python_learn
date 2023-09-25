# python

**Terminal:** 

run python on terminal: 

-python3

control D (will give prompt) 

ls>> to list the no. of folders

cd>> to go to the folder. 

name the folder and run the python file from the folder

- **commands**
    - `ls` list to list the folders in the current directory
    - `ls -a` list all
    - `cd ..` go out of the folder
    - `cd` change directory eg: cd then name of the folder.
    - `pwd` path to working directory shows where you are currently
    - `^C` control c to stop running the code
    - `mv` to move the file
    - `cat` -command to list out the different files and use the `combined` to combine the folders
    - `*` wildcard command
    - `rm` - to delete
    - `^d` to quit
    - `less`
    - `cut`
    - `grep`  to find the word in the folder
- strings
    
    <aside>
    💡 **Ex. 1.** **apostrophe words**- Isn't, Hasn't, etc use quotes " "
    
    </aside>
    
    print('"Isn\'t," they said')
    
    output— "Isn't", they said
    
    <aside>
    💡 **Ex.2. Lines**—
    
    </aside>
    
    - print('first line. second line')
    
    output— first line. second line
    
    - print('first line\nsecond line')
    
    output—first line
    
                  second line
    
    - print('c:\some\name')
    
    output—C: some
    
                   ame
    
    instead use *raw string 'r' to avoid overlap of commands.* 
    
    - print(r'C:\some\name')
    
    output— some
    
                   name
    
    <aside>
    💡 **Ex. 3. Words—**
    
    </aside>
    
    word='python' 
    
    word[0]
    
    'p'
    
    word[5]
    
    'n'
    
- Python for everyone
    
    **lesson 2: Hardware**
    
    - Input: keyboard, mouse
    - Output: screen, speakers, printers, DVD burners
    - CPU
    - Main memory: temp memory whc answers demands from CPU as a feedaback- RAM
    - secondary memory: memory stored permanently
    - operator
        - // quotient without remainder
        - % remainder
        - == equal to
        - ! = (without space) not equal to
        

---

- ******************************WRITING SCRIPTS******************************:
    
    ***sequential***
    
    ***conditional***
    
    - if condition
    
    ***repeated***
    
    - **WHILE LOOP**
        - eg. n=5
        
        while n>0 :
        
        print (n)
        
        n=n-1
        
        print (done)
        
    - **convert string to integer**: name1= input
    
                                                       name_actual= int(name1)
    
    - **def- DEFINITION OF A FUNCTION**
        - assign a function. eg:
        
        ```python
        function (x): (colon important)
        	..... state the funtion tak
        	if ..... : (your function task with colon)
        		print (....) (indent important)
        	else: (colon)
        		print 
        call the function (whatever you want to calculate) 
        
        indent for conditions and two indents below that for print
        ```
        
    
    You can print multiple lines consecutively
    
    eg. print(”goodbye:”) 
    
    print(”any name”)
    
    output: goodbye:
    
    “any name”
    

---

- **string conversions**
    
          sval=’123’
    
    type(sval)
    
    <class ‘str’>
    
    ival=int(sval).       : convert sval (string) to integer (int)
    
    type(ival)
    
    <class ‘int’>
    

- **string concatenation**
    - Use the `+` operator to concatenate strings. For example, `"Hello" + "world"` will output `"Helloworld"`.
    - You can also use the `` operator to repeat a string. For example, `"Python" * 3` will output `"PythonPythonPython"`.
    - String concatenation can also be done with variables. For example, `name = "John"` and `age = 25` can be concatenated with `"My name is " + name + " and I am " + str(age) + " years old."` to output `"My name is John and I am 25 years old."`.

> **String concatenation with `+=`:** You can use the `+=` operator to concatenate strings in place. For example, `name = "John"` and `name += " Doe"` will change `name` to `"John Doe"`.
> 

- ***To create a multi-line string in Python***, you can use triple quotes (`"""`). For example:
    
    ```
    string = """
    This is a multi-line string.
    It can span multiple lines.
    """
    
    ```
    
    Alternatively, you can use the escape character (`\\`) to indicate a line continuation. For example:
    
    ```
    string = "This is a multi-line string. \\
    It can span multiple lines."
    
    ```
    
    Both of these methods will result in a string that spans multiple lines.
    

- **Boolean Operators:**
    - `and` - Returns `True` if both operands are `True`.
    - `or` - Returns `True` if either operand is `True`.
    - `not` - Returns `True` if the operand is `False`, and vice versa.
    
    **c*omes under conditional statements.*** 
    
    Boolean is a separate type named ‘bool’ and always uses Caps ‘T’ or ‘F’ 
    
    — If used as true or false, will return as string. 
    
    — Boolean operators **NOT** enclosed within “” or ‘ ‘ 
    

---

- **LISTS:**
    - Lists written in [] brackets with a comma separating each integer or string or boolean
        
        ```python
        Append: .append() will add a number or string 
        Remove: .remove() will remove number or string
        eg.1 names= ["priya", "monika", "ben"]
        names.append("shiny")
        print(names)
        
        output: priya, monika, ben,shiny
        
        eg.2
        name_list= ["priya", "monika", "ben", "shiny"]
        name_list.remove("shiny")
        print(name_list)
        
        output: priya, monika, ben
        ```
        
    - 2D list: more than one value can be added within one list
    
    ```python
    height= [["Harry", 72], ["Prince", 67]]
    
    - accessing 2D lists
    
    class_name_test= [["Jenny", 90], ["Alexus", 85.5], ["Sam", 83], ["Ellie", 101.5]]
    print(class_name_test)
    sams_score= class_name_test[2][1]
    print(sams_score)
    ```
    
    - **To slice** a list in Python, you can use the colon (`:`) operator. The syntax is as follows:
    
    ```python
    list[start:end:step]
    
    ```
    
    - `start` is the index where the slice starts (inclusive).
    - `end` is the index where the slice ends (exclusive).
    - `step` is the step size between each element in the slice.
    
    Here are some examples:
    
    ```
    numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]
    
    # Get the first three numbers
    print(numbers[:3])  # Output: [1, 2, 3]
    
    # Get the last three numbers
    print(numbers[-3:])  # Output: [7, 8, 9]
    
    # Get every other number
    print(numbers[::2])  # Output: [1, 3, 5, 7, 9]
    
    ```
    
    You can also modify the elements in a slice by assigning to it:
    
    ```
    my_list = [1, 2, 3, 4, 5, 6, 7, 8, 9]
    
    # Replace the first three numbers with zeros
    my_list[:3] = [0, 0, 0]
    print(my_list)  # Output: [0, 0, 0, 4, 5, 6, 7, 8, 9]
    
    ```
    
    - **Counting in list**
    
    ```python
    #counting single items
    num_i= variable.count()
    
    eg: letters = ["m", "i", "s", "s", "i", "s", "s", "i", "p", "p", "i"]
    num_i = letters.count("i")
    print(num_i)
    
    output: 4
    
    #counting pairs of items
    num_pairs= variable.count()
    
    eg:number_collection = [[100, 200], [100, 200], [475, 29], [34, 34]]
    num_pairs= number_collection.count([100, 200])
    
    output: 2
    
    ```
    
    - **Sorting List**
    
    To sort a list in Python, you can use the `sort()` method. By default, this method sorts the list in ascending order:
    
    ```
    numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    numbers.sort()
    
    print(numbers)  # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]
    
    ```
    
    If you want to sort the list in descending order, you can pass the `reverse=True` argument to the `sort()` method:
    
    ```
    numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    numbers.sort(reverse=True)
    
    print(numbers)  # Output: [9, 6, 5, 5, 5, 4, 3, 3, 2, 1, 1]
    
    ```
    
    You can also use the `sorted()` function to sort a list. This function returns a new sorted list and leaves the original list unchanged:
    
    ```
    numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    sorted_numbers = sorted(numbers)
    
    print(sorted_numbers)  # Output: [1, 1, 2, 3, 3, 4, 5, 5, 5, 6, 9]
    
    print(numbers)  # Output: [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    ```
    
    You can also pass the `reverse=True` argument to the `sorted()` function to sort the list in descending order:
    
    ```
    numbers = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    sorted_numbers = sorted(numbers, reverse=True)
    
    print(sorted_numbers)  # Output: [9, 6, 5, 5, 5, 4, 3, 3, 2, 1, 1]
    
    print(numbers)  # Output: [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
    
    ```
    
    **Summary**
    
    - Add elements to a list by index using the `.insert()` method.
    - Remove elements from a list by index using the `.pop()` method.
    - Generate a list using the `range()` function.
    - Get the length of a list using the `len()` function.
    - Select portions of a list using slicing syntax.
    - Count the number of times that an element appears in a list using the `.count()` method.
    - Sort a list of items using either the `.sort()` method or `sorted()` function.
    
    The length of a list in Python can be found using the `len()` function. For example, if `my_list` is a list, `len(my_list)` will return the number of elements in the list.
    
- ***Exercise on list***

```python
inventory = ["twin bed", "twin bed", "headboard", "queen bed", "king bed", "dresser", "dresser", "table", "table", "nightstand", "nightstand", "king bed", "king bed", "twin bed", "twin bed", "sheets", "sheets", "pillow", "pillow"]
inventory_len= len(inventory)
first= inventory[1]
last= inventory[-1]
inventory_2_6= inventory[2:6]
first_3= inventory[:3]
twin_beds= inventory.count("twin bed")
removed_item= inventory.pop(4)
inventory.insert(10,"19th Century Bed Frame")
inventory.sort()
inventory_sorted= sorted(inventory)
print(inventory)
print(inventory_sorted)
```

- **SLICE EXERCISE**
    
    ```
    # Your code below:
    toppings= ["pepperoni", "pineapple", "cheese", "sausage", "olives", "anchovies", "mushrooms"]
    prices= [2, 6, 1, 3, 2, 7, 2]
    num_two_dollar_slices= prices.count(2)
    num_pizzas= len(toppings)
    print("We sell",(num_pizzas), "different kinds of pizza!")
    pizza_and_prices= [[2, "pepperoni"], [6, "pineapple"], [1, "cheese"], [3, "sausage"], [2, "olives"], [7, "anchovies"], [2, "mushrooms"]]
    pizza_and_prices.sort()
    print(pizza_and_prices)
    
    #first element
    cheapest_pizza= pizza_and_prices.pop(0)
    print(cheapest_pizza)
    #last element
    priciest_pizza= pizza_and_prices.pop(-1)
    print(priciest_pizza)
    
    #remove
    pizza_and_prices.pop(-1)
    pizza_and_prices.insert(4, [2.5, "peppers"])
    
    #3 cheapest pizza
    three_cheapest= pizza_and_prices[:3]
    print(three_cheapest)
    ```
    

---

- **FUNCTIONS**
    
    To define a function in Python, use the `def` keyword followed by the name of the function and the arguments in parentheses. The function body should be indented:
    
    ```python
    def my_function(arg1, arg2):
        # function body
        return result
    
    ```
    
    You can then call the function using its name and passing in arguments:
    
    ```python
    result = my_function(value1, value2)
    
    ```
    
    Note that the `return` keyword is used to return a value from the function.
    
    Here's an example of a simple function that takes two numbers and returns their sum:
    
    ```python
    def add_numbers(x, y):
        return x + y
    
    ```
    
    You can call this function like so:
    
    ```python
    result = add_numbers(1, 2)
    print(result)  # Output: 3
    
    ```
    
    Functions can also have optional arguments with default values:
    
    ```python
    def greet(name, greeting="Hello"):
        print(greeting, name)
    
    greet("John")  # Output: Hello John
    greet("Jane", "Hi")  # Output: Hi Jane
    
    ```
    
    In this example, the `greeting` argument has a default value of `"Hello"`, so it can be omitted when calling the function.
    
    Parameters in make dynamic functions
    
    eg: 
    
    ```python
    def trip_welcome(destination):
    ```
    
    ```python
    print("Welcome to Tripcademy!")
    ```
    
    ```python
    print("Looks like you're going to " + destination + " today.")
    ```
    

****Types of Arguments****

- Positional arguments: arguments that can be called by their position in the function definition.
- Keyword arguments: arguments that can be called by their name.
- Default arguments: arguments that are given default values.

********************************Built in Functions********************************

- print, str, len, max, round

---

- **STRINGS**
    
    Writing a string of words, using functions append, length etc 
    
    - An example of how to iterate through strings
    
    ![Screenshot 2023-09-12 at 11.15.01 AM.png](python%204f5f1f97f64a4ade97c4e3f381e18ef3/Screenshot_2023-09-12_at_11.15.01_AM.png)
    
    ```
    - Creating a user name and password. 
    name= Claire Phil 
    oucome password should be,
    1. ClaPhi (First 3/4 words of first and last name)
    
    2. IClaPh (last alphabet gets pushed to first)
    
    def username_generator(first_name, last_name):
      if len(first_name)<3:
        user_name= first_name
      else:
        user_name= first_name[0:3]
      if len(last_name)<4:
        user_name+= last_name
      else: 
        user_name+= last_name[0:4]
      return user_name
    
      #New_function
    def password_generator(user_name):
      password= ""
      for i in range(0, len(user_name)):
        password+= user_name[i-1]
      return password
    
    3. **#Finding common characters**
    
    def contains(big_string, little_string):
      return little_string in big_string
    
    #no.1
    def common_letters(string_one, string_two):
      character= []
      for letter in string_one:
        if (letter in string_two) and not (letter in character):
          character.append(letter)
      return character
    
    4. **#True or False**
    
    def letter_check(word, letter):
      for character in word:
        if character== letter:
          return True
      return False
    ```
    
    - **EXERCISE ON  STRINGS**
    1. Skipping characters in the even index
    
    ![Screenshot 2023-09-12 at 11.05.39 AM.png](python%204f5f1f97f64a4ade97c4e3f381e18ef3/Screenshot_2023-09-12_at_11.05.39_AM.png)
    
    - **FORMATTING IN STRINGS**
    
    ```jsx
    1. .lower()
    2. .upper()
    3. .title()
    4. .split()- delimiter. Splits each word in string. Outcome is printed as a list
    5. .join() eg (' '.join(variable)- We take the list of strings, and we joined it together with our delimiter, ' ', which is a space. The space is important if you are trying to build a sentence from words
    5. \n New line
    6. \t Horizontal tab
    7. .strip()- removes white space characters from beginning to end
    8. .replace() -
    	eg with_spaces = "You got the kind of loving that can be so smooth"
    	with_underscores = with_spaces.replace(' ', '_')
    	print(with_underscores)
    	# 'You_got_the_kind_of_loving_that_can_be_so_smooth'
    9. .find()- will find the index value
    10..format()- you can format within the string as well
    11. .isalpha()- used to check if all the characters in a given string are alphabetic (letters of the alphabet)
    				 - will return if string is true or false
    ```
    
    - Using strip and join together
    
    ```
    love_maybe_lines = ['Always    ', '     in the middle of our bloodiest battles  ', 'you lay down your arms', '           like flowering mines    ','\n' ,'   to conquer me home.    ']
    love_maybe_lines_stripped= []
    for line in love_maybe_lines:
      love_maybe_lines_stripped.append(line.strip())
    love_maybe_full= '\n'.join(love_maybe_lines_stripped)
    print(love_maybe_full)
    
    output
    Always
    in the middle of our bloodiest battles
    you lay down your arms
    like flowering mines
    
    to conquer me home.
    ```
    
    - Example project:
    
    ```
    highlighted_poems = "Afterimages:Audre Lorde:1997,  The Shadow:William Carlos Williams:1915, Ecstasy:Gabriela Mistral:1925,   Georgia Dusk:Jean Toomer:1923,   Parting Before Daybreak:An Qi:2014, The Untold Want:Walt Whitman:1871, Mr. Grumpledump's Song:Shel Silverstein:2004, Angel Sound Mexico City:Carmen Boullosa:2013, In Love:Kamala Suraiyya:1965, Dream Variations:Langston Hughes:1994, Dreamwood:Adrienne Rich:1987"
    print(highlighted_poems)
    
    #spiltting
    highlighted_poems_list= highlighted_poems.split(',')
    print(highlighted_poems_list)
    
    #strip it
    highlighted_poems_stripped=[]
    for space in highlighted_poems_list:
      highlighted_poems_stripped.append(space.strip())
    print(highlighted_poems_stripped)
    
    #separate lists
    highlighted_poems_details=[]
    for colon in highlighted_poems_stripped:
      highlighted_poems_details.append(colon.split(':'))
    
    titles=[]
    poets=[]
    dates=[]
    
    for poem in highlighted_poems_details:
      titles.append(poem[0])
      poets.append(poem[1])
      dates.append(poem[2])
    
    for i in range(0,len(highlighted_poems_details)):
        print('The poem {} was published by {} in {}'.format(titles[i], poets[i], dates[i]))
    ```
    

---

- ***Other functions***

1. Unicode function: Unicode is a standardized character encoding system that assigns a unique numeric code point (a number) to every character, symbol, emoji, and script used in writing systems worldwide.

The **`ord()`** function in Python is used to get the Unicode code point (integer representation) of a character.

```python
print(ord('A'))  # Output: 65 (Unicode code point for 'A')
print(ord('a'))  # Output: 97 (Unicode code point for 'a')
print(ord('1'))  # Output: 49 (Unicode code point for '1')
print(ord('€'))  # Output: 8364 (Unicode code point for the Euro symbol)
```

The **`chr()`** function in Python is used to convert an integer (Unicode code point) into its corresponding character. It returns a string containing a single character that corresponds to the provided Unicode code point.

```python
print(chr(65))  # Output: 'A' (Unicode code point 65 corresponds to the character 'A')
print(chr(97))  # Output: 'a' (Unicode code point 97 corresponds to the character 'a')
print(chr(8364))  # Output: '€' (Unicode code point 8364 corresponds to the Euro symbol)
```

---

- **************MODULES**************
    - A module is a collection of Python declarations intended broadly to be used as a tool. Modules are also often referred to as “libraries” or “packages”

```python
from module_name import object_name
```

We’ll work with two common `random` functions:

- `[random.choice()](https://www.codecademy.com/resources/docs/python/random-module/choice?page_ref=catalog)` which takes a list as an argument and returns a number from the list
- `[random.randint()](https://www.codecademy.com/resources/docs/python/random-module/randint?page_ref=catalog)` which takes two numbers as arguments and generates a random number between the two numbers you passed in

---

— ************************************************************Printing random numbers************************************************************

```python
import random

# Create random_list below:
random_list=[random.randint(1,100) for i in range(101)]

# Create randomer_number below:
randomer_number= random.choice(random_list)

# Print randomer_number below:
print(randomer_number)
```

---

— ************************Aliasing************************

- Aliasing is most often done if the name of the library is long and typing the full name every time you want to use one of its functions is laborious.

```python
import module_name as name_you_pick_for_the_module
```

---

— ************************************************************An Example of using matlotlib and creating a random plot************************************************************

— Also my first plot ❤️

![Screenshot 2023-09-21 at 2.27.31 PM.png](python%204f5f1f97f64a4ade97c4e3f381e18ef3/Screenshot_2023-09-21_at_2.27.31_PM.png)

---

- ************************DICTIONARIES************************
    - A *[dictionary](https://www.codecademy.com/resources/docs/python/dictionaries?page_ref=catalog)* is an unordered set of `key: value` pairs.
        
        ```python
        e.g  sensors = {"living room": 21, "kitchen": 23, "bedroom": 20, "pantry": 22}
        ```
        
    - 1. A dictionary begins and ends with curly braces `{` and `}`.
    - dictionaries can be lists, strings but not only integers
        
        
        ***— Adding a new key to the dictionary***
        
        To add a single `key: value` pair to a dictionary, we can use the syntax:
        
        ```
        dictionary[key] = value
        ```
        
        — *********************Adding multiple keys to the dictionary*********************
        
        - To add multiple keys use `[.update()](https://www.codecademy.com/resources/docs/python/dictionaries/update?page_ref=catalog)`
        
        ```python
        e.g sensors.update({"pantry": 22, "guest room": 25, "patio": 34})
        
        ```
        
        — ***Overwrite Values***
        
        ```python
        menu = {"oatmeal": 3, "avocado toast": 6, "carrot juice": 5, "blueberry muffin": 2}
        menu["oatmeal"] = 5
        print(menu)
        
        							(OR)
        oscar_winners = {"Best Picture": "La La Land", "Best Actor": "Casey Affleck", "Best Actress": "Emma Stone", "Animated Feature": "Zootopia"}
        oscar_winners.update({"Supporting Actress": "Viola Davis", "Best Picture": "Moonlight"})
        print(oscar_winners)
        
        ```
        
        ```python
        names = ['Jenny', 'Alexus', 'Sam', 'Grace']
        heights = [61, 70, 67, 64]
        
        ```
        
        Python allows you to create a dictionary using a dict comprehension, with this syntax:
        
        ```python
        students = {key:value for key, value in zip(names, heights)}
        #students is now {'Jenny': 61, 'Alexus': 70, 'Sam': 67, 'Grace': 64}
        
        ```
        
        — ***Getting a specific key***
        
        ```python
        zodiac_elements = {"water": ["Cancer", "Scorpio", "Pisces"], "fire": ["Aries", "Leo", "Sagittarius"], "earth": ["Taurus", "Virgo", "Capricorn"], "air":["Gemini", "Libra", "Aquarius"]}
        print(zodiac_elements["earth"], zodiac_elements["fire"])
        ```
        
        — ************************Checking if a key is in the dictionary************************
        
        - Use If “key word” in variable
        
        ```python
        zodiac_elements = {"water": ["Cancer", "Scorpio", "Pisces"], "fire": ["Aries", "Leo", "Sagittarius"], "earth": ["Taurus", "Virgo", "Capricorn"], "air":["Gemini", "Libra", "Aquarius"]}
        
        if "energy" in zodiac_elements:
          print(zodiac_elements["energy"])
        zodiac_elements["energy"]= "Not a Zodiac element"
        print(zodiac_elements)
        ```
        
        — ******To get a key safely (from a huge list when you do not know the key value)******
        
        - Use .get(”something”, nothing)
            - get - “something” (which you want to get) and nothing here determines — if “something” not present, print nothing.
        
        ```python
        user_ids = {"teraCoder": 100019, "pythonGuy": 182921, "samTheJavaMaam": 123112, "lyleLoop": 102931, "keysmithKeith": 129384}
        tc_id= user_ids.get("teraCoder", 100000)
        print(tc_id)
        
        #get another something
        stack_id= user_ids.get("superStackSmash", 100000)
        print(stack_id)
        ```
        
        — ******************************Remove Key******************************
        
        - Similar to removing in lists, use .pop()
            
            ```python
            available_items = {"health potion": 10, "cake of the cure": 5, "green elixir": 20, "strength sandwich": 25, "stamina grains": 15, "power stew": 30}
            health_points= 20
            
            health_points+= available_items.pop("stamina grains", 0)
            health_points+= available_items.pop("power stew", 0)
            health_points+= available_items.pop("mystic bread", 0)
            print(available_items, health_points)
            ```
            
        
        — ************Get all keys************
        
        - Operating on all keys; dict_keys, use:
        1. .list()
        2. .keys()- prints only keys
            
            ```python
            user_ids = {"teraCoder": 100019, "pythonGuy": 182921, "samTheJavaMaam": 123112, "lyleLoop": 102931, "keysmithKeith": 129384}
            users= user_ids.keys()
            print(users)
            
            #output
            dict_keys(['teraCoder', 'pythonGuy', 'samTheJavaMaam', 'lyleLoop', 'keysmithKeith'])
            
            ```
            
        
        — ******************************************Get all values******************************************
        
        - similar to dict_keys, use .values()
        
        ```
        num_exercises = {"functions": 10, "syntax": 13, "control flow": 15, "loops": 22, "lists": 19, "classes": 18, "dictionaries": 18}
        total_exercises= 0
        for exercise in num_exercises.values():
          total_exercises+= exercise
        print(total_exercises)
        
        #output
        115 (addition of all values)
        ```
        
        — *********Get all items (keys and values)*********
        
        - You can get both the keys and the values with the `[.items()](https://www.codecademy.com/resources/docs/python/dictionaries/items)` method. Like `[.keys()](https://www.codecademy.com/resources/docs/python/dictionaries/keys)` and `[.values()](https://www.codecademy.com/resources/docs/python/dictionaries/values)`, it returns a `dict_list` object. Each element of the `dict_list` returned by `.items()` by iterating through the list
        
        ```python
        pct_women_in_occupation = {"CEO": 28, "Engineering Manager": 9, "Pharmacist": 58, "Physician": 40, "Lawyer": 37, "Aerospace Engineer": 9}
        for occupation, value in pct_women_in_occupation.items():
          print("Women make up " +str(value)+ " percent of " + occupation+ "s")
        
        #output
        Women make up 28 percent of CEOs
        Women make up 9 percent of Engineering Managers
        Women make up 58 percent of Pharmacists
        Women make up 40 percent of Physicians
        Women make up 37 percent of Lawyers
        Women make up 9 percent of Aerospace Engineers
        ```