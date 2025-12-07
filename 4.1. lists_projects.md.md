---
assignment: Chapter 4 — Project Solutions
---

# Practice Projects

Answers

1. Project 1 — Comma Code
   - Objective:
     Convert a list into a string like "a, b, c, and d".
   - Answer:

        def comma_code(items):
            if len(items) == 0:
                return ''
            if len(items) == 1:
                return items[0]
            return ', '.join(items[:-1]) + ', and ' + items[-1]

2. Project 2 — Character Picture Grid
   - Objective:
     Print a rotated picture from a 2D grid.
   - Answer:

        grid = [
            ['.', '.', '.', '.', '.', '.'],
            ['.', 'O', 'O', '.', '.', '.'],
            ['O', 'O', 'O', 'O', '.', '.'],
            ['O', 'O', 'O', 'O', 'O', '.'],
            ['.', 'O', 'O', 'O', 'O', 'O'],
            ['O', 'O', 'O', 'O', 'O', '.'],
            ['O', 'O', 'O', 'O', '.', '.'],
            ['.', 'O', 'O', '.', '.', '.'],
            ['.', '.', '.', '.', '.', '.']
        ]

        for x in range(len(grid[0])):
            line = ''
            for y in range(len(grid)):
                line += grid[y][x]
            print(line)
