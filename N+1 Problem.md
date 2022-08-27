# N+1 Problem

## Problem description

The n+1 problem is a problem occurs in object-relational mapping, here's an example:

Let's give a relationship, a car can have many wheels, this is a one-to-many relationship.

Suppose we want to iterate through all the cars and print a list of corresponding wheels. A n+1 problem occurs when we query a car (which is 1 query) then do n queries to find the wheels that have the matching id (which is n  query).

## Solution

We can instead look up the car and then look up the wheels all at once, then perform matching in-memory to print out the wheels.

