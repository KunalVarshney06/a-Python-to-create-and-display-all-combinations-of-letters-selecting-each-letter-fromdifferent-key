# a-Python-to-create-and-display-all-combinations-of-letters-selecting-each-letter-fromdifferent-key
import itertools
data = {'1':['a','b'], '2':['c','d']}
combinations = list(itertools.product(*[data[key] for key in data]))
for combination in combinations:
print(''.join(combination))
