--- 
layout: post 
title: Present Value of Happiness 
---

# Present Value of Happiness

_August, 2012_

_Disclaimer: This is totally amature thoughts of a computer science and
business administration junior._

In this post I will try to modelize your action taking mechanism using
economic terms. I will start by giving a very simple real world example and
describing it peice by peice to derrive final formula.

Let's say you have a midterm next week, basically there are two actions you
can take for this situation. First one is procastinating, and the other one
is studying without getting distracted. 

Which one will you choose? why does one of them sounds like an obvious
choose to you? and how will this affect your life? To be able to answer
these questions, we first need to understand the differenet consequneces of
these 2 reactions/investments.

If you choose to procastinate, let's call this reaction `R1` for given
situation, you will be happy `H1` untill the time of your midterm. After
you take your midterm you will be unhappy `UH1` ,because you did not study
enough and you know that you will get a bad grade.

On the other hand, if you chose to study, let's call it reaction `R2` for
this given situation, you will be very unhappy `UH2` during the time you
are studying. But after the midterm you will probably `P2` get a good grade
and be happy `H2`.

There is also an interest rate of happiness `I` that decides how much you
value your future happiness in todays unit happines `I` is unique for every
person and it is constant for a person. I believe that higher `EQ` you have
lower your `I` is.

Using these variables for given reactions we can derive a formula for
present value of happiness of each reaction option. Then we can conclude
the topic by comparing these numbers.

    PV of NH1 = H1 - (UH1 / I) 
    PV of NH2 = (P2 * H2 / I) - UH2  

If `NH1 > NH2` that means you preffer short-term happiness to long-term
happiness, if `NH2 > NH1` vica versa. If `NH1 = NH2` you are indifferent
between these two reactions.

Now, we know the results of these reactions, so why do we always tend to
choose one of them? Actually answer is really simple. Most of us make our
decisions based on our emotions. That means present happiness is more
valualbe then future happiness.

That means there are 2 reasons for not being able to achive your goals. One
of them is P2 being too low, that means you don't believe that you will
achieve you goal no matter how much you work. Second possible reason is
that even if you know that you will achive your goal, it is very hard to
giving up your current happiness to get future happiness. That means you
have high `I`. If that is the reason of your reaction this is really bad,
because that will make very hard to focus on your long-term goals.

## Application: Losing Weight

+ I = My personal constant, depends on my `EQ`

### Reaction 1, Working out:

+ P = Probablity of me having 6 pack
+ H2 = Happiness of being fit
+ UH2 = Cost of working out everyday

### Reaction 2, Living the same daily routine:

+ H1 = Happiness of sitting on the couch
+ UH1 = Cost of having fat body

### Conclusion

My `I` is too high. That means I am not successfull at long-term goals.

## Find the cause and fake it 

There will always be two contradictory actions you can take for any given
goal. One of them will always be 'easy to choose' option and the other one
will be harder to choose. 

Try to understand why you feel like one of them is easier. Find the
variable which causes you to take that action. Try to fake that variable to
change the result of the formula.

For example, these are my solutions to fake high `I`.

+ Plan in advance, and obey your plan no matter what
+ Motivate yourself with frequently with results, for long-term goals
+ Know that your emotions are not always helping you
