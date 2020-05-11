---
title: Shapley Values
categories:
- Models Explainable
feature_image: "https://picsum.photos/2560/600?image=872"
---

I already read a lot of articles about Shapley Values, but none of them make me feel easy to understand, that is why I decided to write this article. I hope this article can help you have another way to understand this value.

So, what is Shapley Value? It’s a value representing the contribution of each person in a cooperative task.

Before goes deeper into the definition and computation of the Shapley value, let’s play a game.

Imagine that A, B, C are working together on a task, how do we know each other’s contributions is?

Imagine also that our current goal is to calculate the marginal contribution of player C.

To do this we create all subsets excluding C and group them into 3 groups: group with 0 people, group with 1 people, group with 2 people.

Assume that f is a task outcome function. We calculate f(∅),f(A),f(B) and f(A,B).
Then when we calculate the outcome when C came in: f(∅,C),f(A,C),f(B,C) and f(A,B,C).

Next, we have an average contribution of C in each group:


The average contribution of C in in-group has 1 people

The average contribution of C in in-group has 2 people
Then we take an average for all groups:

In general, the shapely value can also be expressed as:

Where n is the total number of people, v is a value function.

<img src="https://github.com/tianangthang7/tianangthang7.github.io/blob/master/_posts/_img/default-offline-image.png" alt="hi" class="inline"/>

