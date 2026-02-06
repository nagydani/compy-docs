# Become a Wizard

*This is the manual to Compy computer, a project dedicated 
to Steve Vickers, the author of the manual and the firmware 
for the ZX Spectrum computer.*

## Introduction

Welcome to **Compy**, a programmable general-purpose 
computer for introducing children between the ages of 5 and 
105 to the centuries-old tradition of **_wizardry_**. One 
could also say "*regular symbolic manipulations under a 
Turing-complete set of rules*" instead of "wizardry" and 
that would be certainly correct, but the latter seems a 
more fitting expression for the art of *creating* 
functioning mechanisms of unlimited complexity by merely 
describing them in a special language. Wizardry has been 
around for much longer than computers, so while *computer 
programming* is certainly wizardry, there is more to it 
than programming computers. A large part of mathematics and 
science is also wizardry and so is genetic engineering and 
many other important human endeavors. While capable wizards 
are today among the most sought-after specialists, 
mastering this art is its own reward, being one of the most 
stimulating intellectual exercises.

In this book, the first uses of important terms are set in 
**_bold italic_**. Usually, you will find the explanation 
of these terms somewhere around their first use. If not, 
you can look them up elsewhere or ask someone who knows 
what they mean. Framed texts are either **notes**, **fun 
facts** or **challenges**. Notes provide additional 
information typically relating the discussed topic to the 
broader context of the world beyond Compy. Fun facts are 
trivia related to the discussed topic, often providing a 
historical perspective. Challenges are, well, challenges. 
The first word in the frame, set in **bold regular** tells 
you which one that particular frame is. Texts that you 
should see on the screen, such as keywords, listings, 
reports and so on, are set in the native font of `Compy`.

*To be continued...*

## Meet the Console

After launching the **Compy IDE** app by double-clicking on 
the corresponding icon on Compy's **_desktop_**, one faces 
Compy's **_console_**. The console is how wizards talk to 
computers, in their own language.

The language your Compy understands is called **_Lua_**, 
which is Portuguese for "Moon".

