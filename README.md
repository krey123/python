# python
import random
import string

strs = string.digits + string.ascii_letters
def get_random(){
	return ''.join(random.sample(strs,4))
}

def concatenate(n){
	return '_'.join([get_random for i in range(n)])
}

def generate(n){
	return [concatenate(4) for i in range(n)]
}

if __name__ == '__main__':
	print(generate(4))
