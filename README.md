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
what they mean. Framed texts are either **notes**, 
providing additional information typically relating the 
discussed topic to the broader context of the world beyond 
Compy or trivia, interesting facts related to the discussed 
topic, often providing a historical perspective or 
**challenges**. The first word in the frame, set in **bold 
regular** tells you which one that particular frame is. 
Texts that you should see on the screen, such as keywords, 
program line numbers, listings, reports and so on, are set 
in the native font of `Compy`.

*To be continued...*

## Meet the Console

After launching the **Compy IDE** app by double-clicking on 
the corresponding icon on Compy's **_desktop_**, one faces 
Compy's **_console_**. The console is how wizards talk to 
computers, in their own language. Unlike the desktop, which 
is what muggles use to get the computer do what they need, 
the console allows you, in principle, to make the computer 
do *anything* that the computer is capable of doing at all. 
It might seem less fancy, but it is far more powerful and 
expressive than the desktop. Different computers might 
speak different languages on their console, but they are, 
in many ways, similar.

> **Note:** Truth be told, the console opened by this app 
> is *not* the *actual* console of Compy, and unlike the 
> latter, it *does* have certain limitations mainly to keep 
> the user and the computer safe from each other. However, 
> it is still enormously powerful, allowing everything one 
> might need to develop video games and other fun and 
> useful pieces of software.

The language your Compy understands is called **_Lua_**, 
which is Portuguese for "Moon". This is a word play, as it 
is a direct descendant of another computer language called 
Simple Object Language, or SOL for short, which, in turn, 
means "Sun" in Portuguese. The creators of Lua lived in Rio 
de Janeiro, Brazil and spoke Portuguese to one another. 
There are many versions of Lua; ours is called [Lua 
5.1](https://www.lua.org/manual/5.1/), which is one of the 
most popular ones, especially in the video game industry.

When you turn on your Compy, after about a minute, it 
brings up the Android home screen as its desktop, which is 
probably familiar to you from countless interactions with 
tablets and smartphones with the Android operating system. 
Prominently on it, you find the **Compy IDE* icon, to which 
you can point using either Compy's touchpad or the mouse 
that comes with Compy. Unlike most Android devices, Compy's 
screen is *not* touch sensitive. After double-clicking the 
icon with the *left* button of the mouse or the touchpad, 
the entire screen except the very bottom turns into muted 
white.

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
hitting the **⟵** key int top right corner, just below a 
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

Now you know enough to start chatting with Compy.

## The Basics of Lua

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

> **Trivia:** Statements instructing the computer to answer 
> us in writing begin with the word `print`. The reason for 
> this is historical: computers got consoles before they 
> became able to display anything on screens. In those 
> days, the console's output was a roll of paper on which 
> things were literally *print*ed. While this has no longer 
> been the case for many decades now, the notation stuck.

So let's try this: type `print(2+2)`. The word `print` is, 
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

