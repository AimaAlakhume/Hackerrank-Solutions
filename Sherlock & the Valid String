
def isValid(s):
    
	from collections import Counter
	
	letters = list(s)
	str_dict = Counter(letters)
	
	count_dict = {}
	
	for key, val in str_dict.items():
			if val in count_dict:
					count_dict[val] += 1
			else:
					count_dict[val] = 1

	if len(count_dict) == 1:
			return 'YES'
		
	elif len(count_dict) == 2:
			count = 0
			for key, val in count_dict.items():
					if val > 1:
							count += 1
			if count <= 1:
				cmp = list(count_dict)
	
				num1 = cmp[0]
				num2 = cmp[1]
		
				if num2 == (num1 - 1) or num1 == (num2 - 1):
					return 'YES'
			else:
					return 'NO'
	else:
			return 'NO'

#testing
print(isValid('abccdee'))
