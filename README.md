# mississippi2
from collections import Counter

def most_frequent():
    freq = str(input())
    a = dict(Counter(freq))

    sorted_dict = sorted(a.items(),key=lambda x : x[1],reverse=True)

    for elem in sorted_dict:
        print(elem[0], '=',elem[1])

most_frequent()
