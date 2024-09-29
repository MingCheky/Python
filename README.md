def name(s):
    return s[0]


def age(s):
    return s[1]


def height(s):
    return s[2]


def weight(s):
    return s[3]


athletes = [('Дима', 10, 130, 35), ('Тимур', 11, 135, 39), ('Руслан', 9, 140, 33), ('Рустам', 10, 128, 30),
            ('Амир', 16, 170, 70), ('Рома', 16, 188, 100), ('Матвей', 17, 168, 68), ('Петя', 15, 190, 90)]

options = {1: name, 2: age, 3: height, 4: weight}
for i in sorted(athletes, key=options[int(input())]):
    print(*i)


--------------------------------------------------------------------------------------------------------------
def compair(s):
    return sum([int(i) for i in s])


numbers = [str(j) for j in input().split()]
print(*sorted(numbers, key=compair))
