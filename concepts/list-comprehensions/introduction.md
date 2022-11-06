# Introduction

[List comprehensions][list comprehension definition] in Python provide a concise method of 
creating lists and performing operations on them. Below is the syntax of a simple list comprehension:

[**expression** for **variable** in **list**]

**Expression**: The operation we perform on a variable belonging to the list

**Variable**: Temporary variable used to loop through the list, just like in a for-loop

**List**: The list which we want to transform.

A list comprehension can act as a replacement of a for-loop. Let's say that we have a list of strings,
where each string is a user's first and last name, written in title case. We would like to transform this into a list
of usernames that have the underscore as a separator. Here's how we could do this with a for-loop:


    def get_normalised
        normalised = []
        for name in names:
            name = name.lower().replace(' ','_')
            normalised.append(name)
        
        return normalised
        
    names = ['Joan Smith','Kyle Summers','Eleanor Paddington','Joshua Steele']
    get_normalised(names)
    ['joan_smith', 'kyle_summers', 'eleanor_paddington', 'joshua_steele']

While this approach is valid, we can simplify the above function with a list comprehension:

    def get_normalised(names):

        return normalised =  [name.lower().replace(' ','_') for name in names]


    get_normalised(names)
    ['joan_smith', 'kyle_summers', 'eleanor_paddington', 'joshua_steele']

## List comprehensions with conditional statements



[list comprehension definition]: https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions
