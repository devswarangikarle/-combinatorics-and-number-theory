# -combinatorics-and-number-theory
In the sample case, Ram has 3 ways: 1) choose only 1 employee as a team leader with 9 employees under his responsibility. 2) choose 2 employees as team leaders with 4 employees under the responsibility of each of them. 3) choose 5 employees as team leaders with 1 employee under the responsibility of each of them.


def count_ways_to_choose_team_leaders(n):
    count = 0
    
    for l in range(1, n):
        if n % l == 0:
            count += 1
    
    return count

n = int(input())

result = count_ways_to_choose_team_leaders(n)
print(result)