> **Fun fact:** This is a word play, as Lua is a direct 
> descendant of another computer language called Simple 
> Object Language, or SOL for short, which, in turn, means 
> "Sun" in Portuguese. The creators of Lua lived in Rio de 
> Janeiro, Brazil and spoke Portuguese to one another. There 
> are many versions of Lua; ours is called
> [Lua 5.1](https://www.lua.org/manual/5.1/),
> which is one of the most popular ones, especially in the
> video game industry.

When you turn on your Compy, after about a minute, it 
brings up the Android home screen as its desktop, which is 
probably familiar to you from countless interactions with 
tablets and smartphones with the Android operating system. 
Prominently on it, you find the **Compy IDE** icon, to which 
you can point using either Compy's touchpad or the mouse 
that comes with Compy. Unlike most Android devices, Compy's 
screen is *not* touch sensitive. After double-clicking the 
icon with the *left* button of the mouse or the touchpad, 
the entire screen except the very bottom turns into muted 
white.

Start **Compy IDE**.

You are using the console now, as indicated in the 
beginning of the **_status line_**, that black stripe with 
bright letters in it near the bottom of the screen. It is, 
essentially a dialog with the computer, similar to instant 
messaging. You type something, hit the **Enter** key and 
the computer responds. **Enter** is just about the most 
important key on the keyboard. Just pressing it means, 
"*Okay computer, I've typed in your orders. Now go and obey 
them.*"

As you start typing, you can immediately notice that the 
screen is divided into two parts by the status line. In 
fact, the part *below* it is the console, the part above it 
is the **_canvas_**. Inside the status line, you find the 
following information: `console` stands for the kind of 
input the console expects from you. In this case, it 
expects a sequence of **_statement_**s in Lua. Then you 
have `L1:1`, which just indicates that you are about to 
type the first letter of the first statement.

The bright vertical line is the so-called cursor which 
shows you where what you type is going to appear. If you 
have already typed in anything, you can move the cursor 
using the arrow keys. You can also delete what is *before* 
the cursor (which is normally what you have typed last) by 
hitting the **⟵** key in the top right corner, just below a 
key marked **Delete**, which deletes what is *after* the 
cursor.

If you press **Caps Lock**, a green light at the bottom 
right marked with a padlock symbol with a capital A lights 
up (try!), meaning that you will by typing in CAPITAL 
LETTERS. You can change back to regular mode by pressing 
**Caps Lock** again. You can also type capital-case letters 
in regular mode by pressing and holding either of the 
**Shift** keys before hitting the letter key. The **Shift** 
key needs to be pressed while you are hitting the letter 
key in order for it to produce a capital letter. If you 
keep any key pressed long enough, it will repeat its 
function. To type the symbols above number or letter keys, 
you should also press one of the **Shift** keys similarly 
to how you type capital-case letters. In general, if there 
are two symbols above one another on a key, the bottom one 
is typed *without* the **Shift** key, while the top one is 
typed *with* it.

Below the left **Shift** key, there is a key labeled 
**Ctrl** (pronounced "Control") that is similar to 
**Shift** in that it needs to be pressed down for 
modifying what some other key does. For example, if you 
feel like you messed up and want to get out of the 
console, **DO NOT PANIC**: just press **Ctrl** + **Esc** 
(pronounced "Escape"). If you launch **Compy IDE** again, 
things will be back to normal.

Now you know enough to start chatting with Compy.

## The Language Of The Machine

If you try to greet the computer by typing `Hello Compy!`, 
you will notice that what you are typing is displayed in 
red. This is the computer's tactful way of telling you it 
does not understand a word you're saying. If you hit 
**Enter**, it will actually tell you — in English, red on 
black — what its actual problem is with what you have just 
written, but at this point it probably makes little sense 
to you, so just press any key to get back to typing in the 
console.

If you type `Draw.`, you'd notice that the word is now in 
black, with only the dot being red. The computer does still 
not understand what this is supposed to mean, though it 
understands a bit more than last time. If you hit 
**Enter**, the list of complaints is a lot shorter, though 
still a bit cryptic.

> **Note:** Even though the keywords and identifiers of Lua 
> are mostly English words, *Lua is not English*. For the 
> computer to understand what you type, it needs to be 
> correct Lua, not correct English. For instance, in Lua, 
> you do not end statements with a period.

Now, let's try something that would actually make sense to 
the computer. Type `print("Hello, World!")`. You'd notice 
that `print` is displayed in black, the opening and closing 
parentheses are dark blue, while the quoted text is green. 
If you hit **Enter**, the computer will respond with
```
Hello, World!
```
on the canvas.

> **Fun fact:** Statements instructing the computer to answer 
> us in writing begin with the word `print`. The reason for 
> this is historical: computers got consoles before they 
> became able to display anything on screens. In those 
> days, the console's output was a roll of paper on which 
> things were literally *print*ed. While this has no longer 
> been the case for many decades now, the notation stuck.

Here are a few more things that you can try out to see what 
they do (type them in this order):

```lua
love.graphics.circle("fill", 200, 200, 100)
gfx = love.graphics
gfx.setColor(Color[2])
gfx.circle("fill", 250, 200, 100)
sfx = compy.audio
sfx.beep()
sfx.win()
sfx.lose()
gfx.clear()
compy.terminal.clear()
```

Now let's try this: type `print(2+2)`. The word `print` is, 
again, displayed in black. The parentheses and the plus 
sign are dark blue. The twos are purple. If you hit **Enter**, 
the computer dutifully writes `4` on the canvas.

What happened here? The `4` is, as you might have guessed, 
the **_evaluation_** of `2+2`. But what are all these 
different colors? Red is reserved for things that do not 
make any sense in Lua. Black denotes **_identifiers_**, 
sequences of symbols (typically letters) that identify 
something, much like *names*. In fact, wizards often use 
the word "name" when they speak about identifiers. Blue 
denotes Lua **_keywords_**, sequences of symbols (not 
necessarily letters) that *cannot* be identifiers, as their 
meaning is fixed in the Lua language. Green and purple are 
used for **_literals_**, things that literally mean what 
they say. Specifically, **_string_** literals meaning the 
text enclosed in the quotes are displayed in green, 
**_numeric_** literals meaning the number are displayed in 
purple.

So, now you can use the computer as a calculator.

> **Note:** Computers are very fussy that you should 
> distinguish between the digit zero and the letter O. To 
> make it absolutely clear, zero appears on the screen as 
> `0`, with a dot in the middle. You also need to distinguish 
> between the digit one (`1`), the capital letter i (`I`) and 
> the small letter L (`l`). All ten digits are on the second 
> row of the keyboard. Furthermore, you must use the star 
> (`*`) for multiplication, *not* the letter x.

## Identifiers

*"When **I** use a word", Humpty Dumpty said in rather a 
scornful tone, "it means just what I choose it to mean — 
neither more nor less."*

*— Lewis Carroll: "Through the Looking Glass"*

Identifiers can mean anything. Whenever we want to *name 
something*, we can **_assign_** an identifier. Identifier 
assignment in Lua is done by using the equal sign (`=`) 
with the identifier on its *left* and the value on its 
*right*. For example, we can assign the identifier `two` the 
numeric value `2` like this:

```lua
two = 2
```

After pressing **Enter**, we can immediately use this 
identifier. Try this:

```lua
print(two + two)
```

As you can see, the computer now understands the new 
identifier. In Lua, all unassigned identifiers have a 
special value, `nil`, which in Lua means "nothing". Try 
entering this:

```lua
print(nothing)
```

As you might have noticed, `print` is also just an 
identifier. We can make some other identifier to mean the 
same thing:

```lua
display = print
```

> **Note:** What you put on which side of `=` is 
> *important*. For example, the above example *cannot* be 
> written as ~~`print = display`~~, because it would 
> assign the value of `display` (which is currently `nil`) 
> to `print`, thus making it impossible to use.

As you would expect, from now on, `display(two)` would 
display `2`. Try it. We can even re-assign `print` to mean 
something else entirely, but that could be very confusing. 
You can try it now, but in the future, try not doing it 
unless absolutely necessary.

> **Note:** Identifiers are, indeed, completely arbitrary 
> from the computer’s point of view. For a human mind, 
> however, it is very difficult to let go of conventional 
> meanings. Most programming languages, Lua very much 
> included, are meant to be understandable by *both* 
> computers and humans. Thus, in order not to confuse 
> fellow wizards or ourselves in the future, it is 
> strongly recommended to use meaningful identifiers. The 
> art of choosing what and how to denote with identifiers 
> is one of the most important skills of a wizard and is 
> to be refined through experience over a lifetime.

## Values

So far, we have seen identifiers denote two kind of 
things: **_numbers_** and **_functions_**, the latter 
being things that do something, like `print`. We are going 
to discuss them in much more detail a bit later. We 
already know that they can also denote nothing (called `nil` 
in Lua). What other things there are that can be assigned 
an identifier?

We have already had a glimpse of how textual information 
is handled using **_strings_**. Let’s look into it in a 
bit more detail. String literals can also be assigned to 
identifiers, like this:

```lua
greeting = "Hello, World!"
```

After which `print(greeting)` displays the above assigned 
greeting. There are also ways to describe strings other 
than literals. For example, we can tie two strings 
together (wizards call this **_concatenation_**) using the 
double dot:

```lua
greetings = greeting..greeting
```

Now try `print(greetings)`. There are many more ways that 
we will learn later.

What if we want the computer to verify whether a statement 
is true or not? Try `print(2 > 1)` and `print(2 < 1)`. As 
expected, the result is `true` and `false`, respectively. 
These are also values that can be assigned. They are 
called **_boolean_** values, and there are only these two 
of them.

> **Note:** In Lua, `true` and `false` are keywords, not 
> identifiers. They cannot be reassigned, they *always* 
> mean the two boolean values.

To verify whether or not two values are *equal*, we use 
the double equal sign (`==`), since the single equal sign 
is already taken to mean assignment. To verify whether or 
not they are *unequal*, we use `~=`. These can be used for 
any kind of value, not just numbers. To flip a boolean 
value from `true` to `false` or from `false` to `true`, we 
can use the keyword `not`. Try `print(not true)`.

> **Challenge:** Before trying, guess what would be 
> displayed by `print(not not true)`

Unsurprisingly, `print(two ~= 2)` and `print(not two == 2)` 
give the same result.

> **Fun fact:** Booleans are named after **George Boole**, 
> the wizard that introduced the rigorous rules of 
> **_binary_** (two-valued) logic almost two centuries 
> ago. It is important to note that this is not the only 
> possible logic, though it is the one used by the 
> overwhelming majority of computer languages, so it is 
> worth learning very well.
>
> One can also create similarly rigorous rules around 
> **_ternary_** (three-valued) logic, where in addition to 
> `true` and `false`, we also have `unknown` and build 
> computers around it. In fact, it has been done in the 
> past and may well be done in the future, but at present 
> it out of fashion.

These (`nil`, booleans, numbers, strings and functions) 
are the only **_primitive_** value types in Lua, meaning 
that all other values are composed of these. In Lua, there 
is only one **_composite_** value type, the **_table_**, 
in which the computer can look up a value using another 
value. Tables are going to be discussed in a lot more 
detail a bit later, but here is a glimpse of how they 
work.

An **_empty table_**, in which every lookup results in 
`nil`, is denoted by `{ }`. Let’s assign an initially empty 
table to the identifier `my_table`:

```lua
my_table = { }
```

Now, we can add **_entries_** to the table:

```lua
my_table[1] = "one"
my_table[2] = "two"
my_table[false] = 0
my_table["foo"] = "bar"
```

All unassigned values are `nil`, as expected. Try 
`print(my_table[1 + 1])`. The value in square brackets is 
called **_key_** or **_index_** (these two words usually 
mean the same thing in wizardry).

> **Note:** With the exception of `nil`, all values can be 
> used as a *key* in a table, including functions and 
> tables, but using the latter two is highly unusual and 
> can be very confusing. It is better avoided.

In fact, Lua identifiers are just values in a table with 
the identifier `_G` (underscore followed by capital G) 
called the **_global table_**, where the keys are strings 
holding the identifiers. You can check that 
`print(_G["print"] == print)` actually prints `true`.

Now you can understand identifiers.

## Functions

Functions are the essence of wizardry. One way to think 
about functions is to imagine them as machines. They may 
consume some values, called **_arguments_** of the 
function, they may produce some values, called, well, the 
(return) values of the function. And they can also have some 
**_side effects_**.

Functions come into existence by describing what they do: 
what are their arguments and how their side effects and 
values depend on them. Wizardry!

So far, `print` is the only function with a name that we 
have seen. It can have an arbitrary number of arguments. 
It returns no values. Its most important side effect is 
displaying all its arguments on the screen, separated by 
whitespaces and beginning a new line at the end.

We can describe our own functions with the `function` 
keyword. Let's try an example which takes two arguments 
and prints them below one another:

```lua
print2 = function(first, second) print(first) print(second) end
```

Try `print2("one", "two")`. What have we just done? The 
command above is an *assignment*, assigning a value to the 
identifier `print2`, which happens to be a function.

The description of a function begins with the `function` 
keyword and ends with the `end` keyword. After the 
`function` keyword, we find a comma-separated list of 
identifiers for the arguments in parentheses. When we 
**_call_** the function, these identifiers will be 
*temporarily* assigned the values of the function. After 
the argument identifiers, a sequence of **_statements_** 
follow, which are very similar to commands, except in that 
they are not executed immediately. This is called the 
**_body_** of the function.

When we entered the command `print2("one", "two")`, we 
have actually *called* `print2`. Calling a function is 
denoted by putting a comma-separated list of arguments in 
parentheses after he identifier of the function. If we 
wish to call a function without supplying any arguments, 
we follow the function identifier by an opening 
parenthesis immediately followed by a closing one.

> **Challenge:** Before trying, guess what `print2()` 
> would display.

Assigning function identifiers is such a common thing to do 
that there is a shorthand for it, which is how we are going 
to write it in most cases:

```lua
function print2(first, second) print(first) print(second) end
```

